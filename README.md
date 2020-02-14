The utility that does rule-based validation checks

# Eample

###### `ruleSet.js`
Refer [ruleSet](#ruleSet) for [`fields`](#ruleSetFields) and [`rules`](#ruleSetrules)
```js
module.exports = ruleSet = {
    fields: {
        'fname': ['name', 'fname'],
        'lname': ['name', 'lname'],
    },
    rules: [
        { name: 'required', fields: ['fname', 'lname', 'email', 'consent'], required: true, error: 'this field is required' },
        { name: 'length', fields: ['fname', 'lname'], validators: { regex: /.{2,}/ }, error: 'too short' },
        { name: 'contact', fields: ['email'], validators: { regex: /^(([0-9a-zA-Z])+([-._'+&]))*[0-9a-zA-Z]+@([-0-9a-zA-Z]+[.])+[a-zA-Z]{2,6}$/ }, error: 'invalid email' },
        { name: 'agreement', fields: ['consent'], validators: { value: true }, error: 'consent needed' },
        { name: 'gender', fields: ['gender'], validators: { values: ['male', 'female', 'non-binary'] }, error: 'gender is required' },
        { name: 'address', fields: ['city', 'zip'], validators: { fn: (value, field, data, rule) => true }, error: 'address is incorrect' },
    ],
}
```

Include `validate` utility and [`ruleSet.js`](ruleSetjs)
```js
const validate = require('../util-validator/index.js')
const ruleSet = require('./ruleSet.js')
```

### Complete Form Validation
```js
...
const formData = {
    name: {
        fname: 'TestFirst',
        lname: 'TestLast'
    },
    email: 'someone@gmail.c',
    gender: 'male',
    city: 'new york',
    zip: 90210
}
const formErrors = validate(ruleSet.rules, formData, ruleSet.fields)
console.log(JSON.stringify(formErrors))
/* Output:
{
    "consent": {
        "required": "this field is required",
        "agreement": "consent needed"
    },
    "email": {
        "contact": "invalid email"
    }
}
*/
```

### In-Place Validation
```js
...
const fieldData = {
    __fields: ['email'],
    email: 'someone@gmail.c',
}
const fieldErrors = validate(ruleSet.rules, fieldData, ruleSet.fields)
console.log(JSON.stringify(fieldErrors))
/* Output:
{
    "email": {
        "contact": "invalid email"
    }
}
*/
```

# ruleSet
ruleSet has [`rules`](#ruleSetrules) to validate incoming data, and will return the `errors` based on the validity of individual rules.

## ruleSet > rules
```js
{
    name: 'contact',
    fields: ['email'],
    validators: {
        regex: /^(([0-9a-zA-Z])+([-._'+&]))*[0-9a-zA-Z]+@([-0-9a-zA-Z]+[.])+[a-zA-Z]{2,6}$/
    },
    error: 'invalid email'
}
```
- `name`: The unique name for the rule
- `fields`: List of fields that the rule will be applied to
- `required` (optional): If the values of the fields are mandatory
- `validators`: List of validators used to validate the fields
- `error` (optional): The error message that will be returned when the rule fails for a field

### ruleSet > rules > Validators
Validators are used to determine if the fields pertaining to a rule are valid.
Validity checks may include
- `values`: expects the value of the field to be from a list of values
- `regex`: expects the value of the field to be suffice the regular expression(s) provided
- `fn`: a custom function to evaluate if the field is valid or not

#### ruleSet > rules > Validators > fn
This custom function will be called for each field in the rule
```js
{ fn: (value, field, data, rule) => true|false }
```
- `value`: the value of filed being processed
- `field`: the field being processed
- `data`: the original input
- `rule`: the rule object that this custom function belongs to

## ruleSet > Fields
A mapping of fields in case the data coming in isn't a flat object. The fields in `ruleSet > rules > fields` will use this mapping when provided (defaults to `data.fieldName`)
```js
{
    'fname': ['name', 'fname'],
    'lname': ['name', 'lname'],
}
```
Where `fname` is the name used in the `ruleSet > rules > fields` which will resolve with `R.path(['name', 'fname'])` ([Ramda Path](https://ramdajs.com/docs/#path)) to retrieve value of `fname`

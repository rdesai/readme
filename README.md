# Usage
###### `ruleSet.js`
Refer [ruleSet](https://github.com/KlickInc/klick-dataservice/packages/124980#ruleSet) for [`rules`](https://github.com/KlickInc/klick-dataservice/packages/124980#ruleSet--rules) and [`fields`](https://github.com/KlickInc/klick-dataservice/packages/124980#ruleSet--fields)
```js
module.exports = ruleSet = {
    rules: [
        { name: 'required', fields: ['fname', 'lname', 'email', 'consent'], required: true, error: 'this field is required' },
        { name: 'length', fields: ['fname', 'lname'], validators: { regex: /.{2,}/ }, error: 'too short' },
        { name: 'contact', fields: ['email'], validators: { regex: /^(([0-9a-zA-Z])+([-._'+&]))*[0-9a-zA-Z]+@([-0-9a-zA-Z]+[.])+[a-zA-Z]{2,6}$/ }, error: 'invalid email' },
        { name: 'agreement', fields: ['consent'], validators: { value: true }, error: 'consent needed' },
        { name: 'gender', fields: ['gender'], validators: { values: ['male', 'female', 'non-binary'] }, error: 'gender is required' },
        { name: 'address', fields: ['city', 'zip'], validators: { fn: (value, field, data, rule) => true }, error: 'address is incorrect' },
    ],
    fields: {
        'fname': ['name', 'fname'],
        'lname': ['name', 'lname'],
    },
}
```


```js
module.exports.triggers = [
  {
    name: 'dataservice-httpjson-validate',
    enabled: true,
    options: {
      data: ['body'],
      ...require('ruleSet.js') // i.e. { rules: ruleSet.rules, fields: ruleSet.fields }
    }
  }
]
```
## triggers > options

- `data`: the path to the data in the `input` being passed to the trigger. default: `data: input`
- [`rules`](https://github.com/KlickInc/klick-dataservice/packages/124980#ruleSet--rules)
- [`fields`](https://github.com/KlickInc/klick-dataservice/packages/124980#ruleSet--fields)

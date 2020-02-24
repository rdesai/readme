# [@KlickInc/util-validator](https://github.com/KlickInc/klick-dataservice/tree/core/utils/util-validator) *0.0.8*

> Used to validate json data with given rules


### index.js


#### module.exports(trigger, errKey, errVal) 

Refer [ruleSet](#ruleSet) for [`rules`](#ruleSet--rules) and [`fields`](#ruleSet--fields)

Options:

  - `stream` defaulting to _stdout_




##### Parameters

| Name | Type | Description |  |
| ---- | ---- | ----------- | -------- |
| trigger | `String`  | The trigger name of the error creating trigger | &nbsp; |
| errKey | `String`  | The name of the error | &nbsp; |
| errVal | `Any`  | The value of the error. Can be any time | &nbsp; |




##### Examples

```javascript
input.addError(‘triggername’, ‘error1’, ‘errorvalue’) //=> null 
Examples:

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


##### Returns


-  null




*Documentation generated with [doxdox](https://github.com/neogeek/doxdox).*

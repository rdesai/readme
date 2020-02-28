# [@KlickInc/util-validator](https://github.com/KlickInc/klick-dataservice/tree/core/utils/util-validator) *0.0.8*

> Used to validate json data with given rules


### index.js


#### module.exports(trigger, errKey, errVal) 

Refer [ruleSet](#ruleSet) for [`rules`](#ruleSet--rules) and [`fields`](#ruleSet--fields)

Options:

  - `stream` defaulting to _stdout_
  
  

<details>
  <summary>(trigger, errKey, errVal)</summary>
  <p> - by Refsnes Data. All Rights Reserved.</p>
  <p>All content and graphics on this web site are the property of the company Refsnes Data.</p>
  ##### Parameters

  | Name | Type | Description |  |
  | ---- | ---- | ----------- | -------- |
  | trigger | `String`  | The trigger name of the error creating trigger | &nbsp; |
  | errKey | `String`  | The name of the error | &nbsp; |
  | errVal | `Any`  | The value of the error. Can be any time | &nbsp; |
</details>







##### Examples

```javascript
input.addError(‘triggername’, ‘error1’, ‘errorvalue’) //=> null
```


##### Returns


-  null




*Documentation generated with [doxdox](https://github.com/neogeek/doxdox).*

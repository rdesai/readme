# [@KlickInc/util-validator](https://github.com/KlickInc/klick-dataservice/tree/core/utils/util-validator) *0.0.8*

> Used to validate json data with given rules


### index.js


#### module.exports(trigger, errKey, errVal) 

Refer [ruleSet](#ruleSet) for [`rules`](#ruleSet--rules) and [`fields`](#ruleSet--fields)

Options:

  - `stream` defaulting to _stdout_
  
<style>.red { color: red }</style>
<span class="red" style="color: blue">Test</span>

##### Parameters

| Name | Type | Description |  |
| ---- | ---- | ----------- | -------- |
| trigger | `String`  | The trigger name of the error creating trigger | &nbsp; |
| errKey | `String`  | The name of the error | &nbsp; |
| errVal | `Any`  | The value of the error. Can be any time | &nbsp; |




##### Examples

```javascript
input.addError(‘triggername’, ‘error1’, ‘errorvalue’) //=> null
```


##### Returns


-  null




*Documentation generated with [doxdox](https://github.com/neogeek/doxdox).*

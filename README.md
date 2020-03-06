## Modules

<dl>
<dt><a href="#module_index">index</a></dt>
<dd><p>Validation</p>
</dd>
</dl>

## Functions

<dl>
<dt><a href="#create">create(data, errors, headers)</a> ⇒ <code>object</code></dt>
<dd><p>Create input</p>
</dd>
</dl>

<a name="module_index"></a>

## index
Validation


| Param | Type | Default |
| --- | --- | --- |
| rules | <code>Array</code> |  | 
| data | <code>Object</code> |  | 
| [fields] | <code>Object</code> | <code>{}</code> | 

<a name="create"></a>

## create(data, errors, headers) ⇒ <code>object</code>
Create input

**Kind**: global function  

| Param | Type |
| --- | --- |
| data | <code>\*</code> | 
| errors | <code>\*</code> | 
| headers | <code>\*</code> | 


* [create(data, errors, headers)](#create) ⇒ <code>object</code>
    * [.setData(d)](#create.setData)
    * [.getData()](#create.getData)
    * [.addError(trigger, errKey, errVal)](#create.addError)
    * [.rmError(trigger, errKey)](#create.rmError)

<a name="create.setData"></a>

### create.setData(d)
set the data

**Kind**: static method of [<code>create</code>](#create)  

| Param | Type |
| --- | --- |
| d | <code>\*</code> | 

<a name="create.getData"></a>

### create.getData()
get the data

**Kind**: static method of [<code>create</code>](#create)  
<a name="create.addError"></a>

### create.addError(trigger, errKey, errVal)
add the error

**Kind**: static method of [<code>create</code>](#create)  

| Param | Type |
| --- | --- |
| trigger | <code>\*</code> | 
| errKey | <code>\*</code> | 
| errVal | <code>\*</code> | 

<a name="create.rmError"></a>

### create.rmError(trigger, errKey)
remove the error

**Kind**: static method of [<code>create</code>](#create)  

| Param | Type |
| --- | --- |
| trigger | <code>\*</code> | 
| errKey | <code>\*</code> | 


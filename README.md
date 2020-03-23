<a name="module_validate"></a>

## validate "updated"
Utility to do rule-based validation checks


| Param | Type | Default | Description |
| --- | --- | --- | --- |
| rules | <code>Array</code> |  | [rules] {module:validate~rules} |
| data | <code>Object</code> |  | JSON data to be validated |
| fields | <code>Object</code> | <code>{}</code> | Map of fields if the `data` isn't a flat object |

**Example**  
```js
{
    rules: [{
        name: 'Required',
        fields: ['firstname', 'lastname', 'email', 'specialty', 'term-of-use'],
        required: true,
    }, {
        name: 'Name',
        fields: ['firstname', 'lastname'],
        validators: [/^[^\d]*$/],
    }, {
        name: 'Contact',
        fields: ['email'],
        validators: [/^(([0-9a-zA-Z])+([-._'+&]))*[0-9a-zA-Z]+@([-0-9a-zA-Z]+[.])+[a-zA-Z]{2,6}$/],
    }, {
        name: 'Specialty',
        fields: ['specialty'],
        validators: [['Rheumatologist', 'Cardiologist', 'Pulminologist', 'Gastroenterologist', 'Primary Care', 'NP/PA', 'Other']],
    }, {
        name: 'Agreement',
        fields: ['term-of-use'],
        validators: [true],
    }],
    fields: {
        firstname: ['name', 'firstname'],
        lastname: ['name', 'lastname']
    },
}
```

* [validate](#module_validate)
    * [~rules](#module_validate..rules)
        * [new rules(name, fields, required, [validators])](#new_module_validate..rules_new)

<a name="module_validate..rules"></a>

### validate~rules
Rules are set of validators used to determine validaity of the data

**Kind**: inner class of [<code>validate</code>](#module_validate)  
**Typicalame**: rules  
<a name="new_module_validate..rules_new"></a>

#### new rules(name, fields, required, [validators])

| Param | Description |
| --- | --- |
| name | The unique name for the rule |
| fields | List of fields that the rule will be applied to |
| required | (optional)                         If the values of the fields are mandatory |
| [validators] | (optional if `required: true`) List of validators used to validate the fields |

**Example**  
```js
{
    name: 'contact',
    fields: ['email'],
    required: true,
    validators: [/^(([0-9a-zA-Z])+([-._'+&]))*[0-9a-zA-Z]+@([-0-9a-zA-Z]+[.])+[a-zA-Z]{2,6}$/]
}
```
> Generated by Klick DataService Doc builder

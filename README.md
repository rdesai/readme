<p>Refer <a href="#ruleSet">ruleSet</a> for <a href="#ruleSet--rules"><code>rules</code></a> and <a href="#ruleSet--fields"><code>fields</code></a></p>
<p>Options:</p>
<ul>
<li><code>stream</code> defaulting to <em>stdout</em></li>
</ul>
<p>Examples:</p>
<pre><code> module.exports = ruleSet = {
     rules: [
         { name: 'required', fields: ['fname', 'lname', 'email', 'consent'], required: true, error: 'this field is required' },
         { name: 'length', fields: ['fname', 'lname'], validators: { regex: /.{2,}/ }, error: 'too short' },
         { name: 'contact', fields: ['email'], validators: { regex: /^(([0-9a-zA-Z])+([-._'+&amp;]))*[0-9a-zA-Z]+@([-0-9a-zA-Z]+[.])+[a-zA-Z]{2,6}$/ }, error: 'invalid email' },
         { name: 'agreement', fields: ['consent'], validators: { value: true }, error: 'consent needed' },
         { name: 'gender', fields: ['gender'], validators: { values: ['male', 'female', 'non-binary'] }, error: 'gender is required' },
         { name: 'address', fields: ['city', 'zip'], validators: { fn: (value, field, data, rule) =&gt; true }, error: 'address is incorrect' },
     ],
     fields: {
         'fname': ['name', 'fname'],
         'lname': ['name', 'lname'],
     },
 }</code></pre>

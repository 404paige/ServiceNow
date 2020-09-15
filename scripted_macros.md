## Scripted Macros

Script macros provide shortcuts for typing commonly used code. To use a macro, type the macro name in a script field and press Tab. The macro name is replaced with the full macro text. 

The following macros are available by default. Administrators can define additional script macros.

To view a list of the macros that are available in your system, type help in a script field and press Tab.

### vargror
--------
GlideRecord query with OR condition
```javascript
var gr = new GlideRecord('$0');
var qc = gr.addQuery('field', 'value1');
qc.addOrCondition('field', 'value2');
gr.query();
while (gr.next()) {

}
```

### vargr
--------
GlideRecord query examples
```javascript
var gr = new GlideRecord(“$0”);
gr.addQuery(“name”, “value”);
gr.query();
If (gr.next()) {

}
```

### method
--------
Standard JavaScript class method
```javascript
/*_________________________________________________________________
   * Description:
   * Parameters:
   * Returns:
   ________________________________________________________________*/
   $0: function() {

   },
```

### info
--------
Add an info message to the current session
```javascript
gs.addInfoMessage("$0");
```

### for
--------
Standard loop for arrays
```javascript
for (var i=0; i< myArray.length; i++) {
//myArray[i];
}
```

### doc
--------
Code documentation (comment) header
```javascript
/**
* Description: $0
* Parameters:  
* Returns:
*/
```

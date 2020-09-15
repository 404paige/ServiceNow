##Dup Checker

```javascript
var dpchk = new GlideAggregate('table');
dpchk.groupBy('number');//  field on which you want to find duplicate
dpchk.addHaving('COUNT', '>', 1);
dpchk.query();
while(dpchk.next())
{
     gs.print(dpchk.number); // adjust field name as per your table
}
```

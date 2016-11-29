### From NodeJs source
#### ../lib/cluster.js L572
---
```javascript
const indexesKey = [ options.address,
                     options.port,
                     options.addressType,
                     options.fd ].join(':');
``` 
It simplify to concat all options to generate a unique indexes. We also can use this to generate a url. 

---
Different `+` and `parseInt` to convert to int.
```javascript
  console.log(+null)            //print 0
  console.log(parseInt(null))   //print NaN
``` 

---
how yield an array with each value excute same function.
``` javascript
const task = co.wrap(function*(x){
   //somework
   return b;
});

const result = yield array.map(task);
```
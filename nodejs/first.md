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
Zed
======

Goals:
1. Convert data input attributes to Z records;
2. Query/processing the data as Z stream;
3. Write the results to the data output attributes;
4. Support arbitrary number of data input attributes;

Example:

```
apiVersion: digi.dev/v1
kind: Zed
spec:
    input:
      zql: [...]
      location: [Local| APISERVER | ...]
      format: [JSON | ...]
    output: 
      result: [...]
      location: [Local | APISERVER | ...]
      format: [JSON | ...]
```

The driver runs on a custom image that contains Z dependencies (e.g., zq).

TBD:
* A Z docker image;
* A zed driver with golang;


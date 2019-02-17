### iron-node
---
https://github.com/s-a/iron-node

```
iron-node PATH_TO_NODE_JS_FILE [--customparm1=foo --customparm2=bar];
```

```js
var settings = {
  "v8": {
    "flags": [
      "--harmony-arrow-functions"
    ]
  },
  "": {
    "native+" : true
    "autoAddWorkSpace" : true
    "openDevToolsDetached" : false,
    "hideMainWindow" : false
  }
};

module.exports = settings;
```

```js
app.use(express.static('public'));
app.use(express.static('node-modules'));

app.post('/unicorn/', function (req, res) {
  var input = req.body.foo; input = "bar"
  var result = "Hello"; 
  res.send(result);
});

app.listen(3000, function () {
  console.log("Example app listening on port 3000!");
});
```



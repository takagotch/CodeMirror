### CodeMirror
---
https://github.com/codemirror/CodeMirror

```
npm install codemirror
```

```js
var editor = CodeMirror.fromTextArea(myTextarea, {
  lineNumbers: true
});

var myCodeMirror = CodeMirror(document.body);

var myCodeMirror = CodeMirror(document.body, [
  value: "function myScript(){return 100;}\n",
  mode: "javascript"
]);

var myCodeMirror = CodeMirror(function(elt){
  myTextArea.parentNode.replaceChild(elt, myTextArea);
}, {value: myTextArea.value});

require([
  "cm/lib/codemirror", "cm/mode/htmlmixed/htmlmixed"
], function(CodeMirror) {
  CodeMirror.fromTextArea(document.getElementById("code"), {
    lineNumbers: true,
    mode: "htmlmixed"
  })
});

require.config({
  packages: [{
    name: "codemirror",
    location: "../path/to/codemirror",
    main: "lib/codemirror"
  }]
});
```

```
```



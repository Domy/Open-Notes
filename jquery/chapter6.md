# 通过Ajax发送数据

```javascript
$.get('/path/to/file', function(data) {
  /*optional stuff to do after success */
});
```

```javascript
$.getJSON('/path/to/file', {param1: 'value1'}, function(json, textStatus) {
    /*optional stuff to do after success */
});
```

```javascript
$.getScript('path/to/file', function(data, textStatus) {
  /*optional stuff to do after getScript */ 
});
```

```javascript
$.post('/path/to/file', {param1: 'value1'}, function(data, textStatus, xhr) {
  /*optional stuff to do after success */
});
```

```javascript
$.ajax({
  url: '/path/to/file',
  type: 'default GET (Other values: POST)',
  dataType: 'default: Intelligent Guess (Other values: xml, json, script, or html)',
  data: {param1: 'value1'},
})
.done(function() {
  console.log("success");
})
.fail(function() {
  console.log("error");
})
.always(function() {
  console.log("complete");
});
```
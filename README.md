# formToObject.js

[![Build Status](https://travis-ci.org/serbanghita/formToObject.js.svg?branch=master)](https://travis-ci.org/serbanghita/formToObject.js) [![Dependency Status](https://www.versioneye.com/user/projects/5446a74944a5254346000085/badge.svg?style=flat)](https://www.versioneye.com/user/projects/5446a74944a5254346000085)

> Convert **HTML forms** with all their **fields** and **values** to **multi-dimensional JavaScript** objects


##### Include

```html
<!-- Include minified script (~2kb) -->
<script src="build/formToObject.min.js"></script>
```

##### Usage

Using the form's id value:

```javascript
var myFormObj = formToObject('myFormId');
console.log(myFormObj);
```

Using the actual DOM Node:

```javascript
var $formNode = document.getElementById('myFormId');
var myFormObj = formToObject($formNode);
console.log(myFormObj);
```

Real case scenario with jQuery AJAX:

```javascript
$.ajax({
  'url': '/app/settings/save/',
  'type': 'post',
  'data': formToObject('saveSettingsForm'),
  'success': function(r){}
});
```

##### Browser support

IE 8, Firefox 3.5, Chrome, Safari, Opera 10, every mobile browser.

##### Screenshot

![](http://serbanghita.github.io/formToObject.js/formToObj-demo.png)

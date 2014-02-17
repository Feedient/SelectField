SelectField
===========
Tiny (~2KB) jQuery-based select field replacement used at [Feedient](https://feedient.com).

![SelectField screenshot](http://i.imgur.com/VRnrvVm.png)

### Dependencies
- [jQuery](http://jquery.com) OR [Zepto.js](http://zeptojs.com/)
- [FontAwesome](http://fontawesome.io) for up/down chevrons.

### Usage

**HTML**
```html
<a class="select" id="select-language">
	<div class="option selected" data-value="en-GB">English (UK)</div>
	<div class="option" data-value="en-US">English (US)</div>
	<div class="option" data-value="nl-BE">Nederlands</div>
	<div class="option" data-value="sv-SE">Svenska</div>
</a>
```

**Initialize selectField**
```javascript
$('#select-language').selectField();
```

**Listen for changes**
```javascript
$('#select-language').on('change', function(e, value) {
	// Do something with value
});
```

**Get value**
```javascript
var value = $('#select-language').attr('data-value');
```

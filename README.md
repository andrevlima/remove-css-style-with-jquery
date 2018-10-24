# remove-css-style-with-jquery

Remove css style applied in an element using jQuery.
It will remove the style attribute of the element targeted.

Just use it:
```javascript
$.fn.css.remove = function(attr) {
  var bodyStyle = this.get(0).style;
  if (bodyStyle.removeAttribute)
      bodyStyle.removeAttribute(attr);
  else        
      bodyStyle.removeProperty(attr);
  return this;
};
```

Usage:
```javascript
$(document.body).css.remove("cursor"); // For example...
```

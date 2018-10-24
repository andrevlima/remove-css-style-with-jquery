# remove-css-style-with-jquery

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

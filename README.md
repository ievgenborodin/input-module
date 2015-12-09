## Custom Input module

*While using web applications on mobile devices we don't necessarily need to have full keyboard, 
which covers the half of our screen, when we need only to enter an integer...*

Use:

* include: **input.js**, **input.css**
* inside of the body of your html add:
```html
  <div id="input-wrap">
    <div id="input">
      <div title="Done" id="input-done">&#10003;</div>
      <div class="brow" id="input-buttons">
        <div id="input-backspace">&larr;</div>
      </div>
    </div>
  </div>
```  
* initialize with: 
```javascript
var inputName = Input.init({
      keys: ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9', 
            'a', 'b', 'c', 'd', 'e', 'f'] /* list of chars you need */
    });
```
* add event to element you need to type on 
```javascript
$('.someHtmlElement').on('click',function(e){
    input.reset($(this));
});
```

### Preview
![Preview image](/preview.jpg)
 

# 演示文档

---



````javascript
seajs.use('autosize', function($){
    $('#textarea').autosize();
});
````

## 无动画

<textarea name="" id="textarea" cols="60" rows="5" style="color:#666;padding:15px;border-color:#ccc;border-radius:5px;"></textarea>

## 带动画

<textarea name="" id="textarea2" cols="60" rows="5" style="color:#666;padding:15px;border-color:#ccc;border-radius:5px;"></textarea>

````css
.animated {
        -webkit-transition: height 0.2s;
        -moz-transition: height 0.2s;
        transition: height 0.2s;
        }
````

````javascript
seajs.use('autosize', function($){
    $('#textarea2').autosize();
    document.body.offsetWidth; // trigger a reflow before the class is changed
    $('#textarea2').addClass('animated');
});
````




# Steam-Profile-Custom
Steam Profile Custom Guide

## 1. Set Image Dimensions

Set the image width to `1000` and height to `1`, then remove the `id` attributes from both elements.

```javascript
$J('#image_width').val(1000).attr('id',''),$J('#image_height').val(1).attr('id','');
```

## 2. Set the Title Value

Define `v_trim` as an identity function and set the title value to a newline followed by 126 tab characters.

```javascript
v_trim=_=>{return _},$J('#title').val(' \n'+Array.from(Array(126),_=>'\t').join(''));
```

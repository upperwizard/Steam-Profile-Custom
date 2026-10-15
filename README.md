# Steam-Profile-Custom
Steam Profile Custom Guide


/*
 * 设置图片尺寸：
 * 将 image_width 的值设为 1000，image_height 设为 1，
 * 然后移除这两个元素的 id 属性。
 */
$J('#image_width').val(1000).attr('id',''),$J('#image_height').val(1).attr('id','');

# 水平垂直居中的方法
## 定位的方式三种
1、父盒子开启相对定位，子元素开启绝对定位。top、left都为50%，margin-top、margin-left分别为子元素的高度一半和宽度一半
2、父盒子开启相对定位，子元素开启绝对定位。top、left都为50%，使用CSS3的方法，transform:translate(-50%,50%)
3、父盒子变为flex弹性盒，justify-content: center;align-items: center;
## JS的方法
获取父元素和子元素的宽度和高度，最后将子元素的top和left设置为父元素的高度-子元素的高度之差/2，父元素的宽度-子元素的宽度之差/2
## 让父元素变成表格
这种方式不太常用，因为表格的水平垂直居中是针对文本的，这就是意味着要将子元素设置为行内元素或者行内块元素。父元素dispaly:table-cell;vertical-align:middle;text-align:center;
子元素display:inline-block;

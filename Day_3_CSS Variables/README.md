#### HTML一些标签用法与作用
* for属性规定label与那个表单元素绑定，label的for属性要与绑定表单元素（input）的ID对应。
绑定完成后，可以通过点击label触发表单元素的默认属性。

* ` type = “range”`  可以显示进度条
* <input type="range" value="0" max="100" min="0" step="5"/> 

* ` type = “color” `
用来创建一个允许用户使用颜色选择器，
<input type="color" value="#8aa8af" id="base-color"/>

* `：root` CSS伪类匹配文档树的根元素，选择器匹配文档根元素，在HTML中，根元素始终为HTML元素。

* filter 修改图片的颜色  blur( px )给图片设置高斯模糊
`img {filter:grayscale(100%) }`

* <code> 在HTML中插入代码块

#### HTML5中的input
input的type属性决定了input元素的类型，常见的有：hidden、text、password、checkbox、radio、file、submit、reset、image、button等，

#### HTML5自定义属性对象Dataset
参考资料
> 
https://www.zhangxinxu.com/wordpress/2011/06/html5%E8%87%AA%E5%AE%9A%E4%B9%89%E5%B1%9E%E6%80%A7%E5%AF%B9%E8%B1%A1dataset%E7%AE%80%E4%BB%8B/

使用 `data-` 前缀设置需要的自定义属性，来进行一些数据的存放。
```
<div id="day2-meal-expense" 
  data-drink="coffee" 
  data-food="sushi" 
  data-meal="lunch">¥20.12</div>
```
获取某个属性的值，可以如下操作：
```
var expenseday2 = document.getElementById('day2-meal-expense');  
var typeOfDrink = expenseday2.dataset.drink;
```

#### JS设置CSS样式的几种方式
使用setProperty
```
element.style.setProperty('height', '300px', 'important');
```
#### 美元符在JS中的使用
> 
https://blog.csdn.net/zwj1030711290/article/details/50265619

#### ：root 全局声明 & CSS 变量
* :root 伪元素匹配文档的根元素，即为`<html>`标签，用于声明全局CSS变量
* CSS Variables，在全局`:root{}`伪类中定义一个CSS变量，形如`--spacing`命名CSS Variables。使用时，`padding:var(--spacing)`







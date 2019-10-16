### 10月5日&10月16日

### 实现过程
#### 阴影实现知识点
> https://www.html.cn/archives/9360

#### 旋转部分知识点
* `transform` 将一根黑色条状div平移，旋转，做原始指针使用。
```
transform: none | transform-functions ;
```
> https://www.runoob.com/cssref/css3-pr-transform.html
rotate(angle) ： 定义 2D 旋转，在参数中规定角度
* `transform-original` 百分比对应的关系
>详细内容
>http://caibaojian.com/transform-origin.html

#### 动画切换部分
`transition` 
```
transition-timing-function属性指定切换效果的速度。此属性允许一个过渡效果，以改变其持续时间的速度。
```
#### 获取系统当前时间
```
const now = new Date();
console.log(now);
const seconds = now.getSeconds( );
const minutes = now.getMinutes( );
const hours = now.getHours( );
```

#### CSS伪元素使用
伪元素：不是真正的页面元素，html中没有对应的元素，但是其用法和表现行为与页面元素一样，可以使用页面元素一样的css样式，伪元素结构无法审查。
```
：after  
：before
```
属性为`content`，内容必须设置，否则伪元素不起作用。

#### 指针旋转轴心与圆心不重合
造成此结果原因是，div块构成的指针具有一定的高度height，其位置由上边界确定，所有通过`margin-top：-height/2`来纠正移位问题。



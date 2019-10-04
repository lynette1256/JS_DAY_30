### 实现效果
当用户输入页面指示的字母时，页面对应字母变大变亮，对应鼓点声音响起。
* * *
### 关键事件
1. 键盘事件
2. 播放声音
3. 改变样式
* * *
### 步骤分解
* HMLT DOM addEventListener()方法

```
document.addEventListener(event, function, useCapture)
```
参数值详情：
```
event：必需。描述事件名称的字符串
function：必需。描述事件触发后执行的函数
useCapture：可选。布尔值，指定事件是否在捕获或者冒泡阶段执行。
```
* HTML document.querySelector() 
返回文档中与指定选择器或选择器组匹配的第一个html元素。如果找不到匹配项，则返回null。
> https://developer.mozilla.org/zh-CN/docs/Web/API/Document/querySelector

* 实现连续敲击发生事件
将按键发生的时间设置为
```
audio.currentTime = 0；
```
当发生连续敲击事件时，对应的按键声不会持续完毕，紧接着按键操作继续发声，形成连续的效果。

* 按钮边框发亮时间 添加css样式classList.add()
```
key.classList.add('playing');
```
`playing ` 对应CSS样式

* transitionend事件
在CSS transition事件结束后触发  
>https://developer.mozilla.org/zh-CN/docs/Web/Events/transitionend



---
title: "十二HTML常用标签"
date: 2020-06-27T17:57:49+08:00
draft: false
---

# a 标签
a标签是一个链接，常用来进行跳转、导航使用。
写法
```html
<a href="//baidu.com" target="_blank">BaiDu</a>
```
属性：
* `href`属性的取值:
```html
网址：
https://baidu.com
http://baidu.com
//baidu.com

路径：(/为http服务开启的目录)
/a/b/a/b/a/b 及/a/b/a.html
index.html 及 ./index.html

id锚点：（值 为 某个元素的id值）
href="#titelOneID"

伪协议：
href="javascript:alert("abc");"
tel="1111"
mailto="a@a.a"
```

* target的取值：
```html
内置名字
_self
_blank 
_top
_parent

程序员写的：
浏览器窗口的 name值
iframe的 name值 
```
* download
##### 作用
下载页面
##### 问题
很多浏览器不支持

* rel=noopener

作用：
* 跳转外部页面
* 跳转内中锚点
* 跳转到邮箱或电话等
  
# img 标签的用法
image标签会发送get请求，展示一张图片。
*前端工程师需要保证图片不会变形*
```html
<img src="" alt="" width="" height=""/>
```
* 属性
`src`是source的意思，值：
1. 可以是网址
2. 可以是路径


`alt`是alternative的意思很容易记住
功能
当图片加载失败后，可以显示文字，代替图片进行说明。

`width`宽 和 `height` 高：
当只写一个的时候，另一个会自适应；如果两个都写，弄不好，图片会变形。

* 事件
`onload`监听如果 加载成功，我们可以做什么 
`onerror`监听如果图片 加载失败，我们可以做什么

* 响应式图片：
```css
*{
    margin:0;
    padding:0;
    box-sizing:boreder-box;
}
img{
    max-width:100%;
}
```

* 可替换元素

# table 标签的用法
`table`标签只能包含`<thead>`、`<tbody>`、`<tfoot>`三个标签。
##### 相关标签：
* `<thead> <tbody> <tfoot>`
这三个标签出现在`table`标签中
* `<tr> `
行
* `<th>` 
行头、列头
* `<td>`
数据

##### 相关样式
* table-layout 值：
1. auto 根据内容设置尽量平均的宽度
> 大多数浏览器采用自动表格布局算法对表格布局。
> 表格及单元格的宽度取决于其包含的内容。

2. fixed 
> 表格和列的宽度通过表格的宽度来设置，某一列的宽度仅由该列首行的单元格决定。
> 在当前列中，该单元格所在行之后的行并不会影响整个列宽。

* 表格之间的间隙
许多浏览器默认样式是有间隙的，需要用如下样式消除：
```css
table{
    border-collapse:collapse;
    border-spacing:0;
}
```
`border-collapse`
> `border-collapse` CSS 属性是用来决定表格的边框是分开的还是合并的。
> 在分隔模式下，相邻的单元格都拥有独立的边框。在合并模式下，相邻单元格共享边框。

`border-spacing` 
> `border-spacing` 属性指定相邻单元格边框之间的距离（*只适用于 边框分离模式* ）。
> 相当于 HTML 中的 cellspacing 属性，但是第二个可选的值可以用来设置不同于水平间距的垂直间距。

# 其他感想
昨天2020年06月27日 18时19分42秒就只学习了12的开头。因为要学的内容太多了，我想全部都记住，不记住=白学，但是要记忆的内容太多了，我感到很绝望。就打了半天半夜的游戏——炉石传说。越是打游戏，压力越大，很难受。
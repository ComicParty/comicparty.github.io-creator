---
title: "十八css总结"
date: 2020-08-11T16:31:00+08:00
draft: false
---

# 浏览器渲染原理
虽然具体渲染过程很复杂，但是还是可以将其分为几个关键路径，如下：

* 处理 HTML 标记并构建 DOM 树
* 处理 CSS 标记并构建 CSSOM 树
* 将 DOM 与 CSSOM 合并成一个渲染树
* 根据渲染树来布局，以计算每个节点的几何信息，再将各个节点绘制到屏幕上
# CSS 动画的两种做法（transition 和 animation）
### transition 补间动画
我们只要设置一个开头 和 一个结尾，中间的动画内容不需要操心会自动补齐，这是补间动画。
transition属性可以被指定为一个或多个 CSS 属性的过渡效果，多个属性之间用逗号进行分隔。
```
transition:属性名|时长|过渡方式|延迟;
```
transform 四个功能 
1. translate
2. rotate
3. scale
4. skew
### animation 帧动画
我们可以通过添加关键帧，来设置中间动画变化。
```
animation:时长|过渡方式|延迟|次数|方向|填充模式|是否暂停|动画名;

/*可以使用 百分比添加关键帧，from==0%,to == 100% */
@keyframes slidein{
    0%{
        /* 开始的时候，怎么变化*/
    }
    30%{
        /* 到30%的时候，怎么变化*/
    }
    to{
        /* 100%的时候，怎么变化*/
    }
}
```

# 其他任何你想写的。
CCS是真的难，我都心理建设一个多月才好的。
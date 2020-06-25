---
title: "如何使用hugo搭建博客 共7步"
date: 2020-06-25T12:32:43+08:00
draft: false
---

正如文章名所说，这是一篇教人用hugo搭建博客的教程。
下面的操作都是在mac上进行的。
步骤，在[hugo官网](https://gohugo.io/getting-started/quick-start/)上面都有

# 下面咱们齐步走

## 1.安装hugo
```
brew install hugo
hugo version
```
成功安装hugo是可以查询hugo版本的
![我这里error了 sudo&chmod红圈中的文字就解决了](/images/boke2/brewinsallhugoerro.png)

## 2.`hugo new site comicparty.github.io-creator`
里面的`comicparty`是使用的github名称，注意要小写。
![恭喜你](/images/boke2/congratulations.png)

## 3.执行肆句话
注意：执行的时候需要下载东西，所以网络要好
![1-4](/images/boke2/3.4.png)

## 4.`hugo new posts/xxx.md`
   
这一步相当于 创建一篇博客，博客名可以自定义

![my-first-post](/images/boke2/博客名.png)

创建成功之后，打开他
![修改内容](/images/boke2/修改博客内容.png)

如果想写第篇博客，还是这个`hugo new post/xxx.md`代码，只需要换个博客名，就行

## 5.`hugo server -D`本地预览博客
![在浏览器中输入 光标选中内容](/images/boke2/本地链接.png)

## 6.修改config.toml文件

![可以修改的4个内容](/images/boke2/可修改内容.png)

```
baseURL= github pages显示的网址
languageCode = 语言 zh-hans 
    zh =中文
    han =汉字
    s =简体
title =标题
theme =主题
```

## 7.使用源代码生成博客 

![hugo最后一行代码](/images/boke2/最后一行代码.png)
输入之后，会看到一个叫 public文件夹，咱们的博客就在里面，把public上传到github上面，就可以炫友了。


## 8.结束
以上就是用hugo写博客的内容了886
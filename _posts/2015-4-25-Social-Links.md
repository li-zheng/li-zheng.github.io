---
layout: post
title: 怎么在Jekyll自定义更多的社交媒体的图标
categories: jekyll
tags: weibo 微博 svg icons
---

在Github开了博客，看了好多的主题，决定还是从最清爽的Jekyll Now开始，后面会慢慢的把内容丰富起来。
  
  第一次只是做把新浪微博的图标链接加到脚注栏里和加了Google Analytics的东西，由于Google Analytics是已经支持的，需要做的仅仅是到Google的网站上去注册相应的一个项目，就可以监控本网站的访问流量了。

  下面主要记录一下怎么添加的新浪微博的图标链接，因为在Google上也没有搜索到相应的信息，还是研究源代码管用，已经成功的完成了。其它的社交网站的图标也类似。
  
  1. 准备图标
  ![weibo](/images/weibo.png)
  这个图标我已经修改好了，注意图标大小一定是40*40的，否者会很难看，最好是支持透明背景的，要不也不好看。
  
  2. 生成图标的base64的data
  这里列了一些可以做这个事情的网站：
  
  [b64.io](http://b64.io/)
  
  [AskApache's Base64 encoder/decoder](http://www.askapache.com/online-tools/base64-image-converter/)
  
  [duri.me](http://duri.me/)
  
  3. 修改_sass/_svg-icons.scss 文件
  
  在最后加上&号并把新的图片的base64的数据粘贴过去就可以了
  
  4. 修改_config.yml 文件
  
  在footer-links下面添加一项 weibo，相应的值填上你在微博的子域名
  
  5. 修改_includes/svg-icons.html 文件
  
  在最后加上一行,里面相应的字符换成weibo

title: html/css学习笔记（二）
date: 2013-05-06
categories:
- Work
tags:
- HTML
- CSS
- Study
comments: true
---

接上篇html/css 学习笔记（一），这段时间项目和个人事情明显加多，进度变慢了，但是得提醒自己不能懒惰，继续总结。。。

这段时间其实还在折腾Gmail template, 从页面来看，变化不大，最多的是是明白html代码架构，更熟练地应用各个属性等。有点痛苦的感觉，也逐渐明白什么叫做扣html。

以下仅仅是我学习到的几个知识点，具体内容和原理都没有详细表述。因为其实这些知识点google得到的结果更准确些：）

### 1. Gmail template继续重构，达到以下几个目标

#### 1）css module

推荐阅读  http://smacss.com/book/type-module

     ```
     new_message li {
     text-align: left;
     margin:0px;
     padding:10px;
     }
     .new_message li.title{
     background-color: black;
     color: white;
     }
     .new_message li.recipients{
     color: #848484;
     border: 1px solid #848484;
     height: 10px;
     }
     ```

#### 2）加入Common.css/ Reset.css

跨浏览器神马的最讨厌了，有木有？那就用reset吧

关心reset历史或者八卦的可以移步 http://ued.taobao.com/blog/2009/03/reset_css_a/
目前比较全的CSS重设(reset)方法总结 http://blog.bingo929.com/css-reset-collection.html

一段相同的css出现了n多次，代码很冗余，有木有？ 那就把公用的部分抽出来放到common.css里吧

### 2. CSS Image Sprites

页面的每个图片都是一个http request,所以如何提高页面加载速度，我们需要把页面中的图片进行组合以较少请求，详情请参考阅读 http://css-tricks.com/css-sprites/

### 3. UI选颜色

如果你也遇到了每次想设置背景颜色，但是不知道具体值，只能写"white/black"的话，请参考阅读 http://html-color-codes.info/chinese/

### 另外，在做项目的时候，总结了2个知识点，分享给大家：

#### 1. clear:both的妙用

如在DIV + CSS设计网页中，经常需要设置多个DIV并列排列，这个时候就需要使用float来实现，但问题出现了，当前面并列的多个 DIV总宽度不足100%，下面的的DIV就很可能向上提，和上一行的并列的DIV在同一行，这不是我们想要的结果。使用Clear属性正好可以解决这一问题。

#### 2. @font-face

http://www.smashingmagazine.com/2011/03/02/the-font-face-rule-revisited-and-useful-tricks/

#### 3. width, height如果可以少用就少用， float: left也要少用，涉及到调浏览器时候的痛苦。

#### 4. 如何让链接a 没有下划线，text-decroation

#### 5. 能去掉不必要的div就尽量去掉----让代码更加清爽

#### 6. Background---设置Button/page background

![Homework: Gmail](https://raw.githubusercontent.com/xmyang/xmyang.github.io/master/images/Homework_Gmail.png)

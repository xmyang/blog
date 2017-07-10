title: html/css学习笔记（一）
date: 2013-04-11
categories:
- Work
tags:
- HTML
- CSS
- Study
comments: true
---

之前也学过几天html/css，但是这2个星期里自我感觉进步最快，简单总结下。。。

### 一、循序渐进之html/css

- ul/li ol/li dl/dt/dd
- block inline元素
- box model---padding margin
- class VS  id
- clear  
- position
- media queries

### 二、必杀技

- clearfix 比如当父元素no float, 子元素float, 并且高度大于父元素时，这样父元素无法被撑开，可用该必杀技
- position: relative 比如想解决radiobutton 图标和字不在一行的问题
- margin: 0 auto  比如解决横向居中的问题
- visibility:hidden 和 display:none的使用场景  

### 三、推荐一个无敌网站
http://learnlayout.com/ 超级适合学前端开发的新手

### 四、我的作业：

![Gmail](https://raw.githubusercontent.com/xmyang/xmyang.github.io/master/images/Homework.png)

gmail.html Html代码

  ```
	<!Doctype html>  
	<html>  
    <head>  
        <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">  
        <link rel="stylesheet" href="gmail.css">  
    </head>  
    <body>  
        <div class="skin">  
        <div class="header">  
                <img class="logo" src="Gmail_logo.png"/>  
            <!-- <div class="input_wrapper"> -->  
                <input class="input"/>  
            <!-- </div> -->  
            <!-- <div class="search_button_wrapper"> -->  
                <input type="button" value="Search" class="search_button"/>  
            <!-- </div> -->  
                <p class="user">xmyang1221@gmail.com</p>  
            <!-- <div style="clear:both;">  
            </div> -->  
        </div>  
        <div class="left_pannel">  
            <input type="button" value="Compose" class="compose">  
            <div>  
                <ul class="ul">  
                    <li>Inbox</li>  
                    <li>Starred</li>  
                    <li>Important</li>  
                    <li>Sent Mail</li>  
                    <li>Drafts</li>  
                    <li>Backlog</li>  
                </ul>  
            </div>  
            <div>  
                <hr class="hr">  
                </hr>  
            </div>  
            <div>  
                <ul class="ul">  
                    <li>xiaoli</li>  
                    <li>xiaohong</li>  
                    <li>xiaohe</li>  
                    <li>xiaozhao</li>  
                    <li>xiaoli</li>  
                    <li>xiaoxiao</li>  
                </ul>  
            </div>      
        </div>  
        <div class="right_pannel">  
            <dl>  
                <dt> xiaoli</dt>  
                <dd class="subject"> welcome to TW</dd>  
                <dd class="time">Apr,8th,2013</dd>  
            </dl>  
            <dl>  
                <dt> Xiaoli</dt>  
                <dd class="subject"> TW policy</dd>  
                <dd class="time">Apr,8th,2013</dd>  
            </dl>  
            <dl>  
                <dt> Xiaoli</dt>  
                <dd class="subject"> TW policy</dd>  
                <dd class="time">Apr,8th,2013</dd>  
            </dl>  
            <dl>  
                <dt> Xiaoli</dt>  
                <dd class="subject"> TW policy</dd>  
                <dd class="time">Apr,8th,2013</dd>  
            </dl>  
            <dl>  
                <dt> Xiaoli</dt>  
                <dd class="subject"> TW policy</dd>  
                <dd class="time">Apr,8th,2013</dd>  
            </dl>  
            <dl>  
                <dt> Xiaoli</dt>  
                <dd class="subject"> TW policy</dd>  
                <dd class="time">Apr,8th,2013</dd>  
            </dl>  
        </div>  
        <div class="new_message">  
                <ul>  
                    <li class="title">New Message</li>  
                    <li class="recipients:">Recipients</li>  
                    <li class="subject:">Subject</li>  
                    <li class="body"></li>  
                    <li class="submit">  
                        <input type="button" value="Send">  
                    </li>  
                </ul>  

            </div>  
        <div>   
    </body>  
	</html>  
  ```

gmail.css Java代码

  ```
	.skin{  
    /*max-width: 800px;
    margin: 0 auto*/  
	}  
		.header{  
    	height: 50px;  
    	border:1px solid grey;  
    	background: #D8D8D8  
	}  

	.logo{  
    	display: block;  
    	height: 50px;  
    	width: 200px;  
    	float: left;  
	}  

	.input{  
    	display: block;  
    	float: left;  
    	padding: 10px 50px;  
    	height: 20px;  
    	width: 100px;  
	}  

	.search_button{  
    	display:block;  
    	float: left;  
    	width: 60px;  
    	height: 30px;  
    	margin-top: 10px  
	}  

	.user{  
		display: block;  
    	float: right;  
    	height: 30px;  
	}  

	.left_pannel{  
    	background: #D8D8D8;  
    	width: 200px;  
    	height: 600px;  
    	float: left;  
	}  

	.compose{  
    	display: block;  
    	float: left;  
    	width: 80px;  
    	margin: 10px auto;  
	}  

	.left_pannel .ul{  
    	display: block;  
    	list-style: none;  
    	width: 60px;  
    	margin:0px;  
    	padding:15px;  
	}  

	.hr{  
    	width:200px;  
    	size:1px;  
    	color:#848484;  
	}  

	.right_pannel{  
    	float:left;  
    	position: absolute;  
    	margin-left: 200px;  
    	height: 600px;  
	}  

	dd.time{  
    	float: right;  
    	width: 100px;  
    	border-bottom: 1px solid #D8D8D8;  
	}  

	dt{  
    	float: left;  
    	width: 80px;  
    	border-bottom: 1px solid #D8D8D8;  
    	padding-left: 5px;  
	}  

	dd.subject{  
    	width: 300px;  
    	float: left;  
    	border-bottom: 1px solid #D8D8D8;  
	}  

	.new_message{  
    	position: absolute;  
    	right: 10px;  
    	bottom: 10px;  
    	border: 1px solid black;  
    	height: 300px;  
    	width: 300px;  
    	background-color: white  
	}  

	.new_message ul {  
    	list-style: none;  
    	margin:0px;  
    	padding:0px;  
	}  

	.new_message li {  
    	text-align: left;  
    	margin:0px;  
    	padding:10px;  
	}  

	.new_message ul li.title{  
    	background-color: black;  
    	color: white;  
    	border-bottom: 1px solid #848484;  
	}  

	.new_message ul li.recipients{  
    	color: #848484;  
    	border: 1px solid #848484;  
    	height: 10px;
	}  

	.new_message ul li.subject{  
    	color: #848484;  
    	border-bottom: 1px solid grey;  
    	height: 10px  
	}  

	.new_message ul li.body{  
    	color: #848484;  
    	height: 120px  
	}  

	.new_message ul li.submit{  
    	background-color: #D8D8D8;  
	}  
  ```
  
### 五、心得

1. 任务驱动，比如，模拟Gmail
2. 针对同一个作业持续完善
3. 网站关于前端开发很多资料，要针对开发过程中遇到的问题一点一点google解决
4. 将html/css各种属性和具体场景关联记忆

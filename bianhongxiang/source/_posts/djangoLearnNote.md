---
title: Django Learn-Note
date: 2016-12-05 11:41:44
tags: [python,django]
categorise:
description: 边洪祥
---
django框架，作为一种高效的web开发方案，从深层次上讲，它是一系列的python类。学习django的过程，其实就是在学习这些python类的使用方法。当然，还有在这些类背后的，高效实现web开发的一系列方法和思想。
<!--more-->
django将整个开发过程以人本原则进行了拆分，使整个开发过程对开发人员更加友好，从而提高开发效率。这也让我意识到，一门编程语言既是能够编写软件产品的生产工具，同时它本身也是一个产品。作为一个产品，我们就不能漠视它的用户--开发人员的感受。用户友好，且能够解决用户的痛点，才是评价好产品的无上标准。这方面，python做得很好，django亦然。
##初识Django
简单看来，django将开发过程分成三个模块：数据库、页面设计和业务逻辑。这三个模块分别对应dba、前端开发人员和后端开发人员。在实际使用时，这三个模块分别对应models.py、index.html、views.py和urls.py文件。没错，确实是对应了四个文件，urls.py文件是用来配置什么样的URL对应什么样的视图的。

我们创建一个简单的django项目，来了解django的基本文件架构。 
``` bash
$ django-admin.py startproject mysite
```
这样会创建一个目录mysite,进入该目录中，启动web服务
```bash
$ cd mysite
$ python manage.py runserver 0.0.0.0:8000
```
现在用浏览器访问地址http://127.0.0.1:8000/，应该可以看到一个Django的欢迎界面。

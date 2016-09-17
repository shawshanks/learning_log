# learning_log
##1.项目目标
我们要编写一个名为"学习笔记"的Web应用程序,让用户能够记录感兴趣的主题,并在学习每个主题的过程中添加日志条目.
"学习笔记"的主页对这个网站进行描述,并邀请用户注册或登录. 用户登录后, 就可以创建新主题,添加条目以及阅读已有的条目.

##2.项目进行中遇到的坑
###2.1 本书357页*在Django中创建项目*
书中所用命令为`django-admin.py startproject learning_log .`
 1. 若用pip安装Django, 命令中所用 `.py`可以不写.
 2. 命令末尾点号作用是,创建的项目最外层根目录省略,直接在当前目录创建真正的项目--真正的python包. 我猜作者用意是,项目建成后就不用
从最外层目录`cd`至项目中, 即可以直接使用`python manage.py`命令了.

###2.2 p431项目部署
 使用`git push hero master`命令推送到Heroku创建的库中时, 没有添加 Procfile文件,导致推送后出现` code=H14 desc="No web processes running" `错误.  并且使用`heroku ps:scale web=1` 出现 `Couldn't find that formation.`
  
  注:
 1. [Heroku Error Codes](https://devcenter.heroku.com/articles/error-codes#h14-no-web-dynos-running)
 2. Pracefile作用: 告诉Heroku启动哪些进程, 以便能正确地提哦那个项目提供的服务.
 

-----------------------------------------------------
1如果您嫌命令麻烦：
可以使用这个一键部署：
https://github.com/onplus/you2php-heroku/tree/web

-----------------------------------------------------
**手动部署：**
**为了您一次能安装成功，请按照以下步骤逐步操作：**


> 1.点击fork这个项目。操作成功后跳转到您的you2php项目页面。

![pH5t3D.png](https://s1.ax1x.com/2018/01/25/pH5t3D.png)

> 2.编辑web/config.php文件，修改里面的第三行，填入您申请的youtube api key。其他几行也可以修改。看注释

![pHhWRg.png](https://s1.ax1x.com/2018/01/25/pHhWRg.png)
![pHhRJS.png](https://s1.ax1x.com/2018/01/25/pHhRJS.png)

> 3.执行命令创建您的heroku应用：

ps：记住把下面命令中的第一条中的you2php改成您的Github用户名，(如：`git clone https://github.com/You-username/you2php-heroku.git` )因为您需要提交您的仓库代码。第三条中{You APP Name}改成您的heroku应用域名前缀名（不需要加花括号）。


```
git clone https://github.com/You2php/you2php-heroku.git

cd you2php-heroku

heroku create {You APP Name}

git push heroku master

heroku ps:scale web=1

heroku open
```


ps：执行上面的命令需要在您的计算机上安装heroku CLI（下载地址：https://devcenter.heroku.com/articles/getting-started-with-php#set-up）



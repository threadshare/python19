
# virtualenv介绍

virtualenv是用于创建独立的python环境，使得多个python应用相互独立。

## virtualenv优点

1. 使得不同应用开发环境相互独立
2. 环境升级不影响其他应用，也不会影响全局的Python环境。（虚拟环境会将全局的python环境进行一个复制）
3. 他可以防止系统中出现包管理混乱和版本的冲突


## 安装virtualenv

`pip install virtualenv`

## 测试virtualenv

`virtualenv testvir`

**Notice**: 执行这个命令之后安装的路径是你当前所在的路径。

![virtualenv 路径](http://upload-images.jianshu.io/upload_images/3027952-a9fa80b632cdb678.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

## 激活virtualenv的方法

### 在目录中激活

我们在上面可以看到我们的testvir的安装目录，他的安装目录如下图：

![testvir 目录结构](http://upload-images.jianshu.io/upload_images/3027952-42d7c0565a406847.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

Scripts目录如下：

![Scripts目录结构](http://upload-images.jianshu.io/upload_images/3027952-20350986b97523da.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

可以看到有activate.bat和deactivate.bat这两个文件，我们在命令行中运行这两个命令：

![activate.bat运行结果](http://upload-images.jianshu.io/upload_images/3027952-e43aeb9565ff8eb6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)




![deactivate.bat运行结果](http://upload-images.jianshu.io/upload_images/3027952-866221d44ace1a0a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

我们每次打开或者关闭都需要知道testvir的位置然后用相应的文件来对文件进行操作才能进入或退出虚拟环境这样太麻烦了。

### virtualenvwrapper激活
**Notice:** 在windows下使用`pip install virtualenvwrapper-win`
                  在linux下使用`pip install virtualenvwrapper`

**command:**
* mkvirtualenv <env-name> 创建一个虚拟环境（这里会放在同一个目录下）
* deactivate 退出虚拟环境
* workon 展示所有的虚拟环境
* workon <env-name> 进入相应的虚拟环境

### 在虚拟环境中安装开发包

`pip install <package>`
`pip uninstall <package>`






# Leanote on OpenShift #

Leanote is an open source, Knowledge and blogging management 
platform written in Go with a MongoDB backend.

The easiest way to install this application is to use the [OpenShift
Instant Application][template]. If you'd like to install it
manually, follow [these directions](https://github.com/leanote/leanote/wiki/leanote-source-installation-tutorial).

For additional deployment and management considerations, see [leanote Wiki](https://github.com/leanote/leanote/wiki).

## Usage

To deploy leanote on OpenShift, you have to do the following:

1. Create a new Openshift "Do-It-Yourself" application
2. Add a MongoDB cartridge to your application
3. Clone this repository
4. Add a new remote "openshift" (You can find the URL to your git repository
   on the Openshift application page)
5. Run `git push --force "openshift" master:master`
6. Wait for deploy to finish
7. Open http://appname-namespace.rhcloud.com/ to verify

-----------------------------------------------------------------------
# Leanote OpenShift 快速安装脚本 #

Leanote是一个使用开源的知识管理和博客系统，程序是Go语言开发MongoDB做后端数据库。

此脚本可以快速帮助你在OpenShift上部署运行Leanote，如果你希望手动安装请参考此[文档](https://github.com/leanote/leanote/wiki/leanote-source-installation-tutorial)。

##使用

在OpenShift上部署leanote需要下列操作：

1. 创建一个OpenShift "Do-It-Yourself 0.1" 应用程序
2. 向你的应用程序中添加一个MongoDB数据库
3. 使用git clone克隆这个git库
4.  添加一个新的名称为"openshift"的remote（你可以在OpenShift中的application页面中找到这个上传git的url）
5. 运行`git push --force "openshift" master:master`
6. 等待部署成功服务启动
7. 打开你的应用地址http://appname-namespace.rhcloud.com/ 查看
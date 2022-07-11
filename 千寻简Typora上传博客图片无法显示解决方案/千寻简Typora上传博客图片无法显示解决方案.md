# :butterfly:千寻简Typora上传博客图片无法显示解决方案

## :notebook_with_decorative_cover: 笔记介绍

大家好，这里是千寻简笔记，我是作者星辰，笔记内容整理并发布，内容有误请指出，笔记源码已开源，前往Gitee搜索《**[chihiro-notes](https://gitee.com/opxc/chihiro-notes)**》感谢您的观看。

作者各大平台直链： [GitHub](https://github.com/MrChihiro) | [Gitee](https://gitee.com/opxc) | [CSDN](https://blog.csdn.net/IUTStar) 

## :bookmark_tabs: 目录

[TOC]

## :man_student:正文

**参考链接**：

- [如何上传本地离线的Typora笔记到CSDN](https://blog.csdn.net/qq_43523503/article/details/108935238)
- [Typora笔记上传到CSDN解决图片问题](https://blog.csdn.net/weixin_43871072/article/details/112979310)

### :a:解决方案

#### :one:下载安装node.js

- [node.js安装教程](https://www.runoob.com/nodejs/nodejs-install-setup.html)

- [官网下载地址](https://nodejs.org/en/download/)

> 安装成功后windows+R，命令行输入下面命令来检测安装成功和版本号：
>
> `node -v` 和 `npm -v`
>
> **安装成功后，切记重启windows**

#### :two:Gitee的操作

- [官网传送门](https://gitee.com/)

1）进入主界面，点击 + `创建新仓库`

![image-20220711061152305](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711061152305.png)

2）新建仓库–>`创建`

![image-20220711061359179](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711061359179.png)

3）申请开源

![image-20220711061603366](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711061603366.png)

> 遇到的问题：内容过于简单（请完善内容、README、不少于 10 字真实有效的简介）
>
> 解决方案：
>
> 第一步：编辑**README.md**，找些内容复制进去。
>
> ![image-20220711062107403](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711062107403.png)
>
> 第二步：新建一个文件，随便是什么都可以。
>
> ![image-20220711063221420](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711063221420.png)
>
> ![image-20220711062938919](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711062938919.png)
>
> 第三步：点击管理`保存提交审核`。
>
> 提示：当前仓库 Web 页面仅限登录用户可访问。仓库公开申请已提交审核中，我们将在 2 个工作日内为你处理。

4）`设置`–>`私人令牌`

![image-20220711063447417](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711063447417.png)

5）生成新令牌，选择权限，保持最小权限的原则。

![image-20220711063503516](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711063503516.png)

![image-20220711063623184](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711063623184.png)

6）复制`私人令牌`，令牌需要保存好。

> 提示：如果你忘记了或者希望更新这个私人令牌，可点击右边按钮重新生成，生成新的令牌后，当前的令牌将不能访问 Gitee OpenAPI。

![image-20220711063815645](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711063815645.png)

#### :three:下载安装PicGo

1）链接

- [PicGo 2.3.0正式版](https://github.com/Molunerfinn/PicGo/releases/tag/v2.3.0)

2）拉到最下面，找到[PicGo-Setup-2.3.0-x64.exe](https://github.com/Molunerfinn/PicGo/releases/download/v2.3.0/PicGo-Setup-2.3.0-x64.exe)，下载安装。

![image-20220711064359995](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711064359995.png)

3）打开PicGo，安装插件：`gitee`

> 提示：默认安装编号1，编号1安装不成功在去安装编号2，安装一个即可。

![image-20220711153532847](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711153532847.png)

4）配置图床

![image-20220711154006609](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711154006609.png)

> repo：存放照片仓库名（opxc/chihiro-images）

![image-20220711070414900](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711070414900.png)

5）测试图床是否成功。

> 导致失败的原因：仓库开源，还没有通过。
>
> ![image-20220711070850322](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711070850322.png)

![image-20220711070749950](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711070749950.png)

> 在相册和gitee上都可以看到文件表示成功。

![image-20220711154211930](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711154211930.png)

#### :four:Typora的设置：`文件`-->`偏好设置`-->`图像`

![image-20220711071730580](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711071730580.png)

#### :five:上传图片

![image-20220711072143939](https://gitee.com/opxc/chihiro-images/raw/master/chihiro-img/image-20220711072143939.png)


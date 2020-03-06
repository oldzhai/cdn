# 在线引导图片

## 方法简绍


### 第一步：新建github仓库

(我已经有这个仓库，so...这不是重点)
接着在本地电脑克隆上图仓库（前提配置好本地git环境和ssh）
命令如下：

cd 某个目录下

git clone git@github.com:你的用户名/cdn.git


### 第二步：上传需要的资源
复制需要的静态资源到本地git仓库中，提交到github仓库上。
命令如下：

cd 到git仓库目录下

// 查看状态

git status

// 添加所以改动

git add .

// 提交

git commit -m '第一次提交'

// 推送至远程仓库

git push

注：jsDeliver不支持加载超过20M的资源，所以一些视频最好压缩到20M以下）


### 第三步：发布仓库

点击release发布
发布版本号1.0（自定义）

### 第四步：通过jsDeliver引用资源

使用方法：

https://cdn.jsdelivr.net/gh/你的用户名/你的仓库名@发布的版本号/文件路径

比如：

//加载js

https://cdn.jsdelivr.net/gh/yremp/cdn@1.0/js/jquery.js

//加载图片

https://cdn.jsdelivr.net/gh/yremp/cdn@1.0/images/hb.png

*重点：这个链接相当于一个外链，使用和直链一样，如下图：
总的来说，外链怎么用，这个链接怎么用*
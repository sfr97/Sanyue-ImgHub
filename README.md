# sanyue_imghub

## Introduction

[cf-pages/Telegraph-Image](https://github.com/cf-pages/Telegraph-Image)项目的一个新前端，实现了**上传图片预览**，**多文件上传**，**拖拽上传**，**整体复制**等功能。

![](https://alist.sanyue.site/d/imgbed/202407182157169.png)

![](https://alist.sanyue.site/d/imgbed/202407182157130.png)

## Features

- 前端开源（可自行修改、打包使用）
- 流畅丝滑的过渡动画~
- 支持批量上传（不限同时选择文件数量，但为了保证稳定性，同时处于上传状态的文件最多为10个）
- 上传文件实现呼吸灯效果
- 上传显示实时上传进度
- 支持整体复制和单独复制（整体复制即将所有链接通过换行串联起来后复制）
- 上传后图片无需手动点击，可直接展示在管理页面中

## Deployment

如果要在**原项目基础上部署新前端**，并且具有定制化需求，只需要三步（**前提是你需要有基本的`git`、`nodejs`等工具的使用能力**）：

1. 将该项目拉到本地，`npm install`，修改环境变量`.env`中的`VUE_APP_SITE_URL`为你自己图床的URL
2. 进行DIY，然后`npm run build`，进入打包好的`/dist`目录，将里面的所有内容复制到`telegraph-image`项目的根目录（如果你还想保留原来的前端，请将原来的`index.html`重命名为`index-bk.html`）
3. 将修改好的`telegraph-image`项目部署上去即可，具体方法参照原项目

如果你需要**开箱即用**的完整项目，我将修改好的项目保存在[MarSeventh/CloudFlare-ImgBed](https://github.com/MarSeventh/CloudFlare-ImgBed)仓库中，你可以遵循以下步骤使用：

1. fork上述仓库
2. 按照原项目部署流程在CF上部署上述项目
3. 所有环境变量按照原项目填写即可（注意如果要完全迁移，原来的KV数据库一定要保留！！！）

**一天手搓出来的前端，后续还会继续完善，有bug欢迎提出。**

**如果觉得项目不错希望您能给个免费的star✨✨✨，非常感谢！**

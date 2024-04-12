## 1 项目简介

这是一本开源程序员面试手册，叫做《程序员面试宝典》。

本书针对常见的面试流程和面试失败原因，提出了具体的解决方案，比如如何写简历、如何谈项目经验等。

书中出现的技术案例，主要与分布式系统架构以及Java技术有关。采用其他技术的朋友，可以忽略这些例子，重点关注面试技巧即可。

如果你已经工作1到3年，就是本专栏最合适的读者。这个阶段的程序员，具备了一定的项目经验和知识深度，只要完善面试技巧，就能冲击更高端的职位。

人生的确没有捷径，但是可以少走弯路。对大多数人来说，职场之路几乎等于人生的道路。提升技术能力和学习面试技巧，尽早进入大厂工作，就比别人少走许多弯路。

程序员长期人机交互，往往重技术逻辑而轻表达能力，许多优秀的人在面试阶段没能很好的表现自己。表达能力的提升不是一朝一夕的，但是只要切实的实践专栏中介绍的技巧和理论，也能大大提高面试成功率。

希望有志之士共同完善这本书，造福那些不善于面试的同仁。

## 2 主要作者

倾城 (https://www.codingbrick.com)

## 3 本地构建

本书基于 GitBook 构建，本地构建步骤如下所示：

### 3.1 修改NPM源

```shell
npm config set registry https://registry.npmmirror.com
```

### 3.2 安装gitbook

```shell
npm install -g gitbook-cli

# 查看版本号
gitbook -V
```

### 3.3 构建项目

```shell
# 安装依赖包
gitbook install
# 构建 
gitbook build
# 构建
gitbook build  --no-live
# 运行 
gitbook serve
# 不带热部署运行 
gitbook serve --no-live
```

### 3.4 安装插件

```shell
npm install gitbook-plugin-lightbox
npm install gitbook-plugin-multipart
npm install gitbook-plugin-search-pro
npm install gitbook-plugin-favicon
npm install gitbook-plugin-hide-element
npm install gitbook-plugin-tbfed-pagefooter
npm install gitbook-plugin-baidu-tongji-with-multiple-channel
npm install gitbook-plugin-intopic-toc
npm install gitbook-plugin-chapter-fold
```

### 错误处理

遇到错误：Error: ENOENT: no such file or directory, stat '\_book\gitbook\gitbook-plugin-fontsettings\fontsettings.js'
解决方案：C:\Users\Administrator\.gitbook\versions\3.2.3\lib\output\website中找到copyPluginAssets.js，打开将它地112行的 confirm: true 为 confirm: false

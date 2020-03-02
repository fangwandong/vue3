# vue3 

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


## Vue-cli3搭建框架
[在安装之前请装好nodeJs](http://nodejs.cn/)

## 安装Vue CLI3

1. 检测vue的版本

```bash
vue -V (V大写)
or
vue --version
```

 2. 安装Vue CLI3

```bash
首先你要卸载Vue CLI2,用命令npm uninstall vue-cli -g卸载；
输入命令npm install -g @vue/cli安装Vue CLI3;
安装完成后，输入命令vue --version，
查看Vue CLI的版本号是否是3.0以上，是代表安装成功。
```

## 生成项目

```bash
vue create project-name （注：项目名称不能大写）
```
1、选择预设，自行选择配置，选择之后会根据你的选择出现对应的询问提示。操作完成后开始下载模版。
![选择预设](https://img-blog.csdnimg.cn/20200120160038796.png)
2、回车按空格选择想要的模板
![在这里插入图片描述](https://img-blog.csdnimg.cn/2020012016031457.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2ZhbmdoYW90aWFuMjAxMg==,size_16,color_FFFFFF,t_70)
3、或者使用视图化安装方式：

```bash
vue ui  命令进行视图安装
```
4、启动项目：进入创建项目的文件夹，执行如下命令进行启动。

```bash
npm run serve  
```
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200120161725528.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2ZhbmdoYW90aWFuMjAxMg==,size_16,color_FFFFFF,t_70)
5、访问 http://localhost:8080/ 出现Vue的欢迎界面，代表已完成项目安装。
![在这里插入图片描述](https://img-blog.csdnimg.cn/20200120162222755.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2ZhbmdoYW90aWFuMjAxMg==,size_16,color_FFFFFF,t_70)

6、注：vue-cli3将webpack的基础配置全部内嵌了，如果需要对webpack进行自定义配置，可以在目录下添加vue.config.js文件中进行调整配置。
    至此已完成项目的安装和搭建，下一篇整理项目目录分析。
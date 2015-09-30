# gulp使用笔记
## 安装gulp

> gulp依赖nodejs，需先安装nodejs。

下面介绍用npm安装gulp的方法。

1、全局安装
npm install --global gulp
或者
npm install gulp -g
	
-------------------------
> 如果本机没有安装gulp，需先全局安装一下，如果已经安装可以跳过此步骤。

使用下列命令检测是否安装：
gulp --version
	
2、当前项目安装

首先需要安装gulp。
然后安装需要的插件。

建议第一次安装的时候生成package.json文件，以后可以直接执行package文件就可以了，不需要一个一个安装插件。
详细的命令行如下
```
npm init   //生成package文件，然后摁enter键一步一步执行，知道结束。
npm install gulp --save-dev   //安装gulp，并且写入到package文件
npm install gulp-less gulp-rename --save-dev   //安装gulp-less，gulp-rename，并且写入到package文件。
```
gulp插件安装完成。

gulp有很多插件，用来完成特定任务。
查看更多gulp插件
http://gulpjs.com/plugins/
	
3、新建gulpfile.js
在当前项目的根目录下新建js文件，命名为gulpfile.js。
	
gulpfile.js文件说明

```javascript	
//载入gulp插件
var gulp = require('gulp'),  
    sass = require('gulp-ruby-sass'),
    autoprefixer = require('gulp-autoprefixer');
    
//创建任务，build-js是任务名
gulp.task("build-js", function(){
  	
})
```
  
## 执行任务
```
gulp taskname
```
	
	
## gulp API

具体api请参考：

http://www.gulpjs.com.cn/docs/api

https://github.com/gulpjs/gulp/blob/master/docs/API.md

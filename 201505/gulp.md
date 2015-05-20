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
使用gulp必须在当前项目安装gulp依赖才能正常使用。
	
用命令行进入到当前项目的根目录，然后执行下列命令：
```
npm install --save-dev gulp
或者
npm install gulp --save-dev
```
	
> 到此为止，gulp已经安装完成。
	
## 安装插件
	
gulp有很多插件，用来完成特定任务。
```
npm install gulp-a-name gulp-b-name
```
> gulp-a-name、gulp-b-name是插件名
	
查看更多gulp插件
http://gulpjs.com/plugins/
	
## 新建gulpfile.js
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

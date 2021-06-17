#CatchZongzi

这是一个端午节接粽子的小游戏，在移动端运行，微信上读取用户信息并记录游戏结果。游戏结束分数提交显示排行榜。

基于[CreateJS](http://www.createjs.com/)引擎开发。

CatchZongzi is a simple game on web that was made by createjs.

##Demo
demo需要微信授权，请用微信扫描打开。

<img src="http://pan.baidu.com/share/qrcode?w=150&h=150&url=http://web.mob.com/wechat/catchzongzi/index.php">

##Blog详情
[【接粽子】小游戏 Made With CreateJs](http://www.mjpiero.cc/2016/10/21/%E3%80%90%E6%8E%A5%E7%B2%BD%E5%AD%90%E3%80%91%E5%B0%8F%E6%B8%B8%E6%88%8F-Made-With-CreateJs/)

##Authors
**majing(Piero)**
- [Blog － http://www.mjpiero.cc/](http://www.mjpiero.cc/)
- [Email － merlu.majing@gmail.com](http://merlu.majing@gmail.com)

##Issues
[Report a Problem](https://github.com/MJPiero/catchzongzi/issues)


gulp --tasks
[13:15:42] Tasks for ~/dev/github/catchzongzi/gulpfile.js
[13:15:42] ├── clean
[13:15:42] ├── build:asset
[13:15:42] ├── build:compass
[13:15:42] ├── build:js
[13:15:42] ├── watch
[13:15:42] └── default


Gulp v4 has breaking changes and that creates some problems with run-sequence package.

As I do not have your gulpfile.js, all I can say upto this point is to try to use Gulp4's gulp.series and gulp.parallel with your gulp tasks, instead of run-sequence.

you may receive an error of the sort of like 'task1, 'task2' could not be completed', in the function of the task, accept the done callback and call the callback in your tasks at the end of the function

Example:

gulp.task('task1', gulp.series('task1-1', function (done) {
   // task 1 code here
    done();
}));

gulp.task('task2', gulp.series('task2-1', function (done) {
   // task 2 code here
    done();
}));

// Similarly Tasks 3 and 4 Code here

gulp.task('main', gulp.series('task1', 'task2', 'task3', 'task4', function (done) {
    done();
}));



https://www.gulpjs.com.cn/docs/api/parallel/


https://github.com/akptp/create-js/archive/master.tar.gz


remote: Enumerating objects: 741, done.
remote: Total 741 (delta 0), reused 0 (delta 0), pack-reused 741
Receiving objects: 100% (741/741), 19.91 MiB | 20.00 KiB/s, done.
Resolving deltas: 100% (128/128), done.

bower install
bower not-cached    https://github.com/components/zepto.git#~1.1.6
bower resolve       https://github.com/components/zepto.git#~1.1.6
bower not-cached    https://github.com/akptp/create-js.git#*
bower resolve       https://github.com/akptp/create-js.git#*
bower cached        https://github.com/sole/tween.js.git#16.3.5
bower validate      16.3.5 against https://github.com/sole/tween.js.git#~16.3.4
bower download      https://github.com/akptp/create-js/archive/master.tar.gz


"./bower_components/zepto/zepto.min.js",
"./bower_components/create-js/PreloadJS/lib/preloadjs-0.6.2.min.js",
"./bower_components/create-js/EaselJS/lib/easeljs-0.8.2.min.js",
"./bower_components/create-js/SoundJS/lib/soundjs-0.6.2.min.js",
"./bower_components/tween.js/src/Tween.js"

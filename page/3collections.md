---
layout: page
title: 收集
permalink: /collection/
icon: bookmark
type: page
---

* content
{:toc}

1. ExplainShell.com 命令解释

  对于Linux用户来说每天都会写各种命令和脚本，那么你可以使用这个网站工具来查看命令式如何工作的,这样可以避免不必要的错误出现；也是一个很好的学习命令的方式

2. BashrcGenerator.com 定制个性命令提示符

  简单说就是个性化生成命令提示符，可将生成的代码写入到用户家目录的.bashrc或者可以设置全局变量文件/etc/profile对所有用户生效

可参考：http://stackoverflow.com/questions/4133904/ps1-line-with-git-current-branch-and-colors

3. Vim-adventures.com 通过RPG游戏练习VIM使用

  通过RPG游戏练习VIM编辑器的使用，使用h,j,k,l字符移动人物来获得新的命令能力和搜集钥匙，查看帮助可使用:help;赶脚这个非常cool!

4. Try Github 在线学习Git版本控制

  十五分钟学会Git，很明显这个网站模拟了一个控制台，以很时尚的界面让人对Git不再望而生畏

5. Shortcutfoo.com

  是一个练习快捷键的好地方，涵盖了vim、sublime、emacs、git等软件的快捷使用方式和友好的说明

6. GitHub Free Programming Books 免费编程书籍

  以Github管理的方式搜集了免费的编程和系统管理等书籍，给作者点1024个赞~~，另外连接是fork原作者，后续增加中文书籍

7. Collabedit.com 实时文本交互聊天

   先说下使用，你可以创建一个文档http://collabedit.com/yb22u填写相关的用户名和选择语言；然后可以将此文档地址发给另一个人，那么互相之间就可以实时看到对方的输入，有高亮语法；使用场合嘛，比如通过collabedit可以考量对方编程能力等

8. Cpp.sh 在线编写运行分享C++代码编辑器

  可在线编辑运行C++代码，亦可Ctrl+Z生成url分享给好友

9. Copy.sh 浏览器运行虚拟机

  又一个非常crazy的工具，在线运行虚拟机，可以选择下载虚拟机镜像也可以上传自己的iso，copy.sh在线运行虚拟机源码：https://github.com/copy/v86；

10. Commandlinefu.com 命令或记录网站

  做运维的应该都知道这个网站，可以分享自己的CLI库，也可以学习借鉴别人的命令脚本

11. Alias.sh 命令别名数据库

  有点类似commandlinefu了，可以通过这个网站借鉴获取和分享有用的命令别名

比如lr别名定义了显示目录树

alias lr='ls -R | grep ":$" | sed -e '\''s/:$//'\'' -e '\''s/[^-][^\/]*\//--/g'\'' -e '\''s/^/   /'\'' -e '\''s/-/|/'\'''

12. Distrowatch.com 提供了Linux发行版的详细信息

  通过Distrowath不仅可以精确的查看互联网都有哪些流行的Linux发行版，还可以查看每个发行版的相关信息如默认桌面环境、默认应用程序及镜像的下载链接；堪称Linux的数据库

13. Linuxmanpages.com 在线查看命令帮助

  相当于系统内部的man、help、info等的综合吧

14. AwesomeCow.com 适用Linux环境的软件搜索引擎

  如果有款win下好用的软件想在linux下使用，或许可以通过AwesomeCow找到与其类似或者一样的软件，或者通过WINE

15. PenguSpy.com Linux好玩游戏合集

16. Linux Cross Reference by Free Electrons 在线查看内核代码及不同版本的差异

===

## 工具

* [box-shadow generator](http://www.cssmatic.com/box-shadow)

    生成 box-shadow 的工具。

* [gradient-generator](http://www.cssmatic.com/gradient-generator)

    渐变生成器。

* [Ultimate CSS Gradient Generator](http://www.colorzilla.com/gradient-editor/)

    也是渐变生成器

* [CSS Generators -CSSREFLEX](http://www.cssreflex.com/css-generators/)

    CSS3 生成器

- [tiny png](https://tinypng.com/)

    用于压缩 png 或 jpg 的在线工具

* [图床 https://sm.ms/](https://sm.ms/)

    有 API 可用。

* [新浪微博图床 Chrome扩展](https://github.com/Suxiaogang/WeiboPicBed)

* [Unix 时间戳 Unix timestamp](http://tool.chinaz.com/Tools/unixtime.aspx)

- [在线正则表达式匹配](https://regex101.com/)
    - 这个功能更强大一点，能清楚的区分出贪婪和懒惰正则。
- [http://regexr.com/](http://regexr.com/)
- [google fonts](https://fonts.google.com/)
  - [Google Fonts 加速代理](https://fengmk2.com/blog/2016/google-fonts-mirror)

## 编程语言

### JavaScript

* [JavaScript 标准参考教程（alpha） -阮一峰](http://javascript.ruanyifeng.com/)

* [JavaScript Promise迷你书 -azu](http://liubin.org/promises-book/)

* [You Don't Know JS (book series)](https://github.com/getify/You-Dont-Know-JS)

* [You Don't Need jQuery](https://github.com/oneuijs/You-Dont-Need-jQuery/blob/master/README.zh-CN.md)

    前端发展很快，现代浏览器原生 API 已经足够好用。我们并不需要为了操作 DOM、Event 等再学习一下 jQuery 的 API。同时由于 React、Angular、Vue 等框架的流行，直接操作 DOM 不再是好的模式，jQuery 使用场景大大减少。本项目总结了大部分 jQuery API 替代的方法，暂时只支持 IE10+ 以上浏览器。

- [YOU MIGHT NOT NEED JQUERY PLUGINS](http://youmightnotneedjqueryplugins.com/)

* [JavaScript 秘密花园](http://bonsaiden.github.io/JavaScript-Garden/zh/)

* [JavaScript 设计模式 系列 AlloyTeam](http://www.alloyteam.com/2012/10/common-javascript-design-patterns/)

### ES2015

- [https://tc39.github.io/ecma262/](https://tc39.github.io/ecma262/)
* [http://www.ecma-international.org/ecma-262/6.0/](http://www.ecma-international.org/ecma-262/6.0/)

    ES2015规范

- [http://es6katas.org/](http://es6katas.org/)

    Learn ES6 by doing it. Fix failing tests. Keep all learnings.

* [30分钟掌握ES6/ES2015核心内容（上）](http://segmentfault.com/a/1190000004365693)

* [30分钟掌握ES6/ES2015核心内容（下）](http://segmentfault.com/a/1190000004368132)

* [《ECMAScript 6入门》 -阮一峰](https://github.com/ruanyf/es6tutorial)

* [EcmaScript6 全规范（含node） -ouvens](https://github.com/ouvens/es6-code-style-guide)

### NodeJS

* [七天学会NodeJS -Nanqiao Deng](https://nqdeng.github.io/7-days-nodejs)

## 框架&脚手架

### webpack

* [Webpack 中文指南 -赵达](https://www.gitbook.com/book/zhaoda/webpack/details)

* [Webpack傻瓜式指南（一） -前端外刊评论 知乎专栏](http://zhuanlan.zhihu.com/FrontendMagazine/20367175)

* [Webpack傻瓜指南（二）开发和部署技巧 -前端外刊评论 知乎专栏](http://zhuanlan.zhihu.com/FrontendMagazine/20397902)

* [Webpack傻瓜指南（三）和React配合开发 -前端外刊评论 知乎专栏](http://zhuanlan.zhihu.com/FrontendMagazine/20522487)

    上述傻瓜指南的原始出处 [https://github.com/vikingmute/webpack-for-fools](https://github.com/vikingmute/webpack-for-fools) Webpack傻瓜式指南

* [Webpack，101入门体验 -Yika](http://www.html-js.com/article/3009)

* [Webpack 入门指迷 -题叶](https://segmentfault.com/a/1190000002551952)

* [https://webpack.github.io/ Webpack 官网](https://webpack.github.io/)


### Vue

* [awesome-vue](https://github.com/vuejs/awesome-vue)
* [Vue.js 和 Webpack（一） -Randy Lu](http://djyde.github.io/2015/08/29/vuejs-and-webpack-1/)
* [Vue.js 和 Webpack（二） -Randy Lu](http://djyde.github.io/2015/08/30/vuejs-and-webpack-2/)
* [Vue.js 和 Webpack（三） -Randy Lu](http://djyde.github.io/2015/08/31/vuejs-and-webpack-3/)
* [Vuejs 1.0 中文系列视频教程 -Laravist](https://laravist.com/series/vue-js-1-0-in-action-series)
* [Vuejs-QQ群 相关资料](https://github.com/jsfront/src/blob/master/vuejs.md) 来自豪情


### React

* [深入理解 React -Thinking in React 中文版](http://reactjs.cn/react/docs/thinking-in-react.html)
* [Thinking in React](http://facebook.github.io/react/docs/thinking-in-react.html)

### AngularJS

- [学习AngularJS 1.x -Harry<harry@andtoo.net>](https://hairui219.gitbooks.io/learning_angular/content/zh/index.html)

    本书是作者 [Harry](https://github.com/hairui219) 在学习和应用AngularJS 1.x 的过程中的资料梳理。希望能对大家学习AngularJS有一定帮助……

* [AngularJS api 官网](https://docs.angularjs.org/api)

* [AngularJS入门教程——AngularJS中文社区提供](https://github.com/zensh/AngularjsTutorial_cn)

* [AngularJS 教程 \| 菜鸟教程](http://www.runoob.com/angularjs/angularjs-tutorial.html)

    类似 w3school 的入门 AngularJS 教程。

### 测试

* [测试框架 Mocha 实例教程 阮一峰](http://www.ruanyifeng.com/blog/2015/12/a-mocha-tutorial-of-examples.html)

## 类库与插件

* [Masonry](http://masonry.desandro.com/)

    瀑布流布局库。

* [jssor](http://www.jssor.com/)

    图片轮播图其 GitHub 地址 [jssor/slider](https://github.com/jssor/slider)

* [cssslider](http://cssslider.com/)

    纯 CSS 的图片轮播图。

- [gumshoe](https://github.com/cferdinandi/gumshoe)

    A simple, framework-agnostic scrollspy script.

- [smooth-scroll](https://github.com/cferdinandi/smooth-scroll)

  A simple vanilla JS script to animate scrolling to anchor links.

## 模块化

* [后端程序员的 JavaScript 之旅 - 模块化（一）](http://lishaopeng.com/2016/02/05/js-module/)
* [后端程序员的 JavaScript 之旅 - 模块化（二）](http://lishaopeng.com/2016/02/11/js-module2/)
* [后端程序员的 JavaScript 之旅 - 模块化（三）](http://lishaopeng.com/2016/02/19/js-module3/)

* [CommonJS 规范 -来自 阮一峰 JavaScript 标准参考教程(alpha)](http://javascript.ruanyifeng.com/nodejs/module.html)

## other articles

- [<head> Cheat Sheet](http://gethead.info/)
* [将footer固定在页面底部的实现方法](https://segmentfault.com/a/1190000004453249)
- [HTML5 视频 By Pete LePage](https://www.html5rocks.com/zh/tutorials/video/basics/)

## 编辑器

### Atom 中常用插件

* auto-beautify
* autoprefixer
* block-comment
* color-picker
* docblockr
* emmet
* jquery-snippets
* jshint
* linter
* linter-csslint
* linter-htmlhint
* minimap
* minimap-git-diff
* minimap-codeglance 滑过 minimap 显示代码
* minimap-find-and-replace 在 minimap 中显示 `ctrl+D` 选中的内容
* open-in-browser
* uglify
* active-power-mode
* atom-terminal-panel
* linter-scss-linter
* atom-ternjs
* file-icons 将图标变成彩色
* autocomplete-paths 自动补充路径
* symbols-tree-view A symbol treeview like taglist

常用的主题：

UI Theme: One Dark

Syntax Theme: Atom Dark or One Dark

## GitBook 及其插件

* [Gitbook 的使用和常用插件 -赵达](http://zhaoda.net/2015/11/09/gitbook-plugins/)
* [gitbook-plugin-expandable-chapters](https://plugins.gitbook.com/plugin/expandable-chapters)

    折叠左侧目录章节。

    <!-- ![](http://ww4.sinaimg.cn/large/7011d6cfjw1f08kmplbj1j20gn05l0tk.jpg) -->

## Chrome 插件
- [Octotree](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc)

    - Code tree for GitHub and GitLab

* [Chrome扩展及应用开发 -图灵电子书](http://www.ituring.com.cn/minibook/950)

* [有哪些鲜为人知却非常有意思、好用的 Chrome 扩展？ -知乎](https://www.zhihu.com/question/23228162#answer-28057391)
* [Dribbble New Tab](https://chrome.google.com/webstore/detail/dribbble-new-tab/hmhjbefkpednjogghoibpejdmemkinbn)

    新建 tab 时，显示 dribbble 上的精选作品。

## Other blogs

- [COLORFUL xiaoa](http://www.xiaoa.name/)

* [进击的马斯特 http://pinkyjie.com/](http://pinkyjie.com/)

    马斯特，87年生人，爱溜冰的码农。技术： Javascript、Python、Mac、iOS

* [Jerry Qu](https://imququ.com/)

    JerryQu，奇虎 360，前端开发，前百度前端。

* [码志 https://mazhuang.org/](https://mazhuang.org/)

    我是马壮，码而生，码而立。就职sogou。

* [小胡子哥 http://www.barretlee.com/](http://www.barretlee.com/)

    李靖，阿里巴巴。

* [Xcat Liu http://blog.xcatliu.com/](http://blog.xcatliu.com/)

    Microsoft Software Engineer II, Meituan Senior Front-End Engineer

* [极限前端 http://ouvens.github.io/](http://ouvens.github.io/)

    Ouvenzhang, 前端工程师，对前端领域的技术知识具有较高的职业能力和探究精神。对响应式页面设计、工程构建组件化、mv*设计实现、前端优化、ES6开发体系等有深入的研究与项目实践。来自腾讯科技。

* [凳子_Joinery 邓智容  http://www.dengzhr.com/](http://www.dengzhr.com/)

* [赵达的个人网站 腾讯高级前端开发工程师](http://zhaoda.net/)

* [Randy](http://djyde.github.io/)

    95年出生的全栈。卢涛南，英文名 Randy，用 djyde 这个ID混迹于网络。

* [JS前端开发群月报 -豪情等人维护](http://www.kancloud.cn/jsfront/month/82796)

## 交互设计相关

- [Framer](https://framerjs.com/)

    Design the impossible with Framer

- [FLINTO](https://www.flinto.com/)

    App Prototyping Tools for Designers

- [Principle](http://principleformac.com/)

    Animate Your Ideas, Design Better Apps

- [https://gyrosco.pe/](https://gyrosco.pe/)

    首页的卡片翻动效果非常赞。

## Comments

{% include comments.html %}

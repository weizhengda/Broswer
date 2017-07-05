

1. 常见的浏览器内核和前缀有哪些？ 微信的浏览器内核是什么

* 常见浏览器内核 Trident、Gecko、WebKit

* 常见浏览器前缀 -webkit-   -moz-  -o-  -ms-

* 微信的内核是QQ浏览器X5内核 ？  qq浏览器的x5内核是基于 –webkit-  所以微信的内核也是-webkit-


2. 怎么让Chrome支持小于12px 的文字

浏览器设置最小字体

3. 以前pc端是如何调试页面的?在哪些浏览器测试你的页面


	IETester        谷歌    火狐       360浏览器     Ie8以上     苹果浏览器   （常见的浏览器必须调试）



4. ie8  ie7  ie6 怎么做兼容？
	
	以前写项目的时候不需要考虑 ie7  ie6的兼容问题   (xp的内置浏览器是ie6，微软自己都不更新 xp  )    （ie7  是 windows  vista ）.如果我们公司要兼容，我知道方法
	加前缀可以搞定   *  _
	ie8 怎么做兼容：    代码符合w3c标准，一般不会有问题。   万一有问题。先在Ie8调试。ok以后再在其他浏览器测试。  
 
	js检测浏览器版本 动态可以加载样式。


5. 说一下ie，谷歌和火狐的兼容性问题？

* 常见的兼容性问题大都出现在ie8以下的浏览器，比如ie6的双边距问题，ie6的3像素问题，盒子模型的计算宽度不一样。Ie6，7中li底部有三像素问题增加浮动解决。
Ie一般用css前缀过滤对不同版本的浏览器兼容实现样式。
 
其他的部分就是一些css3新增的属性，个个浏览器相互不兼容，需要加前缀：
-webkit-        -moz-    -o-      -ms-
 

* Js部分：
Firefox中没有removenode方法。node.parentNode.removeChild(node)

绑定事件：
主流浏览器
.addEventListener      //     .removeEventListener
Ie8以及以下：
.attachEvent          //     .detachEvent

---
layout:     post
title:      "在Github中使用评论"
subtitle:   ""
date:       2016-02-23 13:00:00
author:     "HLF"
header-img: "img/post-bg-digital-native.jpg"
header-mask: 0.3
catalog:    true
tags:
    - Gitgub
    - 评论

---

>由于Github默认只支持纯静态的页面，无法使用自己的数据库，很多功能都无法实现，其中就包括评论。因此，要在Github中使用评论，就要使用第三方社交评论系统插件。

各种第三方评论使用方法大同小异，本博客以多说评论作为例子。

* 首先去多说官网，点击我要安装，然后会调到登录注册页面，注册一个账号进去。

* 按照说明很容易的填写站点相关资料

 	![](http://hlfshy.github.io/img/in-post/duoshuo-reg.jpg)

* 然后进入后台就能看到公共代码，如下：

		<!-- 多说评论框 start -->
		<div class="ds-thread" data-thread-key="请将此处替换成文章在你的站点中的ID" data-title="请替换成文章的标题" data-url="请替换成文章的网址">
		</div>
		<!-- 多说评论框 end -->

		<!-- 多说公共JS代码 start (一个网页只需插入一次) -->

		<script type="text/javascript">
		var duoshuoQuery = {short_name:"****"};
		(function() {
			var ds = document.createElement('script');
			ds.type = 'text/javascript';ds.async = true;
			ds.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') + '//static.duoshuo.com/embed.js';
			ds.charset = 'UTF-8';
			(document.getElementsByTagName('head')[0]
			 || document.getElementsByTagName('body')[0]).appendChild(ds);
		})();
		</script>
**注意：其中data-thread-key请保证唯一性，本博客是使用了Url保证唯一性**

* 然后balabala...没有然后了，就这么简单，快试试看看效果吧！








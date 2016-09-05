---
layout:     post
title:      "网站开发中常用到的Url跳转"
subtitle:   ""
date:       2016-01-11 13:00:00
author:     "HLF"
header-img: "img/post-bg-re-vs-ng2.jpg"
header-mask: 0.3
catalog:    true
tags:
    - php
    - 跳转
    - web

---

>


## HTML Meta设置跳转

html中的meta标签中可以设置跳转，参数可以设置跳转延迟时间和跳转的url地址，使用方法非常简单，就在<head></head>中加上一句：

    <meta http-equiv="Refresh" content="5;url=http://hlfshy.github.io" />



## PHP header()函数设置跳转

PHP的header()函数非常强大，它也可以用来做也门面跳转，如：

	$url = "http://hlfshy.github.io";
	header( "Location: $url" );


## JavaScript 跳转

JavaScript跳转可谓是花样百出，各显神通。

第一种：最常见的方法

    <script language="javascript">
    	window.location.href="http://hlfshy.github.io";
    </script>

第二种：类似后退，很常用而是很容易出问题的地方

	<script language="javascript">
	window.history.back(-1);
	</script>


在网站开发中，熟练使用各种跳转，能让工作效率事半功倍！
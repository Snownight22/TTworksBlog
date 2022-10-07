---
layout: post
title: Nginx源码分析-全局变量cycle初始化
date:   2022-09-10 11:02:00 +0800
categories: Nginx源码分析
tags: C nginx
topping: true
---
 


![ngxStartProcess.png]({{site.baseurl}}/styles/images/nginx/ngxStartProcess.png)  


---
nginx源码基于nginx-1.22.0版本  
**参考**：  
[Nginx 启动初始化过程](https://www.kancloud.cn/digest/understandingnginx/202596)   
[菜鸟nginx源码剖析 框架篇（一） 从main函数看nginx启动流程](https://blog.csdn.net/chen19870707/article/details/41050379)  

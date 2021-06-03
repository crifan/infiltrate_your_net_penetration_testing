# 潜入你的网络：渗透测试

* 最新版本：`v1.1`
* 更新时间：`20210603`

## 简介

先对渗透测试进行宏观概述，属于安全方向的哪个子领域。再介绍基本的渗透测试和攻击的大体流程和涉及内容，再整理出网络攻击和防御的全流程和涉及的方方面面的内容。总结各种渗透测试的手段，包括Web前端的代码注入类的XSS跨站脚本攻击、CSRF跨站请求伪造，后端的SQL注入、RCE远程代码执行、SSRF服务端请求伪造、CORS跨域资源共享、越权访问，后端语言比如Java的反序列号、struts2等，以及文件类的文件包含、文件上传、目录浏览、任意文件读取和下载、XML文件的XXE等；以及其他渗透测试工具，比如漏洞扫描类的Metasploit、AppScan、AWVS、BurpSuite、Cobalt Strike、Nessus、ZAP和其他一些不常见的工具；以及端口扫描类的nmap、Layer等，注入类的sqlmap等以及模糊测试相关工具；然后根据渗透测试阶段，分渗透前、渗透中、渗透后；以及相关的玩网络安全，包括安全日志分析等内容。

## 源码+浏览+下载

本书的各种源码、在线浏览地址、多种格式文件下载如下：

### Gitbook源码

* [crifan/infiltrate_your_net_penetration_testing: 潜入你的网络：渗透测试](https://github.com/crifan/infiltrate_your_net_penetration_testing)

#### 如何使用此Gitbook源码去生成发布为电子书

详见：[crifan/gitbook_template: demo how to use crifan gitbook template and demo](https://github.com/crifan/gitbook_template)

### 在线浏览

* [潜入你的网络：渗透测试 book.crifan.com](http://book.crifan.com/books/infiltrate_your_net_penetration_testing/website)
* [潜入你的网络：渗透测试 crifan.github.io](https://crifan.github.io/infiltrate_your_net_penetration_testing/website)

### 离线下载阅读

* [潜入你的网络：渗透测试 PDF](http://book.crifan.com/books/infiltrate_your_net_penetration_testing/pdf/infiltrate_your_net_penetration_testing.pdf)
* [潜入你的网络：渗透测试 ePub](http://book.crifan.com/books/infiltrate_your_net_penetration_testing/epub/infiltrate_your_net_penetration_testing.epub)
* [潜入你的网络：渗透测试 Mobi](http://book.crifan.com/books/infiltrate_your_net_penetration_testing/mobi/infiltrate_your_net_penetration_testing.mobi)

## 版权说明

此电子书教程的全部内容，如无特别说明，均为本人原创和整理。其中部分内容参考自网络，均已备注了出处。如有发现侵犯您版权，请通过邮箱联系我 `admin 艾特 crifan.com`，我会尽快删除。谢谢合作。

## 鸣谢

感谢我的老婆**陈雪**的包容理解和悉心照料，才使得我`crifan`有更多精力去专注技术专研和整理归纳出这些电子书和技术教程，特此鸣谢。

## 更多其他电子书

本人`crifan`还写了其他`100+`本电子书教程，感兴趣可移步至：

[crifan/crifan_ebook_readme: Crifan的电子书的使用说明](https://github.com/crifan/crifan_ebook_readme)

# Web前端

* 前端安全
  * 背景
    * 移动互联网
      * 前端的攻击
  * 攻击手段 =安全问题
    * 传统
      * `XSS`
      * `CSRF`
    * 新型
      * `网络劫持`
      * `非法调用 Hybrid API`
  * 防护手段
    * 浏览器
      * `CSP`=`Content Security Policy`=(浏览器)`内容安全策略`
        * 用来限制网页资源的加载,包括script、img、iframe等
        * 设置方法
          * 服务端
            * 语言：PHP等
            * 返回
              * 头=header
                * `Content-Security-Policy:default-src 'self'`
          * 前端
            * 通过iframe的csp属性
              * `<iframe csp="script-src 'self'" src="11.php"></iframe>`
            * 通过`html的`meta`头设置
              * `<meta http-equiv="Content-Security-Policy" content="default-src 'self'; img-src https://*; child-src 'none';">`
            * 通过继承父页面的CSP属性
              * 通过iframe src加载的页面不继承原页面的CSP属性，即，使两个页面同源
              * 通过iframe srcdoc、data协议、about:blank协议加载的页面继承父页面的CSP属性
        * 优先级：`服务端返回CSP属性 > 继承的CSP属性 > iframe csp > meta头`
      * `Same-Site Cookies`

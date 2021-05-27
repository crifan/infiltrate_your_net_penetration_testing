# 文件上传

* `文件上传`=`File Upload`
  * 举例
    * 把PHP文件作为图片文件上传，可能导致（攻击者希望实现的）PHP文件被执行
  * 如何利用文件上传漏洞？
    * `双文件后缀`=`Double extension`
      * 举例
        * 实际上是PHP文件，但是名为 `hey.php.jpg`
    * `空字节`=`Nulle byte`
      * 背景知识
        * PHP来自C语言：空字节Null表示字符串的结束
      * 举例
        * 上传文件名为`hey.php%00.jpg`，扩展控制器读取文件时，会误以为是上传了`.jpg`文件，而停在`hey.php`
    * `绕过MIME校验`=`Bypass MIME checking`
      * `MIME`即`content-type`头
        * 组成：主类型`type`和子类型`subtype`
        * 举例
          * `png`文件：`image/png`
      * 举例
        * 上传文件之前，用工具修改`MIME`
          * 网络代理工具
            * `Burp Suite`
          * 浏览器插件
            * `Mozilla addon`
              * `Tamper Data`

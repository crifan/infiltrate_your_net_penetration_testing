# RCE远程代码执行

* RCE
  * =`Remote Code Execution`=`远程代码执行`
    * ==`RCI`=`Remote Code Injection`=`远程代码注入`
    * ->
      * `RCE漏洞`
      * `RCE漏洞攻击`
      * `RCE攻击`
      * `RCI攻击`
  * 用途：用户通过浏览器提交执行命令
    * 由于服务器端没有针对执行函数做过滤，导致在没有指定绝对路径的情况下就执行命令
      * 可能会允许攻击者通过改变`$PATH` 或程序执行环境的其他方面来执行一个恶意构造的代码
  * RCE相关
    * PHP
      * 注：Web端最常见语言是PHP -> 很多Web应用都是PHP写的
      * 弱点 -> 导致RCE
        * `eval`
        * `assert`
        * `preg replace`
  * RCE攻击举例
    * PHP
      ```php
      <?php
      $ping = system("ping -c 1".$_GET['ipadd']);
      ?>
      ```
      * 命令作用：等待一个IP地址的参数
      * 如果攻击者传入`; cat index.php`，则PHP执行后会显示出`index.php`文件的内容
  * 相关工具
    * `Commix`


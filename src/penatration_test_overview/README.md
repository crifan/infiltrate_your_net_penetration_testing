# 渗透测试概述

如之前在[信息安全概览](https://book.crifan.com/books/information_security_overview/website/)中所总结的，信息安全领域内有几个大的方向：

* 线上或线下
  * 侧重线下的
    * 侧重windows系统的：`漏洞和安全`
  * 侧重线上的
    * 侧重远程Web网络的：`渗透测试`
    * 侧重远程工控设备的：`工控安全` ~= `物联网安全`
* 设备和端
  * 侧重移动端：`移动端`安全和破解
    * `安卓`的安全和破解
    * `iOS`安全和破解

而此处主要介绍涉及到**线上**的，尤其是**Web网络**端的 **渗透测试**

## 概述

* `渗透测试` ~= `渗透攻击` ~= `网络攻击` ~= `Web安全` ~= `网络安全`
  * 含义
    * 模拟一种网络攻击，在真正的黑客入侵之前，模拟黑客入侵企业网络来发现薄弱之处
      * 渗透测试工程师完全模拟黑客可能使用的攻击技术和漏洞发现技术，对目标网络、主机、应用的安全作深入的探测，发现系统最脆弱的环节
  * 目的
    * 发现目标系统潜在的业务漏洞风险
  * 标准
    * `PTES`=`Penetration Testing Execution Standard`=`渗透测试执行标准`
      * 包含
        1. Pre-engagement Interactions 前期交互
        2. Intelligence Gathering 信息收集
        3. Threat Modeling 威胁建模
        4. Vulnerability Analysis 漏洞分析
        5. Exploitation 渗透利用
        6. Post Exploitation 后渗透
        7. Reporting 报告
  * 输出
    * 渗透测试报告
      * 几类
        * 只提供一份测试报告, 报告主体内容是 漏洞列表, 漏洞详情
        * 提供简单的 checklist, 一般是以附录的形式写在测试报告中
        * 提供来测试计划, 以及测试报告
  * 常用工具
    * 扫描
      * `漏洞扫描`=`Web漏洞扫描`=`Vulnerability Scanning`
        * `AWVS`
        * `appscan`
        * `Metasploit`
        * `Burp` = `Burp Suite` = `Burpsuite`
        * `Metasploit` = `MSF` = `Metasploit Framework`
        * `CS` = `Cobalt Strike`
      * 端口扫描
        * `nmap`
      * 注入类
        * SQL
          * `sqlmap`
  * 相关
    * `模糊测试`
      * 名词：`模糊测试`=`fuzz`=`fuzz testing`=`fuzzing`
      * 工具
        * `PEACH`=`Peach`=`Peach Fuzzer`
        * `Sulley`
        * `AutoDafe`

## 概念对比

### 安全检测 vs 渗透测试

* 安全检测
  * 横向 地毯式 自动化扫描
* 渗透测试
  * 纵向 深度 人工化入侵

---
layout: post
title: 网络工程综合实训... 
categories: [Teaching Research 计算机网络, 安全, 管理]
description: 
keywords:  
---
------------------------------------------------

# 【】TODO
## github小组(我负责总提供更新，每人编写自己的文档和代码-链接??)  vnote 
### 辅助资料！

#### 报告模板

## 实战
 
### WEB APP
https://www.liaoxuefeng.com/wiki/1016959663602400/1018138095494592

#  Python自动化运维：技术与最佳实践OCR.pdf


## CH01

### 安装 dnspython
C:\Windows\SysWOW64>pip install dnspython
Defaulting to user installation because normal site-packages is not writeable
Collecting dnspython
  Downloading dnspython-2.1.0-py3-none-any.whl (241 kB)
     |████████████████████████████████| 241 kB 242 kB/s
Installing collected packages: dnspython
Successfully installed dnspython-2.1.0
WARNING: You are using pip version 20.3.3; however, version 21.0.1 is available.
You should consider upgrading via the 'c:\program files (x86)\python36-32\python.exe -m pip install --upgrade pip' command.

C:\Windows\SysWOW64>python.exe -m pip install --upgrade pip
Defaulting to user installation because normal site-packages is not writeable
Requirement already satisfied: pip in c:\users\lilian\appdata\roaming\python\python36\site-packages (20.3.3)
Collecting pip
  Downloading pip-21.0.1-py3-none-any.whl (1.5 MB)
     |████████████████████████████████| 1.5 MB 327 kB/s
Installing collected packages: pip
  Attempting uninstall: pip
    Found existing installation: pip 20.3.3
    Uninstalling pip-20.3.3:
      Successfully uninstalled pip-20.3.3
  WARNING: The scripts pip.exe, pip3.6.exe and pip3.exe are installed in 'C:\Users\Lilian\AppData\Roaming\Python\Python36\Scripts' which is not on PATH.
  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
Successfully installed pip-21.0.1


C:\Windows\SysWOW64>pip install dnspython
Defaulting to user installation because normal site-packages is not writeable
Requirement already satisfied: dnspython in c:\users\lilian\appdata\roaming\python\python36\site-packages (2.1.0)



### 安装 IPy
C:\Windows\SysWOW64>pip install IPy

## CH2 

sys.argv[1] ???
### python pycharm带命令行参数代码的调试 
run => edit configuration  =>  parameters
## CH3

### excel【】

psutil + rrd 

### scapy【】


## CH4 
ClamAV -- Pyclamad   -- 只支持linux =虚拟机??


### python-nmap 【】


## CH5 -7  批量运维
5-7->级别更高，更简单




### CH5 

### CH6 paramiko - SSH
堡垒机??




### CH7 

## CH8 WebServer
与JS的区别?? 【】
例如： Nginx, Apache 【】
httpwathch ??
CGI ??

## CH9 -10 集中化 

# CH9 Ansible 【】
实验环境搭建 ??
与CH6 paramiko的关系 【】 ??
YAML 【】
playbook网站【】



### 
https://zhuanlan.zhihu.com/c_126268929 王印 网路行者
网络工程师学习Python的首选专栏

## 实例学习Ansible系列
https://blog.csdn.net/liumiaocn/category_9266573.html

http://www.ansible.com.cn/docs/playbooks_best_practices.html

YAML实践指南：5:python中的YAML文件格式 https://liumiaocn.blog.csdn.net/article/details/95321652#comments_15803229



#### ansible best practice 实践
http://www.ansible.com.cn/docs/playbooks_best_practices.html
https://docs.ansible.com/ansible/latest/user_guide/playbooks_best_practices.html
 https://gitee.com/steeed/ansible-best-practices
https://ansible.leops.cn/advanced/best-practices/

安装python3：https://blog.51cto.com/steed/2288045
python多环境扩展（venv模块）：https://blog.51cto.com/steed/2298681
使用python3的pip安装Ansible：https://blog.51cto.com/steed/2299074
把项目复制到/opt目录下：
$ cd /opt
$ git clone https://gitee.com/steeed/ansible-best-practices.git

-------------------------------------

内容摘要
了解高效实用地使用 Ansible 实现自动化的推荐做法。

• 借助 Ansible 自动化操作执行滚动更新。

• 使用 Ansible 的高级功能来处理数据，包括过滤器和插件。

• 借助 Ansible Playbook，通过 REST API 控制应用。

• 实施红帽 Ansible Tower，以集中协调和扩展红帽 Ansible 自动化。

• 利用红帽 Ansible Tower 的功能来管理复杂的自动化工作流。

• 借助 Git 和红帽 Ansible Tower，实现 CI/CD 业务流程自动化。


## CH16 

自动化运维平台 ???

B/S   C/S   涉及到的角色，功能分配/权限??
两层结构


|        | B/S <br>OMSever |                 C/S<br>OManager                 |
| ------ | --------------- | ----------------------------------------------- |
| 服务器 |                 |                                                 |
| 客户端 | HTML表单         | XRC (XML Resource) ??<br>wxWidgets 业务-界面分离 |

窗体组合分离拖动 ??


# 推荐Ansible作为另外一个学习的对象和工具
ansible是一种自动化运维工具,基于paramiko开发的,并且基于模块化工作，Ansible是一种集成IT系统的配置管理、应用部署、执行特定任务的开源平台，它是基于python语言，由Paramiko和PyYAML两个关键模块构建。

不需要在远程主机上安装client/agents，因为它们是基于ssh来和远程主机通讯的. 【】



常用的自动化运维工具技术特性比较:

项目	Puppet	SaltStack	Ansible
开发语言	Ruby	Python	Python
是否有客户端	有	有	无
是否支持二次开发	不支持	支持	支持
服务器与远程机器是否相互验证	是	是	是
服务器与远程机器的通信是否加密	是，标准的SSL协议	是，使用AES加密	是，使用OpenSSH
平台支持	AIX , BSD, HP-UX, Linux , Mac OSX , Solaris, Windows	BSD, Linux , Mac OS X , Solaris, Windows	AIX , BSD , HP-UX , Linux , Mac OS X , Solaris
是否提供Web UI	提供	提供	提供，但是是商业版本
配置文件格式	Ruby 语法格式	YAML	YAML
命令行执行	不支持，大师可以通过配置模块实现	支持	支持

## https://github.com/ansible/ansible

ansible程序目录结构:
配置文件: /etc/ansible/
执行文件目录: /usr/bin/
lib依赖库: /usr/lib/python2.7/site-packages/ansible/
help文件: /usr/lib/python2.7/site-packages/ansible


Ansible依靠它的简单易用、“零依赖”以及弱抽象获得了无数开发者和运维工程师的青睐。
Ansible 有三个最吸引人的地方：无客户端、简单易用和日志集中控管。
在目前4 大主流的组态管理工具(Puppet, SaltStack, Chef, Ansible) 中， Ansible 是最容易上手，且马上就可以用的工具。

使用Ansible 需要具备什么基础知识？
具备Linux 伺服器(server) 基础操作和管理经验。
会使用ssh 远端连线至server。
知道基本的标准输入(stdin)输出(stdout)等观念。6
会安装Linux套件。7
知道sudo指令在做什么，并且会使用它。8
知道什么是档案权限，并且会修改它。
知道如何启用和停止系统服务(Daemon / Service)。
会撰写简易的脚本(Script)。





## 20 分钟内以完全自动化部署Ansible  中文：https://linux.cn/article-12970-1.html
英文： https://opensource.com/article/20/12/ansible-lab   Set up an Ansible lab in 20 minutes _ Opensource.com.pdf
https://github.com/mikecali/ansible-labs-101   ||  https://github.com/LCL-ZWU/ansible-labs-101


## Ansible中文权威指南 https://ansible-tran.readthedocs.io/en/latest/index.html



#### 奔跑吧Ansible（第2版）：探索自动化配置与部署捷径
作者：(加)Lorin Hochstein,(瑞士)Rene Moser著，贝壳找房SRE团队译

https://chusiang.gitbooks.io/automate-with-ansible/content/06.how-to-use-the-ansible.html
https://ftp.sjtu.edu.cn/debian/pool/main/a/ansible-lint/ 可下载
https://www.jianshu.com/p/c82737b5485c




## P4(Programming protocol-independent packet processors) ??
https://cloud.tencent.com/developer/article/1082003?from=information.detail.python%20sdn


## Linux工具栈

Linux优于Windows的工作，是互联网运维，而不是编程。
https://cloud.tencent.com/developer/article/1078721?from=information.detail.python%20sdn
https://cloud.tencent.com/developer/article/1083592?from=information.detail.python%20sdn


我始终认为Linux是一个大宝库，无论是它的内核的架构、解决问题的思路还是它上面提供的丰富的网络工具都非常值得我们学习。



Tcpdump是帮助我们学习TCP/IP协议的最好助手也是帮助我们Debug的绝对利器，对于它的掌握是毋庸置疑的。Iproute2旨在代替net-tools，ip系列的命令就包含在这个下面。Neutron对它的依赖程度简直是深入骨髓。



Linux的namespace是容器技术的基础，我们可以单独使用其中的某个namespace，比如network namespace。Neutron会针对每个Router或者DHCP启动一个独立的Python进程，这些进程的隔离就是直接通过namespace实现的。



Linux虚拟网络设备也是是Linux创建本地虚拟网络的基础，它提供的Bridge、TAP、VETH几乎成为了标配，无论Neutron、OVS、Docker五花八门的SDN、甚至直接用KVM都会用到这些东西。这部分内容都是“工具”性质的知识，更多强调实际操作所以没有成体系的书籍可以参考，大家去读一些网文。



### H3C
http://www1.h3c.com/en/Support/Resource_Center/Technical_Documents/Home/Switches/00-Public/Configure/Configuration_Guides/H3C_S6850_S9850_CG-Release_655x-6W100/01/201905/1188747_294551_0.htm

https://asmcn.icopy.site/awesome/awesome-sdn/

### sdn ryu:  
https://github.com/joechang0113/sdn-handoff
https://github.com/joechang0113/python-lab-answer
https://github.com/mininet/mininet
https://github.com/dariobanfi/multipath-sdn-controller
https://github.com/shreyakupadhyay/SDN-Datacenter
https://github.com/santhisenan/SDN_DDoS_Simulation
https://github.com/andrew-miao/study_sdn
https://github.com/YanHaoChen/Learning-SDN

https://github.com/sdnds-tw/Ryu-SDN-IP

https://github.com/sdnds-tw/awesome-sdn


如何在Eclipse中搭建基于RYU控制器的开发环境。https://cloud.tencent.com/developer/article/1082877?from=information.detail.python%20sdn

学习如何使用管道命令将多个小工具和脚本整合在一起来完成更大的任务。??


### sdn python 图： 
https://networklessons.com/cisco/ccna-routing-switching-icnd2-200-105/introduction-to-sdn-software-defined-networking  

进行SDN实验需要的工具可以有以下两类：mininet，用于模拟底层网络；控制器，根据自己获取的网络信息告诉底层设备如何转发数据包。如果使用mininet自定义网络topo就需要懂得python。控制器方面的话，pox和Ryu是用python编写的。
开发SDN应用过程中有些需求是要用脚本完成的
之前在菊厂参与过一段时间的NEMO项目，期望搞出一种基于意图和目的的网络编程方法

网工2.0 - 给你一次逆袭的机会2018-12-17
https://www.huaweicloud.com/articles/7a471cdb511e1b46f0b01940f623ee9e.html

以我的《老司机网络运维-读者群》为例。

大家讨论的不光是日常网络故障和经验汇总。

慢慢地，朋友们开始研究如何学习Python。

如何把玩Juniper的PyEZ模块实现日常运维自动化。连这13周年庆学习专栏送书活动。

大家购买的不再是什么思科学习指南。

更多的是Python，Ansible等书籍。



## 云技术，虚拟化，SDN，NetOps网络运维自动化会慢慢撕开你坚固的防线。


基于需求的编程学习法
###  H3C SDN  测试

https://www.icourse163.org/learn/NJU-1001773008?tid=1450627499#/learn/content?type=detail&id=1215355708




### 业界IT巨头网工招聘要求分析


华为CloudEngine系列的设备纷纷开始支持SDN，Python自动化

网络工程师2.0 
业界IT巨头网工招聘要求分析
Google，亚马逊，Facebook
基本上以上几个职位，都提到了同一个东西：写代码的能力。
什么Python，Perl，Go，Java语言，都是必备项。若要是没有这个编程能力

来自 <https://blog.51cto.com/gingerbeer/2162956> 


Google，亚马逊，Facebook

计算机相关本科学位。
熟悉一个或者多个通用型计算机语言，包含但并不限于：C，C++，Python，Java，Go。
熟悉网络架构，企业级网络管理，排错，和日常运维。


3年以上大型网络工作经验。
熟悉网络路由协议：TCP/IP, BGP, MPLS, ISIS and/or OSPF
熟悉Cisco IOS和JUNOS
熟悉自动化，包括bash/shell脚本，Perl、Python编程。

2年ISP运营商、CDN运营商、或者大型企业核心工程师或者设计工程师工作经验。
熟悉IS-IS，BGP，MPLS，并具有使用（OpenConfig，NetConf，YANG）等工具的经验。
熟悉业界网络硬件和软件架构，以及掌握发展趋势。
实际编程经验，包括不限于Python、Go、Perl等语言。尤其是控制和管理网络相关项目的编程经验。
熟悉并协调厂商网络产品研发和支持的工作。
具有展示技术PPT的沟通能力。


###  5G移动基站系统运行与维护 https://www.icourse163.org/learn/cqcet-1461577162?tid=1462360443#/learn/announce

#


#### 

## In python3 package is dnspython3 not dnspython

## 2to3
https://docs.python.org/zh-cn/3.7/library/2to3.html

python 2to3.py的路径 -w 文件路径 -n -o 输出路径

## 课程-资料
网络应用综合实训	李翠莲	8	17	18	星期一二四五	6	9	通信18（B模块）	4302 20201231  


综合实训要求提交课程报告博客git账号代码
网络应用综合实训课表-17-18周.png 20210108




## Python自动化运维：技术与最佳实践.pdf  


https://github.com/yorkoliu/pyauto   源码 python2.X 

https://blog.liuts.com/component/id/5/  
纠错  https://github.com/kurolz/Books/find/master 电子书

2to3_pyauto_log.txt    https://docs.python.org/zh-cn/3.7/library/2to3.html 转换3

### 2020年Python自动化运维系统性20讲
https://www.bilibili.com/video/BV1J7411j7JN
加微信19121525487
课程是按照刘天斯的《python自动化运维》讲的
来我们平台实操学习吧！电脑端百度 云开见明 ??

#### 答疑??
p16-p20 是不是传错了？

为什么发送邮件，还是HTML代码呢？而不是像老师那种 表格
搞定了。    """
,_subtype='html',_charset='utf8')     在后面加。 我是Python3的

在win10系统，py3.8，运行您的那个
p=psutil.Popen(['C:\Users\cy\AppData\Local\Programs\Python\Python38\python.exe',"-c","print('hello world')"],stdout=PIPE) 报错decode

Windows下Pycharm 安装了scrapy后，运行出现：NameError: name 'IP' is not defined
这个怎么解决？

scapy graph方法不能用是怎么回事

第八章中 发送了的是xls文件，收到的是bin二进制文件，怎么都没说明如何发送正常，并收到xls文件

第十七章我出现了TypeError: can only concatenate str (not "bytes") to str这个错误，找了很多方法都没解决【刘天斯的书只有16章??】

在浏览器实现主次屏的是什么系统???


### Python 网络自动化运维-学习视频教程-腾讯课堂

#### Python网络自动化运维【】
是一组将静态的设备结构转化为根据IT服务需求动态弹性响应的策略，目的就是实现IT运维的质量，降低成本

### 四种企业内常用的自动化运维案例【】

* 读取华为交换机数据并导出【监控】
* 获取交换机上活跃计算机的信息（思科） https://www.bilibili.com/s/video/BV1PE411h7NR
* telnet到设备上执行命令【安全隐患】
* 在网页中实现SSH的连接【】


PE1-HWNE40E.log 
read_sw_log.py 
sshDemo.rar 
telnetmodule.py


#####  网络工程师的Python之路：网络运维自动化实战(博文视点出品)
 本书内容基于思科设备和技术
Python零基础网工自学入门/基于Python3.8/资深网络老兵、知乎专栏“网路行者”全力打造/从基础知识到实战应用手把手教学/实战案例源于日常工作

## 通过google上网助手可以访问，但dnspython中查到的IP却ping不通【无法直接访问谷歌，只能通过代理中转?】
通过dns.query得到的：
www.google.com -- 111.243.214.169
www.google.com.hk -- 108.160.169.54；

ping过程中看到的IP：
ping www.google.com.hk   
正在 Ping www.google.com.hk [128.242.240.91]  【与dns.query得到的不一致??!!】

wireshark抓包看到的：
120.204.17.123
120.241.186.223
220.246.94.223
52.7.219.23
52.242.211.89




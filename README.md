# 2021SRE_Winter_SecTask

## 前言

结束了2020秋季的学习与冬季的沉淀，想必大家已经学到了不少吧！！

废话不多说，在指定时间之前提交考核内容即可获得通往SRE下学期学习的门票！！

本次SRE安全方向的考核分为2个大方向--**Web安全**和**二进制安全**！！

本次安全方向考核意在督促大家学习，选择的考核内容都是在上学期学习内容的基础上加上寒假一定的自学时间就能够完成的（多多~~Google~~百度是好文明）

请不要当懒狗！！！请不要当懒狗！！！请不要当懒狗！！！遇到不懂的不会的有问题的一定要及时解决（搜索+提问）！！！

注意：

1. 两个方向任选其中一个提交即可。
2. 提交截止日期：2021年2月27日晚上12:00之前
3. 提交方式：
   1. 提交邮箱：xiaoyaovo@qq.com
   3. 邮件标题：`2020212xxx-张三-Web安全方向/二进制方向`
4. 有任何问题请及时联系@肖瑶
5. 鼓励大家多使用Google，禁止互相抄袭，禁止大面积抄袭网上代码，禁止以各种方式攻击平台

## Web安全方向考核内容

>  2个TASK选择其中一个完成即可

#### [TASK1]AWD自动攻击模拟

给出题目地址 172.23.26.66:12345

在[12345---12354]端口存在10个相同的web服务

flag提交地址：172.23.26.66:10001

##### **Level-0**

​	尝试绕过给出的过滤并获取flag

##### **Level-1**

​	编写python脚本实现自动攻击10台机器并读取flag文件（请将输出结果截图）

##### **Level-2**

​	编写python脚本实现自动攻击，并且能够自动提交flag，每次提交打印出返回的结果（请将输出结果截图）。

##### **其余加分项**

 	1. python代码规范，简洁，优美
 	2. 提交时间早
 	3. 另外在自己的博客里面撰写writeup

##### **注意：**

1. 请至少完成至Level-1
2. 提交时撰写一个md 文档，写出每个level的完成细节与思路，注意排版简洁好看
3. 邮件内容为你的md文档以及python源代码以及必要的截图（有自己写博客可以附加博客地址）
4. 提示： 寒假期间按照大家完成的进度逐渐放出hint
6. 环境崩溃请联系@肖瑶

###### Hint 1：两个入口，一是linux查看文件命令你知道几个，二是百度看看php中的include

###### Hint 2：自动提交还不简单，get换成post即可，顺便看看提交flag的流量包长啥样子

###### Hint 3：未解锁

#### [TASK2]超简单的渗透

给出目标：172.23.26.66:7001

> 备用地址：172.23.26.66:7002

##### **Level-0**

​	请找出目标机器存在的漏洞，如果漏洞是已有CVE，则给出CVE的编号

##### **Level-1**

​	简单阐述漏洞利用方式，防御方式，尝试获取目标机器的webshell （如使用现成POC请贴上POC地址与内容）

##### **Level-2**

​	尝试在本地进行复现漏洞，并且撰写复现文章

##### **Level-3**

​	编写属于自己的poc脚本

##### **注意：**

1. 请至少完成至Level-1
2. 提交时撰写一个md文档，写出每个level的完成细节与思路，注意排版简洁好看
3. 邮件内容为你的md文档以及必要的截图（有自己写博客可以附加博客地址）
4. 提示：寒假期间按照大家完成的进度逐渐放出hint
6. 环境崩溃请联系@肖瑶

###### Hint 1：未解锁

###### Hint 2：未解锁

###### Hint 3：未解锁

## 二进制方向考核内容

#### [TASK3]NWP

题目附件下载地址：https://xiaoyaovo.cn/WinterTask.zip

请写出详细的分析报告（类似WP），图文并茂，使用优雅的Markdown格式将获得加分，word和ppt等不建议，txt扣分，请勿在考核结束前将自己的作业上传到自己的博客等公共网络区域

作弊是真没意思，请勿抄袭、找代做

至少完成一个Level，有任何问题请联系@唐清炀

##### Level-空

​	找到能使程序输出“Chongqing No Water No Electric No Network University”的**长度小于20个字符**的输入

##### Level-荧

​	对文件进行打补丁，使得输入任何**长度小于20个字符**的输入都能让程序输出“Chongqing No Water No Electric No Network University”

##### Level-Paimon

​	在不修改文件、不附加调试器的前提条件下，让程序输出“Redrock”

###### Hint 1：对付SMC的最好办法就是~~面对它~~动态调试，或者试试万能的IDA脚本？BTW，z3了解一下

###### Hint 2：无脑jmp，yyds！也许你需要考虑一下SMC的影响？

###### Hint 3：白给ROP，但是怎么输入数据是需要思考的一个点

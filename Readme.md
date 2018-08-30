# Lockers-client-masterV2.0

   ![](https://i.imgur.com/bvEYtvX.gif)　　
       
## 总体介绍
 Lockers-client-masterV2.0，是Lockers-client-masterV1.0的升级版，在V1.0原有的存样、取样、弃样的功能上增加了

- 判断是否真正存入物品



- 获取样柜门的状态　　



- 新建了被查样异常记录表RLGL _ BYGL _ YCJL　　
　　



　
---
　　
<table>
  <tr>
      <td>　　　　　开发工具　　　　</td>
      <td>　　　　　eclipse　　　　　</td>
      <td>　　　　　exe4j　　　　</td>
  </tr>
  <tr>
      <td>　　　　　开发环境　　　</td>
      <td>　　　　　jdk 1.8　　　</td>
      <td>　　　sqlserver 2008　</td>
  </tr>
</table>



　　　　
　　
　　　　　
　　　

## 代码结构  　　


├──libs　　　　　　　　　　　　　　　　　　//项目所需要的jar包

├──src

│　├──main

│　│　├──ClientContext　　　　　　　　　　//GUI的界面控制核心

│　│　├──DqygFrame　　　　　　　　　　　　//到期样柜界面

│　│　├──KeyPanel　　　　　　　　　　　　//数字键盘控制

│　│　├──LoginFrame　　　　　　　　　　　　//登陆界面

│　│　├──LoginMain　　　　　　　　　　　　//登陆主函数

│　│　├──Main　　　　　　　　　　　　　　　　//主函数

│　│　├──MainFrame　　　　　　　　　　　　　//主界面

│　│　├──RecordFrame　　　　　　　　　　//操作记录界面

│　│　├──SoftKey　　　　　　　　　　　　　　//软键盘

│　├──service

│　│　├──BcyjlService　　　　　　　　　//处理被存样记录逻辑

│　│　├──DzygService　　　　　　　　　　//获取样柜箱体逻辑

│　│　├──UDPClient　　　　　　　　　　　//UDP协议操作样柜

│　│　├──UDPThread　　　　　　　　　　

│　├──entity 　　　　　　　　　　　　　　//设置实体类

│　├──db　　　　　　　　　　　　　　　//连接并设置数据库

│　├──Config　　　　　　　　　　　　　　　//配置文件

│　├──resources

│　│　├──bk.gif　　　　　　　　　　　　　//主界面图片

│　│　├──ds.config.xml　　　　　　　　　//连接数据库配置

│　│　├──log4j.properties　　　　　　　//控制日志的生成过程

│　│　├──login_bg.jpg　　　　　　　　　　//登陆背景

│　│　├──system-config.properties　　　　//系统配置文件

├──.gitignore　　　　　　　　　　　　　　//git忽略项

├──build.gradle　　　　　　　　　　　　　//gradle构建

├──settings.gradle　　　　　　　　　　　//gradle设置

├──Readme.md　　　　　　　　　　　　　　//说明

　![](https://i.imgur.com/82Aq0Ez.png)　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　
　
## 运行方法
  

- [在eclipse中将项目打包成jar;](./jar.md)

- [通过exe4j将jar打包成exe文件;](./exe.md)

- 运行Lockers-Client_v2.0_fat.exe，弹出主页面后自行选择刷卡登陆或者输入账号密码登陆。

## 现场所需要配置的项目

1. [控制面板的基本操作命令](./rule.md)　　

2. [PC端配置读卡器所需文件](./xml.md) 
 
3. [ds.config.xml文件中连接数据库的信息与所要连接的数据库信息相匹对](./dsconfig.md)  

4. [system-config.properties文件中的时间限制和操作员身份](./sysconfig.md)

5. [数据库中RLGL_SYS_IPTEMP表中的ip要与机器ip相匹配](./ip.md)

## 燃料系统与电子样柜之间的关系

- 制样室电子样柜维护

- 化验室电子样柜维护

- 采制化人员分配









 




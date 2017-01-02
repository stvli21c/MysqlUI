# MysqlUI
新年快乐，各位爱写代码的亲！让我们用一个新的程序来庆祝新年吧！

当你在调试代码的时候，是不是常常想要反复检查数据库里的数据？这款只有仅仅 50KB 的小程序 MysqlUI 将将可以满足你的需求，又不用打开巨大的 SQL Studio　和 MySQL Workbench 之类的东东哦。目前已经可以支持SQL Server (Microsoft) 和 MySQL Server 了。不过需要安装MySQL Connector for .Net, 最低要求.Net4.0 Framework. MySQL Connector for .Net 下载地址:
http://dev.mysql.com/downloads/connector/net/


界面简单，
	- 选择数据库类型:　SQL (Microsoft Server)，MySQL 
    
	- Show Table : 查询并返回所有的数据
	
	- Edit Table : 将在表里的数据返存回数据库，达成 Edit 的功能，基本和　SQL Studio 的 “编辑200行”的功能一样，只不过没有限制200。但是，记得不要不选全列就编辑哦，那样要丢数据的。
	
	- Execute Query : 执行Query框中的指令。Query框内的指令可以手工更改。
	
	- Hide Password : 显示/隐藏密码
	
	- Save Settings : 保存设置 (设置是明文保存，请谨慎使用)
	
记得配置MySQL 服务器上的设置哦：
	- CentOS6.7 iptables不太标准，发现打开网卡而不是地址才有效：-i ethx -p tcp --dport 3306 
	
为了赶工庆祝新年，没有汉化。大家都是代码亲，请多多见谅哦！


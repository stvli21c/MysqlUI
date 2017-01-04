# MysqlUI
新年快乐，各位爱写代码的亲！让我们用一个新的程序来庆祝新年吧！

当你在调试代码的时候，是不是常常想要反复检查数据库里的数据？这款不到 300KB 的小程序 MysqlUI 将将可以满足你的需求，又不用打开巨大的 SQL Studio　和 MySQL Workbench 之类的东东哦。目前已经可以同时支持SQL Server (Microsoft) 和 MySQL Server （Oracle）了，具有基本的增删改查功能，也可以手工输入查询命令。
程序需要安装MySQL Connector for .Net, 最低要求.Net4.0 Framework。 MySQL Connector for .Net 下载地址:
http://dev.mysql.com/downloads/connector/net/


界面简介:	
	
	'x' (Delete):   在顶部导航条的删除图标对光标选择了的行进行删除标记，之后再点保存，所有的删除生效。如果不保存，而是紧接着再查询，则所有未保存的删除操作被放弃。

	'💾'保存图标:  保存对数据表的删除、更改。注意：开始修改数据前一定要用 'select * from'　以保证其他列的数据不丢失！

	show 500 row：  查询结果行数限制，默认500行，可以选1000行，或无限制。

	Server:Port:  不填内容，程序使用默认的端口。

	Table Name:  使用 Microsoft SQL Server 时注意, 这个标签变为 <Schema.Table>, 在键入 Table 名时，请加 schema 前缀，默认的前缀是‘dbo.’ 。这样定制 schema 的 Table 也可以使用本程序了。

	Hide Password: 默认密码显示‘*’

	Save settings： 明文保存所有设置，包括密码。本程序为绿色程序，不用安装，没有通讯。但提醒您注意含密码文件的敏感性。

	查询框：　可以在该大框中手工编写查询语句，按<Execute Query>键即可执行此框内的语句。

	MySQL / SQL:　该下拉菜单设置查询服务器的种类: 微软的 SQL Server, 或者是甲骨文的 MySQL Server。

	Show Table：  执行 'Select * from table', 默认限制500行结果。由 <show 500 row> 下拉菜单设置。

	Save Table :  保存对数据表的更改。注意：开始修改数据前一定要用 'select * from'　以保证其他列的数据不丢失！修改和删除数据需要用到 Primary Key (PK)来定位，如果表中没有 ，请创建 PK，或者手工编写修改删除命令。

	Execute Query : 执行查询框内的语句。
		
	
记得配置MySQL 服务器上的设置哦：
	- CentOS6.7 iptables不太标准，发现打开网卡而不是地址才有效：-i ethx -p tcp --dport 3306 
	
为了赶工庆祝新年，没有汉化。大家都是代码亲，请多多见谅哦！


# vimNote
## day15

* /< CR >

	正向跳转到上一个搜索内容的下一处匹配;
* ?< CR >
	
	反向跳转到上一个搜索内容的上一处匹配;
* /或?< up >

	浏览之前的查找记录;
* 高亮设置

| 命令 | 描述 |
| ---- | ---- |
| :set hls[earch] | 打开搜索高亮 |
| :set nohls[earch] | 禁用搜索高亮 |
| :noh | 本次禁用搜索高亮 |

* :set incsearch

	设置搜索增量查询功能;

	设置后,执行搜索前可以预览第一处匹配;

	当找到了预览词汇,可以< C-r >< C-w >将预览的词汇补全到搜索输入中;

* /pattern/e< CR >

	将搜索后光标移动到最后一个字符,?同样适用;

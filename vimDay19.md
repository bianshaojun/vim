# vimNote

## day19
* :make命令

	在vim中可以使用make命令,直接编译文件;

	确保当前所在Makefile文件的目录下;

	执行完毕,输出的信息,将保存于quickfix列表中;

	回车后,将跳转到第一个quickfix列表中错误位置,不想跳转到错误位置使用:make!;

* 浏览Quickfix列表的命令

| 命令 | 用途 |
| ---- | ---- |
| :cnext | 跳转到下一项 |
| :cprev | 跳转到上一项 |
| :cfirst | 跳转到第一项 |
| :clast | 跳转到最后一项 |
| :cnfile | 跳转到下一个文件的第一项 |
| :cpfile | 跳转到上一个文件的最后一项 |
| :cc N | 跳转到第N项 |
| :copen | 打开quickfix列表 |
| :cclose | 关闭quickfix列表 |
| :colder | 回退上一个quickfix列表 |
| :cnewer | 前进下一个quickfix列表 |



	以上命令c换成l,将变成位置列表;
	
	quickfix列表是全局的;

	位置列表是当前窗口下的,可以每个窗口一个;

	在quickfix列表中时,可以直接在列表中回车跳转到相应位置;

* 定制外部编译器

	暂时没用,先不关注;

* vim filename +No 

	打开文件时,可以+No,直接跳转到指定行号;

* :grep

	在vim中,执行grep命令会调用外部grep程序;
	
	会自动加入-n参数(-n 指示grep输出加入行号信息);

	-i参数,不区分大小写;

	执行完,输出就在quickfix列表里;
* :vim[grep][!] /{pattern}/[g][j] {file} ...

	使用vim内部的grep命令,可以使用vim自带的正则表达式;

	g标志位为每处匹配创建一条记录;

	j标志位,让其只更新quickfix列表,不调到第一处匹配;

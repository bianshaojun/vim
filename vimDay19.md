## vim note

### day19
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

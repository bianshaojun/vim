# vimNote
## day18

* 安装ctags

	sudo apt-get install exuberant-ctags
* 生成tags文件

	在shell中:

	ctags filename,根据指定文件名在当前目录下生成tags文件;

	ctags -R,在当前目录下,递归子目录生成tags文件;

	在vim中:

	:!ctags filename or :!ctags -R, 生成tags文件,其实跟shell中一样,利用!来执行shell命令;

* 设置快捷键F5

	:nnoremap < F5 > :!ctags -R< CR >;
	
	利用快捷键在vim中按F5更新tags文件;
* 保存文件时,自动更新tags文件

	:autocmd BufWritePost * call system("ctags -R");

* ctags浏览命令

| 命令 | 描述 |
| ---- | ---- |
| < C-] > | 跳转到匹配当前光标下关键字的第一处标签 |
| g< C-] > | 如果有多个标签匹配当前光标下的关键字,提示用户指定一处进行跳转,如果只有一处,则直接跳转 |
| :tag {keyword} | 跳转到匹配keyword的第一处标签 |
| :tjump {keyword} | 如果有多个标签匹配keyword,提示用户指定一处进行跳转,如果只有一处,则直接跳转 |
| :pop 或 < C-t > | 反向遍历标签历史 |
| :tag | 正向遍历标签历史 |
| :tnext | 跳转到下一处匹配的标签 |
| :tprev | 跳转到上一处匹配的标签 | 
| :tfirst | 跳转到第一处匹配的标签 | 
| :tlast | 跳转到最后一处匹配的标签 |
| :tselect | 提示用户总标签匹配列表中选择一处进行跳转 |

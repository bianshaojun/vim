# vimNote
## day17

* :[range]global[!]/{pattern}/[cmd]

	默认情况下,global作用范围是整个文件,相当于[range]为%;

	{pattern}与查找历史相互关联,不填则表示重用上一次查找匹配;

	[cmd]默认使用print;

	global!或vglobal表示在没有被匹配的行上执行cmd;

* :g/re/d命令

	删除匹配re的所有行;

* :v/re/d命令

	只保留匹配re的行,删除其他的行;
* :g/re/y X命令

	复制匹配re的所有行,到寄存器X中(X寄存器名为大写,使用前用qxq命令将寄存器清空);

* :global/{start}/ .,{finish} [cmd]命令

	对从start到finish结束的所有行执行[cmd];


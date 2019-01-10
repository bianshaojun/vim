# vimNote
## day6

* :[range]copy {address}命令

	在命令模式下，把指定范围内的行拷贝到｛address｝所指定的行之下，简写为:co或:t；
* :[range]move {address}命令

	在命令模式下，把指定范围内的行移动到｛address｝所指定的行之下，简写为:m;
* @:命令

	重复上一次ex命令；
* @@命令

	重复上一次@:命令；
* :[range]normal {commands}命令

	在命令模式下，对指定范围的每一行执行普通模式命令｛commands｝;
* < C-o >命令

	在普通模式下，跳转到上一条记录；
* < C-d >命令

	在命令模式下，显示补全列表；
* < Tab >命令
	
	在命令模式下，按照补全列表依次显示，反向显示< S-Tab >;
* :[range]join命令

	在命令模式下，连接指定范围内的行，简写:j;
* :[range]yank　[x]命令

	在命令模式下，复制指定范围内的行[到寄存器ｘ中],简写:y;
* :[range]delete [x]命令

	在命令模式下，删除指定范围内的行[到寄存器ｘ中],简写:ｄ;
* :[line]put [x]命令

	在命令模式下，在指定行后粘贴寄存去ｘ中的内容，简写为:pu;
* :[range]substitute/{pattern}/{string}/[flags]命令

	在命令模式下，把指定范围内出现的pattern替换成string，简写:s;
* :[range]globle/{pattern}/[cmd]命令

	在命令迷失下，把指定范围内的匹配pattern的所有行，在其上执行ｅｘ命令｛cmd｝;


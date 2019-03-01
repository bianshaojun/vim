# vimIDE

* 升级你的vim到8.0

	Ubuntu自带的vim版本,有些低,为了和相关插件配合兼容,先更新一下版本;

	```
	sudo add-apt-repository ppa:jonathonf/vim
	sudo apt update
	sudo apt install vim
	```

	卸载的话:

	```
	sudo apt remove vim
	sudo add-apt-repository --remove ppa:jonathonf/vim
	```

* 安装ctags

	```
	sudo apt-get install exuberant-ctags
	```

* 安装taglist插件

	注意: 在安装taglist插件前,需要先安装前面的ctags;

	这里直接使用Vundle插件管理来进行安装;

	* :PluginSearch taglist

		我这里显示了有两个插件: taglist-plus,taglist.vim

		索性都下载下来,后发现taglist-plus是基于taglist.vim扩展的,加了js等相关的东西,对我来说用处不大,暂时就不用了;

	* 光标移动到taglist.vim

		根据提示按i进行安装;

	* 安装完后,在.vimrc里面添加

		`Plugin 'taglist.vim'`

	* taglist帮助文档

		在vim中:`:help taglist.txt`

	* vim中使用`:Tlist`打开taglist

* 安装NERDTree

	一个浏览文件目录树的插件;

	该插件源码在github上:

	`https://github.com/scrooloose/nerdtree`

	这里也同样直接使用vundle来安装;

	打开.vimrc文件,添加下面一行:

	`Plugin 'scrooloose/nerdtree'`

	如果还需要配合git使用的话,还可以添加下面这个插件:

	`Plugin 'Xuyuanp/nerdtree-git-plugin'`

	然后打开任意vim,输入:

	`:PluginInstall`

	即可安装完毕!

	* NERDTree帮助文档
		
		在vim中:`:help NERDTree.txt`

	* vim中使用`:NERDTreeToggle`打开NERDTree

* 安装bufexplorer

	一个查看历史打开文件的插件;

	同样使用vundle安装插件

	* :PluginSearch bufexplorer


	* 光标移动到bufexplorer.zip

		根据提示按i进行安装;

	* 安装完后,在.vimrc里面添加

		`Plugin 'bufexplorer.zip'`

	* 帮助文档

		在vim中:`:help bufexplorer.txt`

	* vim中使用`:Bufexplorer`打开bufexplorer


* 安装winmanager

	用来管理多个插件窗口的插件;

	可以用其管理bufexplorer,taglist,NERDTree;

	同样使用vundle安装插件
	
	* :PluginSearch winmanager

	* 光标移动到winmanager

		根据提示按i进行安装;

	* 安装完后,在.vimrc里面添加

		`Plugin 'winmanager'`

	* 帮助文档

		在vim中:`:help winmanager`

	* vim中使用`:WMToggle`打开winmanager




<p align="center">
	<img 
		style="margin-bottom: -30px"
		align="center" 
		height="70" 
		src="http://img.labnol.org/images/2008/04/gif-animation.gif">
</p>
【1】部署方法</br>
sh start_vim.sh
</br>
</br>
【2】vim功能</br>
//-------------------------------【#】显示函数列表</br>
<F2> : TlistToggle               //显示函数列表</br>
		按<F2>将会在VIM的左边打开一个Taglist窗口，这个窗口里面包含了C文件里面的定义，如struct,typedef,全局变量,函数等。</br>
		使用'<'Ctrl>+h将光标移动到左边的窗口，上下选择tag按回车定位到tag的定义处。</br>
//-------------------------------【#】当前目录列表，方便打开文件</br>
<F3> : NERDTreeToggle            //当前目录列表，方便打开文件</br>
		按<F3>会在VIM的右边打开一个文件浏览器窗口。再按一下<F3>会关闭这个窗口。</br>
//-------------------------------【#】最近文件列表</br>
<F4> : MRU			//最近文件列表</br>
		按<F4>会打开一个MRU窗口，这个窗口里面记录了最近打开的文档，上下选择文件回车打开。如果没有你想打开的文件可以按"q"关闭窗口。</br>
<F5> : LookupFile</br>
		<F5>在VIM的上面打开文件查找窗口，</br>
<F6> : vimgrep</br>
		假设你想查找某个字符串在项目中出现的位置，你可以把光标放在这个字符串上，</br>
		按<F6>就会在VIM的最下面显示你想查找的字符串，此时你可以修改这个字符串，回车到下一步，此时会提示你要查找的文件范围，</br>
//-------------------------------【#】编译</br>
<F7> : gcc</br>
		直接按<F7>可以对打开的文件直接编译</br>
//-------------------------------【#】gdb调试</br>
<F8> : gdb</br>
		直接按<F8>可以直接进入gdb调试状态</br>
<F9> : Generate tags</br>
		在代码间跳来跳去。先按<F9>生成tag数据库。将会在项目的当前目录下生成tags文件。</br>
		此时将光标放在某个函数调用上，按<Ctrl>+]就会跳到函数的定义处，按<Ctrl>+o就会跳回来。</br>
<F10> : HLUDSync</br>
		按<F10>可以生成cscope的数据库文件cscope.out，再使用",sa"(:cs add cscope.out)添加数据库文件。</br>
		当下次启动VIM的时候就会自动加载当前目录下的cscope数据库文件。</br>
		在.vimrc里面定义了使用cscope的快捷键，比如将光标放在某个函数上使用命令",sc"就可以查看这个函数被哪些函数调用过，</br>
//--------------------------------【#】全屏显示</br>
<F11> :genfiletags.sh</br>
		<F11>是让终端全屏显示</br>
<F12>add cscope.out</br>
		在查找文件之前要生成文件数据库，</br>
		按<F12>将会在项目的当前目录下生成tags.filename文件，所以最好是在项目的根目录下按<F12>。再按<F5>就可以使用通配符查找文件了。</br>
		
		
		
//--------------------------------【#】添加函数注释等</br>
：Dox</br>
		添加函数注释</br>
//--------------------------------【#】	头文件和c文件切换</br>
：AV</br>
		垂直分屏显示头文件或者c文件	</br>
【其他功能】--</br>
1.输入main后按table键，自动生成main函数</br>
2.输入单词自动补全//注，本文档之前输入的单词自动补全</br>


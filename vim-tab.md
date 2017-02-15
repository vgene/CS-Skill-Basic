为了vim更好的支持python写代码,修改tab默认4个空格有两种设置方法：

1. vim /etc/vimrc  

1	set ts=4
2	set sw=4
2. vim /etc/vimrc 

1	set ts=4
2	set expandtab
3	set autoindent
推荐使用第二种，按tab键时产生的是4个空格，这种方式具有最好的兼容性。
 
在 Vim 中设置 Tab
 
缩进用 tab 制表符还是空格，这不是个问题，就像 python 用四个空格来缩进一样，这是要看个人喜好的。在 Vim 中可以很方便的根据不同的文件类型来设置使用 tab 制表符或者空格，还可以设置长度，非常灵活。

首先来看如何设定 tab 的宽度以及如何确定用 tab 制表符还是空格来表示一个缩进：

set tabstop=4
set softtabstop=4
set shiftwidth=4
set noexpandtab / expandtab
说明：

 

其中 tabstop 表示一个 tab 显示出来是多少个空格的长度，默认 8。

softtabstop 表示在编辑模式的时候按退格键的时候退回缩进的长度，当使用 expandtab 时特别有用。

shiftwidth 表示每一级缩进的长度，一般设置成跟 softtabstop 一样。

当设置成 expandtab 时，缩进用空格来表示，noexpandtab 则是用制表符表示一个缩进。

Stay 
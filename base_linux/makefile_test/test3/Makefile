#使用.PHONY表示targeta是个伪目标
.PHONY:targeta
#目标a，依赖于目标targetc和targetb
#目标要执行的shell命令 ls -lh，列出目录下的内容
targeta: targetc targetb
	ls -lh

#使用.PHONY表示targetb是个伪目标
.PHONY:targetb
#目标b，无依赖
#目标要执行的shell命令，使用touch创建test.txt文件
targetb:
	touch test.txt

#使用.PHONY表示targetc是个伪目标
.PHONY:targetc
#目标c，无依赖
#目标要执行的shell命令，pwd显示当前路径
targetc:
	pwd

#使用.PHONY表示targetd是个伪目标
.PHONY:targetd
#目标d，无依赖
#由于abc目标都不依赖于目标d，所以直接make时目标d不会被执行
#可以使用make targetd命令执行
targetd:
	rm -f test.txt
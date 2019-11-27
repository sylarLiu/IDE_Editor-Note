********************
一些小技巧和问题总结
********************

新建一个文件后，默认是\ ``plain text``\ , 没有语法高亮功能，如何设置语法高亮?
=============================================================================

	可以通过右下角的语法高亮选择区域选择希望设置的语法模式.

编写\ *reST*\ 文档时的字体对齐问题
==================================

	编写\ *reST*\ 文档, 使用了中文时, 表格在源文件中的显示可能会错乱:

		.. image:: _static/table_disorder.png


	解决方法: 使用等宽字体.

	``Preferences -> Settings``\ 或\ ``Preferences  -> Settings - Syntax Specific``\ 中做如下设置:

		..  code-block:: text
			:emphasize-lines: 2, 4

			{
				"font_face": "Ubuntu Mono Regular",
				// 字体大小务必设置为12
				"font_size": 12
			}

	这样, 表格和文字在源文件中就可以对齐了:

		.. image:: _static/table_align.png

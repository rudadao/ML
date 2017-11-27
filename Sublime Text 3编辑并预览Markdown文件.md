# 1 安装
下载[Sublime Text 3](http://www.sublimetext.com/3)并进行安装，注意勾选Add to explorer context menu，这样Sublime Text可以被添加到右键中，在右键单击文件时，可以直接使用Sublime Text打开。

# 2 安装Package Control（管理插件的插件）
- 按Ctrl + ` 打开console
- 粘贴[代码](https://packagecontrol.io/installation#st3)(见链接内容）到console并回车
- 下载完成之后重启Sublime Text 3
-如在Perferences->中看到package control这一项，则安装成功

# 3 用Package Control安装Markdown Preview插件
- 按Ctrl + Shift + P，调出控制面板
- 输入install 调出Install Package并回车
- 输入Markdown Preview，调出插件并回车

# 4 创建用Markdown语法编辑的文档
- 按Ctrl + N 新建一个文档
- 按Ctrl + Shift + P，调出控制面板
- 输入ssm (Set Syntax: Markdown)后回车

# 5 在浏览器预览Markdown文档
- 按Ctrl + Shift + P，调出控制面板
- 输入mp (Markdown Preview: current file in browser)后回车
- 此时就可以在浏览器里看到刚才编辑的文档了

# 6 额外配置
- 浏览器预览配置，即通过按alt + m预览编辑内容：
将preference--> key binding user 中输入
```
[
    {"keys": ["alt+m"], "command": "markdown_preview", "args": { "target": "browser"}}
]
```
- MathJax公式支持和语法高亮配置：
在preference--> Package Settings -> Markdown Preview -> Setting - User 中加入内容：
```
{
    
    /*
        Enable or not mathjax support.
    */
    "enable_mathjax": true,

    /*
        Enable or not highlight.js support for syntax highlighting.
    */
    "enable_highlight": true,


}
```
# 7 参考
- http://blog.csdn.net/Marksinoberg/article/details/50993456
- http://blog.csdn.net/orangleliu/article/details/34849723
- http://blog.csdn.net/kamidox/article/details/48380239

---
layout: post
title: 关于Emacs Buffer的积累
tags:
- Emacs
- Linux
- 编程
categories: 学习
---
平时用到的，从网上查来的教程，自己码的字。






* content
{:toc}
#### buffer列表（键入C-x C-b时显示在一窗口中）

Emacs会创建它自己的专用buffer。这些内部buffer的名字一般来说格式为 *buffer name* 。*Help*、*scratch*和*Buffer List*就是Emacs创建的其中一些buffer。

当你启动Emacs时，它会建立两个buffer：

\*Messages*
\*scratch*

\*Messages* buffer存储了Emacs收集自它启动时从minibuffer里显示的消息；*scratch*是个临时的scratchpad（涂鸦板），以便你有地方输入东西。除非你使用C-x C-w明确的把它写到文件中，否则它不会被保存下来。

当然，一般来说你用Emacs编辑文件时，这些文件就会被拷贝到同名的buffer中。如果你需要获得帮助，则会进入 *Help* buffer。

能在Emacs里打开的buffer数量实际上没有限制。大多数情况下，只显示一个或两个buffer；不过即使你无法看到全部，你在某个Emacs会话里 创建的buffer仍处于活动状态。你可以把这些buffer想象成一叠纸，只有放在最上面的那页才显示在你眼前。不过任何时候，你都可以翻到另一页（另 一个buffer），或者也可以创建一个新页。

每个buffer都关联一个主模式（major mode），它决定了Emacs在这个buffer里的行为。例如，设计用来书写文本的文本模式（text mode），和Lisp模式的表现就不一样，后者被设计用来编写Lisp程序。

#### 如何操作多个buffer

如果要新建包含一个文件的buffer，只需键入 C-x C-f 找到该文件。Emacs就会自动新建一个buffer并定位到该buffer。如果该文件已打开，C-x C-f 只是定位到已有buffer中，这一点很有意义，可以避免同一文件存在多个buffer导致混乱。如果键入 C-x C-f 后输入的文件名不存在，Emacs认为你想新建一个文件，并定位到一个空白buffer中。

C-x b：在多个buffer之间进行切换；键入命令后输入buffer名，回车。如果已存在该buffer，则切换到该buffer中；否则以输入的 buffer名新建一个buffer，但是注意这个buffer并没有和文件相关，因此关闭Emacs，它不会给你任何提示。

C-mouse 1：按住Ctrl并单击鼠标左键，会弹出一个Buffer Menu，它会按主模式类型列出活动的buffer供你选择。

C-x -\>(<-)：按下C-x后（放开）再按向右（左）方向键可以定位到下（上）一个buffer中。

我的习惯是： c-x  c-b 显示所有名字   c-x b 输入要切换的buffer名字。

#### 如何删除buffer

注意：如果你修改了一个buffer（且该buffer和一个文件相关），则Emacs会在删除buffer前询问你是否保存所做修改；如果这个 buffer和文件不相关，则你在该buffer里所做任何修改都会丢失，Emacs认为你不在乎这些buffer因此不作任何提示。因此编辑重要的 buffer之前最好先 C-x C-w 写到文件中，或者用 C-x C-f 新建buffer。

C-x k：kill-buffer命令，删除一个buffer；

M-x kill-some-buffers：删除一些buffer；

如果删除了当前会话里的所有buffer，Emacs会新建一个 *scratch* buffer，总得有个东西显示在屏幕上不是？:P

#### 如何保存buffer

C-x C-s：保存当前buffer；

C-x s：即save-some-buffers命令，一次保存所有buffer；

#### 如何重命名buffer

M-x rename-buffer：重命名buffer；

#### 如何使buffer只读

C-x C-q：切换buffer的read-only和read-write状态；

#### buffer和window的关系

buffer和window并不是一一对应的，同一个buffer可以有多个window，比如你可以同时在多个window里查看同一buffer的不同部分。Mark是和buffer关联的；而point是和window关联的。

C-x 2：即split-window-vertically命令，水平切分窗口；

C-x 3：垂直切分窗口；

C-x 4 b(f)：在另一个窗口选择另一个buffer（查找另一个文件），这样你可以不用切换到另一个window，就改变其buffer或打开文件；

C-M-v：滚动另一个window（C-v是滚动当前window）；

C-x o：此处 o 表示other（其它），移动光标到另一个window；

C-x 0：删除当前所在的window；

C-x 1：删除当前所在window之外的所有window；

C-x 5 2：新建一个frame；  

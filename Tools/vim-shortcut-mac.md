# MacBook 快捷键

## terminal 快捷键
### 命令行shell快捷键
vim

### vim 编辑器快捷键

#### 命令模式
```
:sp ~/.vimrc 垂直分屏，ctrl+w n > 当前分屏增宽n列，ctrl+w n < 当前分屏减宽n列，ctrl+w c 关闭当前分屏
:vs ~/.vimrc 水平分屏
:Ve 左右分屏，在左面浏览目录，Ve!在右面浏览目录
:r filename 读取文件并插入到当前文件中
:r !ls 读取命令到当前文件的当前行
:w filename 当前文件另存为
:bp 移到上一个文件
:bn 移到下一个文件

```

#### 普通模式
``` 滚动
ctrl+e 向下滚动一行，当前行为n，将当前行当为第一行需要n-1 ctrl+e
ctrl+y 向上滚动一行

ctrl+d 向下滚动半屏
ctrl+u 向上滚动半屏

ctrl+f 向下滚动一屏
ctrl+b 向上滚动一屏
```

```  撤销
u 撤销
ctrl+r 撤销刚才的撤销
```

``` 删除
x <==> dl 删除当前字符
X <==> dh 删除当前字符的前一个字符，删除中文字符很管用，删除当前字符和前一个字符可以xX
D <==> d$ 删除当前字符到行尾

cl 删除当前字符并进入插入模式
ch 删除前一个字符并进入插入模式
cc 删除当前行并进入插入模式，ncc 删除n行并进入插入模式

dk 删除上一行，删除上n行，dnk
dj 删除下一行，删除下n行，dnj

1,10d 删除1-10行，10可以换成$代表删除1-行尾；+1,+10 d删除当前行的下1行到下10行
```

``` 移动
2j 向下移动2行
+1,+10 co -7 将当前行的下一行到第10行移动到当前行的上第7行，. 代表当前行
+1,+10 m -7 将当前行的下一行到第10行移动到当前行的上第7行
```

```复制
								      3yy => y2j
```

``` 文件保存
:e! 放弃所有修改，并打开原文件，也就是打开:w的文件
```

``` 排版
:ce 本行文字居中排列
:le 本行文字靠左排列
:ri 本行文字靠右排列
>> <==> ctrl+> 行缩进向右移动一个单位
<< <==> ctrl+< 行缩进向左移动一个单位
```

``` esc
esc <==> ctrl+[
```

``` 宏，记录键盘操作，重复使用，但只有在普通模式下才生效
qx 开始录制宏x
q 结束录制
@x 使用宏x
```

``` 折叠，可以用于注释加上所注释的代码块
zf n j 向下折叠n行
zo 打开折叠文本 zO 打开所有折叠
zc 关闭折叠 zC 关闭所有折叠
za 打开/关闭当前折叠
zj 跳到下一个折叠
zk 跳到上一个折叠
zd 删除折叠 zD 删除所有折叠
```
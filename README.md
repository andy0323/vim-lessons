# vim-lessons

vim 操作学习总结

## 操作模式

vim的操作简单分为以下几个模式

1. 默认模式
2. 输入模式
3. 选择模式
4. 命令模式

### 如何进入vim窗口

1. 打开终端
2. `vim hello.txt`

### 如何判断当前状态是哪个模式

判断**vim**左下角的提示信息，可以判断当前的模式状态。

| 操作模式 | 提示信息         | 如何进入该模式|
|---------|----------------|-------------------------|
| 默认模式 | 空白                | ESC                     |
| 输入模式 | `-- INSERT --`     | 默认模式下，输入`a`或者`i`  |
| 选择模式 | `-- VISUAL --`     | 默认模式下，输入`v`        |
| 命令模式 | `:${CMD + PARAMS}` | 默认模式下，输入`:`，跟上命令参数 |

### 这几个模式都是做什么的？

#### 默认模式

在默认模式下，可以进行一些快速操作、以及进入命令模式进行一些命令操作

#### 输入模式

在输入模式下，可以进行内容的编辑，输入你想要添加的内容。

#### 选择模式

在选择模式下，可以进行多行选择，然后`command+c`、`command+v`进行复制黏贴等操作。

#### 命令模式

在命令模式下，可以用不同的命令完成复杂的文件操作、编辑操作。

## 默认模式的快捷方式

| 按键组合  | 功能介绍                   |
|----------|--------------------------|
| `v`              | 进入可视区域       |
| `a`或`i`         | 进入编辑区域        |
| `o`              | 光标后方进行插入    |
| `h`,`j`,`k`,`l`  | 移动光标           |
| `y`              | 复制选中内容        |
| `yy`             | 复制整行           |
| `y`              | 光标后粘贴         |
| `dd`             | 删除整行           |

## 命令模式的命令介绍

| 按键组合  | 功能介绍                   |
|----------|--------------------------|
| `:cd 目录路径`             | 修改当前操作目录                         |
| `:new 文件名.后缀`          | 新建后需要通过，`:w`进行保存生成           |
| `:e 文件名`                | 打开一个文件                             |
| `:split 文件`              | 会将当前窗体分为多个区域，在新的区域打开文件。| 
| `:tabnew`                 | 这将在新的分页中打开文件                   |
| `control + w`             | 通过`:split`分割的文件间的切换             |
| `:ls`                     | 查看`:split`分割文件的文件列表             |
| `:e# + 编号`              | 进入编号对应的文件，编号为`:ls`列表的左测数字  |
| `:f 文件名`                | 修改当前文件的名称                        |
| `:w`                      | 保存文件                                 |
| `:q`                      | 退出文件                                 |
| `:q!`                     | 不进行保存，强制退出文件                    |
| `:x`                      | 退出，如果文件更改则保存                    |

## 参考内容

[Windows上使用VIM入门之文件操作](http://blog.csdn.net/shenjie12345678/article/details/43228159)

###（后续内容、会进行更新补充、更正）

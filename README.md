# Sublime-Text-Theme
#### 定制属于自己的个性化主题
这里有两个概念，Theme 和 Color Scheme，Theme 指的是主题， 而 Color Scheme 指的是主题配色方案。
#### 如何获取 Theme
[Material Theme](http://equinsuocha.io/material-theme/#/default) 个人比较喜欢这款主题，简洁漂亮，下面是它的截图。当然你也可以从[这里](https://packagecontrol.io/browse/labels/theme) 找到其他的主题。

<img src="https://github.com/emanci/SublimeText3-Theme/blob/master/material-theme.png" width = "450" alt="material-theme" align=center />

#### 如何获取 Color Scheme
实际上，我们下载的主题包中就包含了 Color Scheme，但是我们有其他的选择，我们可以从[这个网址](http://tmtheme-editor.herokuapp.com)获取自己喜欢的主题，当然也可以在这个网站按照自己的意愿制作喜欢的主题。制作完毕之后将生成的 xxx.tmTheme 文件添加到 sublime text 的 Packages 文件夹中(Preferences -> Browsr Packages)。
#### 如何配置主题和配色方案
一、首先，安装 Material Theme
1. Press ⌘/Ctrl + ⇧ + P to open the command palette.
2. Type `Package Control: Install Package` and press enter. Then search for `Material Theme`.

二、添加新的配色文件
这里我以 Primer Dark 这个主题为例，在配置主题之前
首先我将 Primer - Light.tmTheme 主题文件添加到 Packages 中。为方便管理，我将该文件放在了新建的 CustomColorScheme 文件夹下。

三、配置
主题和配色安装完后，我们在 Material Theme 主题下，选择刚刚新添加的 Color Scheme 了，但是仅仅是主面板的颜色改变了，左侧菜单栏和面板头部的颜色还没修改。这个时候我们就需要 PackageResourceViewer 这个工具了，他的安装方式同其他插件一样，在 Package Control 中即可安装。
PackageResourceViewer 安装完毕后，在命令面板中输入：PackageResourceViewer:Open Resource 
然后会列出配置文件目录。然后，我们选择 Material Theme 这个选项。这个时候，在 Packages 文件夹下会多出一个新的文件夹，那就是 Material Theme。接下来，我们的配置就在这个文件夹下来完成。
编辑 Material Theme 文件夹下的 Material-Theme.tmTheme 文件，然后我们获取主面板的颜色 RGB, 用来配置菜单栏和其他位置的颜色，保持一致，我们的修改项如下：
- sheet_container_control 
- title_bar 
- dialog
- progress_bar_control
- popup_control
- auto_complete
- mini_quick_panel_row
- quick_panel
- quick_panel_row
- tabset_control
- tab_control
- sidebar_container
- sidebar_tree
- tree_row
- scroll_bar_control
- status_bar
- status_button
- panel_control
- button_control
- icon_button_control

整个配置完成后，效果如下

<img src="https://github.com/emanci/SublimeText3-Theme/blob/master/primer-dark.png" width = "500" alt="primer-dark" align=center />

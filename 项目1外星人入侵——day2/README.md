## 任务介绍

现在来开始开发游戏《外星人入侵》。首先创建一个空的Pygame窗口，供后面用来绘制游戏元素，如飞船和外星人。我们还将让这个游戏响应用户输入，设置背景色以及加载飞船图像。
此时我们创建了两个文件：
- alien_invasion.py 创建一个空的pygame窗口
- settings.py 关于游戏的所有设置
- 运行 alien_invasion.py文件即可

## 代码解析

- 模块sys用来退出游戏

- pygame.init()作用是初始化背景设置，让Pygame能够正确工作

- pygame.display.set_mode()用来创建一个名为screen的显示窗口，这个游戏的所有图形元素都将在其中绘制。

- pygame.event.get()用来访问Pygame检测到的事件。所有键盘和鼠标事件都将促使for循环运行。

- sys.exit()用来退出游戏

- screen.fill()，用背景色填充屏幕；这个方法只接受一个实参：一种颜色

- pygame.display.flip(),命令Pygame让最近绘制的屏幕可见。每次执行while循环时都绘制一个空屏幕，并擦去旧屏幕，使得只有新屏幕可见。在我们移动游戏元素时，pygame.display.flip()将不断更新屏幕，以显示元素的新位置，并在原来的位置隐藏元素。从而营造移动的效果。

- 文件 settings.py为一个模块，其中包含一个名为Settings的类，用于将所有设置存储在一个地方，以免在代码中到处添加设置。
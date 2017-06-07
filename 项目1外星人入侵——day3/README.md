## 任务介绍
为了在屏幕上绘制玩家的飞船，我们将加载一幅图像，再使用Pygame方法blit()绘制它。
今天，我们创建一个新文件ship.py 并修改了 alien_invasion.py文件，只对其增加了代码

## 代码解析

- pygame.image.load()用来加载图像，这个函数返回一个表示飞船的surface

- get_rect()获取相应surface的属性rect

- 要让游戏元素剧中，可设置相应rect对象的属性center，centerx或centery。要让游戏元素与屏幕边缘对齐，可以使用属性top,bottom,left或right;要调整元素的水平或垂直位置，可以使用属性x和y,它们分别是相应矩形左上角的x和y坐标。
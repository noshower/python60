## 任务介绍
下面添加射击功能。我们将编写玩家按空格键时发射子弹（小矩形）的代码。子弹将在屏幕中向上穿行，抵达屏幕上边缘后消失。
我们更新了settings.py文件，加入了子弹的相关数据

## 代码解析

- from pygame.sprite import Sprite 从模块pygame.sprite中导入Sprite类。通过使用精灵，可以将游戏中相关的元素编组，进而同时操作编组中的所有元素。

- super().__init__()继承Sprite

- pygame.Rect()类用来从空白开始创建一个矩形。创建这个类的实例时，必须提供矩形左上角的x坐标和y坐标,还有矩形的宽度和高度。

- pygame.draw.rect()绘制子弹

- from pygame.sprite import Group  导入Group类，编组类似于列表，但是提供了有助于开发游戏的额外功能

- bullets.update() 当你对编组调用update()时，编组将自动对其中的每个精灵调用update()

- bullets.copy() 使用方法copy()来生成一个副本

- self.bullets_allowed =3 将子弹的数量限制为3颗
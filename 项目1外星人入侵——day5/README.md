## 任务介绍
让玩家能够左右移动飞船。

这次我们修改了所有文件。

## 代码解析
- pygame.event.get()能够帮助我们获取事件
- pygame.KEYDOWN 按下键盘事件
- pygame.KEYUP 松开键盘事件
- pygame.K_RIGHT 键盘上的右箭头键
- pygame.K_LEFT 键盘上的左箭头键
- event.key 被操作的键
- ship.rect.centerx 飞船中心的x坐标(左右移动就是操作这个值)
- self.moving_left,self.moving_right 如果值为True，表示可以调整位置
- Settings类中的属性 ship_speed_factor,用来控制飞船的速度
- float()函数将self.rect.centerx的值转换为小数
- self.rect.right的值，返回飞船外接矩形的右边缘的x坐标
- self.screen_rect.right的值，返回屏幕右边缘的x坐标

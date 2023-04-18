# LV_Pong Game

A classic Pong game dose not render in 2D picture control, that everything presented by LabVIEW intrinsic controls.

Other features:
*Some brick could not be destoryed by one hit.
*Can creat more customized level by modify setting.txt file.
*Earn extra ball when reaching specific score, hit more bricks before ball return the paddle.
*Use "Ctrl + Shift + C" to go to next level immediately.


![image](https://github.com/KurtDing/LabVIEW_Pong/blob/d17a218d8bcc1ab2a1733f6c3bb75b91b96ce028/pong3.png)


To create the new level, open the setting.txt
The content looks like figgure below, 
Level infomation starts form ":=" and ends at "//"
Between these is a 6 by 6 array of numbers separated by coma. 
The first row is the most buttom 6 bricks.
The number means the hit point of brick, maximun hp is 6.
If hp of brick set to 0, then it wont exist in the level.

![image](https://github.com/KurtDing/LabVIEW_Pong/blob/44a9f73565b8b75f3e2dd72489976b1cf4d1f031/pong2.png)


TODO()
The perfomance of game is awful. /n
Mybe one of the root cause is using simple AABB collision detection. /n
It can add a broad phase algorim before do collision detection. /n
Like uniform Grid, that looks like blockmap in doom engine. /n
Or do sweep and prune to decrease the possible collide object.


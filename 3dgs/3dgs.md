# 3dgs

# 学习资源

## 讲人话-3d gaussian splatting全解系列

https://www.bilibili.com/video/BV1zi421v7Dr/

code: https://github.com/SY-007-Research/3dgs_render_python

### 1 捏雪球



![image-20240803215623037](/home/mrwang/.config/Typora/typora-user-images/image-20240803215623037.png)

![image-20240803220355712](/home/mrwang/.config/Typora/typora-user-images/image-20240803220355712.png)

![image-20240803220532769](/home/mrwang/.config/Typora/typora-user-images/image-20240803220532769.png)



### 2 抛雪球

观测变换： 世界坐标系->相机坐标系

投影变换：3D空间->2D空间

视口变换：

光栅化：

![image-20240806215717650](/home/mrwang/.config/Typora/typora-user-images/image-20240806215717650.png)



#### 观测变换

![image-20240806215801429](/home/mrwang/.config/Typora/typora-user-images/image-20240806215801429.png)







#### 投影变换

投影变换：正交投影与透视投影

正交投影：与深度无关，没有远小近大的现象，速度快

透视投影：



![image-20240806220211235](/home/mrwang/.config/Typora/typora-user-images/image-20240806220211235.png)







![image-20240806220531531](/home/mrwang/.config/Typora/typora-user-images/image-20240806220531531.png)

#### 视口变换

![](/home/mrwang/.config/Typora/typora-user-images/image-20240806220722517.png)

#### 光栅化

![image-20240806220910410](/home/mrwang/.config/Typora/typora-user-images/image-20240806220910410.png)

![image-20240806221100836](/home/mrwang/.config/Typora/typora-user-images/image-20240806221100836.png)

#### 3dgs的观测变换

![image-20240806221444251](/home/mrwang/.config/Typora/typora-user-images/image-20240806221444251.png)

#### 3dgs的投影变换

![image-20240806221602134](/home/mrwang/.config/Typora/typora-user-images/image-20240806221602134.png)

##### 雅可比矩阵

![image-20240807000558331](/home/mrwang/.config/Typora/typora-user-images/image-20240807000558331.png)

![image-20240807000734819](/home/mrwang/.config/Typora/typora-user-images/image-20240807000734819.png)



 协方差矩阵没有缩放平移，不需要做视口变换（本身就在正交变换后的空间中，不需要视口变换拉回正常比例）

![image-20240807000822832](/home/mrwang/.config/Typora/typora-user-images/image-20240807000822832.png)

![image-20240807001129650](/home/mrwang/.config/Typora/typora-user-images/image-20240807001129650.png)



![image-20240807001220918](/home/mrwang/.config/Typora/typora-user-images/image-20240807001220918.png)



![image-20240807001330846](/home/mrwang/.config/Typora/typora-user-images/image-20240807001330846.png)

![image-20240807002057440](/home/mrwang/.config/Typora/typora-user-images/image-20240807002057440.png)



![image-20240807001954932](/home/mrwang/.config/Typora/typora-user-images/image-20240807001954932.png)



### 3 雪球颜色

![image-20240807002332135](/home/mrwang/.config/Typora/typora-user-images/image-20240807002332135.png)

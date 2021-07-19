---
layout:     post
title:      turtle库的使用
subtitle:   关于turtle库的学习笔记
date:       2021-07-19
author:     tmy
header-img: img/the-first.png
catalog:   true
tags:
    - python的打怪之旅
---
# 很有意思的海龟库的使用
## 关于turtle库的学习笔记
这一知识点的学习笔记的内容我分为8个部分  
一、turtle的绘图窗体  
turtle.setup(width,height,startx,starty)这个函数用来设置窗体大小及位置，在这个函数中的四个参数可选后两个，如果不输入具体数值默认窗体在电脑屏幕的中间。setup函数在turtle库的使用中不是必须的。  
二、绝对坐标和海龟坐标  
绝对坐标其实就是我们数学中学习的直角坐标系，海龟就是原点，x，y轴为正方向。
turtle.goto（a，b）这个函数的意思就是海龟从原点爬行到坐标（a，b）这个点，即goto从哪到哪
这个图更可以帮你理解，如果没看到图就是我这个菜鸡还没学会如何插入图片，请耐心等待hhh
海龟坐标更简单其实就是去掉直角坐标系中的xy轴在这样一个平面内运动
turtle.forward(d)或turtle.fd(d) 海龟向前行进且走直线，其中d为海龟走的距离，d也可为负值表示向后直线行进。
turtle.bk(d)是海龟向后直线行进。turtle.circle(r,angle)是海龟默认以左距离r的点为圆心，走angle角度的曲线行进，这里的角度为绝对角度。  
 三、绝对角度和海龟角度   
绝对坐标其实就是数学中学习的极坐标，区别是这里的角度为绝对角度，不采用弧度制，顺时针角度为负逆时针角度为正，范围0到360度即一周。
turtle.setheading(angle)或turtle.seth(angle)即改变海龟的方向，需注意只改变方向并不行进。
海龟角度turtle.left(angle)和turtle.right(angle)这个so easy    
四、RGB色彩   
这个贴两张图，如果没看到图就是我这个菜鸡还没学会如何插入图片，请耐心等待hhh  
五、库引用（扩充python程序功能的方式）  
使用import保留字完成，采用<a>.<b>()编码风格   
import<库名>   
<库名>.<函数名>(<函数参数>)   
import更多用法：使用import和as保留字共同完成，import<库名> as<库别名><库别名>.<函数名>(<函数参数>)。库别名是给调用的外部库关联一个更短、更适合自己的名字（可以称之为小名）    
六、画笔控制函数  
turtle.penup()或turtle.pu()抬起画笔，海龟飞行 turtle.pendown()或turtle.pd()落下画笔，海龟爬行
turtle.pensize(width)或turtle.width(width)画笔宽带 turtle.pencolor(color)画笔颜色  
color参数可以有三种形式：颜色字符串（需注意字符串要用双引号""），RGB的小数值，RGB的元组值  
七、按照一定次数循环执行一组语句    
for<变量> in range (<参数>)   
<被循环执行的语句>   
<变量>表示每次循环的计数，0到<次数>-1   
这个栗子可以帮助理解，如果没看到图就是我这个菜鸡还没学会如何插入图片，请耐心等待hhh   
八、range ( )函数产生循环计数序列  
range(5)   
0，1，2，3，4    
-range ( N )   
range(2，5)    
产生О到N-1的整数序列，共N个   
2，3，4   
-range ( M，N)   
产生M到N-1的整数序列，共N-M个   
    
结束啦感谢大家支持我的blog。^_^









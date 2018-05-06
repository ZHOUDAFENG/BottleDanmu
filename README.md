# BottleDanmu
bottledm.js，一个简单的，咸鱼写的弹幕JS

## DEMO：<http://x.imbottle.com/bottledanmu.html>
 
--------------------------------------
### 调用方法：
1. 引用bottledm.js.
2. 在html文档里面新建一个div层，并给予id，样式里最好定义一下其长宽.
- 你需要弹幕出现的图片，视频等都放在这个div层内
3. 在<script>标签下使用 ** createdm(元素id,弹幕内容,弹幕颜色,弹幕速度/时间,弹幕类型); ** 来创建弹幕.

-----------------------------
### 小贴士：
* 弹幕速度/时间在不同弹幕类型下有不同作用。在**顶部**和**底部**弹幕，以**秒**为单位，为其停留时间.在普通滚动弹幕里面为**控制其速度**.
- 速度范围建议为**0.5-10**，且无论是什么弹幕，都可以用auto来代替.（默认滚动速度取决于**字数**，默认停留时间是5秒）
- 弹幕类型为
1. bottom - 底端弹幕
2. top - 顶端弹幕
3. normal - 滚动弹幕
#### 下面是例子：
```
createdm('main','真的吗？我真的好高兴啊！','green','auto','normal'); //自动时间且绿色的滚动弹幕
createdm('main','真的吗？我真的好高兴啊！','green','auto','bottom'); //停留五秒的底端弹幕
createdm('main','真的吗？我真的好高兴啊！','green',1,'top'); //停留一秒的顶端弹幕
 
```
### 暂停所有弹幕？
```
theworld();//暂停全屏弹幕
continuedm();//继续全屏弹幕
```

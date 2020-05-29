# slam_bot
SLAM mapping and navigation simulation project

 In this SLAM Mapping and Navigation Simulation Project, there are three main parts, which are
 - Construction of models and environments
 - Location and navigation based on known maps
 - Map building and navigation using RTAB-MAP
 
 The **slam_bot_initial** folder provides the initial slam_bot package,if you want to build package by yourself,this is good choice!




## Launch
```
$ cd ~/catkin_ws/src
$ git clone https://github.com/Xiangyu-Fu/slam_bot.git
$ cd ..
$ source devel/setup.bash
$ ./src/slam_bot/launch/rtab_run
```

---

Here are the final project effects!

![map](https://img-blog.csdnimg.cn/20200529003017489.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM3MjY2OTE3,size_16,color_FFFFFF,t_70)


![](https://img-blog.csdnimg.cn/20200529075334133.gif)

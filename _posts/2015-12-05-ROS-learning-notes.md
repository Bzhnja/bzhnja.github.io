---
layout: post
title: ROS Learning Notes
categories: 
  - ROS
tags:
  - ubuntu
  - wiki.ros.org
comments: true
---
# 1. 创建ROS工作区 #

    $ mkdir -p ~/catkin_ws/src
    $ cd ~/catkin_ws/src
    $ catkin_init_workspace

注意： 是在src文件夹中执行`catkin_init_workspace`

    $ cd ~/catkin_ws/
    $ catkin_make

注意： 是在工作区根目录中执行`catkin_make`


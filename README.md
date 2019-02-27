## 下载和编译

1. 克隆或下载到工作空间的`/src`目录下
```sh
$ cd ~/catkin_ws/src
$ git clone https://github.com/linjiaqin12138/nav_sim.git
```
2. 编译并刷新环境
```sh
$ catkin_make
$ source ~/catkin_ws/devel/setup.bash
```

---
## 运行须知

1. 建议在**本地Ubuntu 16.04**下运行仿真程序。目前Gazebo模拟器的**兼容性**是一大问题，在虚拟机或配置较低的电脑上可能无法运行。**如果你的显卡是N卡，建议安装Ubuntu下的显卡驱动**。

2. 运行Gazebo仿真程序`robot_sim_demo`前，请将Gazebo升级到7.x版本以上（**推荐7.9版本**）。

  查看Gazebo版本方法
  ```sh
  $ gazebo -v   #确认7.0以上，推荐7.9
  ```

  升级方法

  ```sh
  $ sudo sh -c 'echo "deb http://packages.osrfoundation.org/gazebo/ubuntu-stable `lsb_release -cs` main" > /etc/apt/sources.list.d/gazebo-stable.list'
  $ wget http://packages.osrfoundation.org/gazebo.key -O - | sudo apt-key add -
  $ sudo apt-get update
  $ sudo apt-get install gazebo7
  ```

3. 确保所有依赖都已安装，如navigation


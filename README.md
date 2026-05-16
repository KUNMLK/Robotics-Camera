# 📷 机器人与具身智能相机入门指南

## 🌟 什么是机器人视觉？

机器人通过相机"看"世界，就像人类用眼睛感知环境。不同相机适合不同任务，本指南帮你快速入门。

---

## 📚 目录

1. [单目相机](#1-单目相机-monocular-camera)
2. [双目相机](#2-双目相机-stereo-camera)
3. [RGB-D相机](#3-rgb-d相机)
4. [ToF相机](#4-tof相机)
5. [事件相机](#5-事件相机)
6. [鱼眼相机](#6-鱼眼相机)
7. [热成像相机](#7-热成像相机)
8. [实用工具与资源](#8-实用工具与资源)

---

## 1. 单目相机 (Monocular Camera)

**最简单的相机**，一个镜头，像人的一只眼睛。

### 核心特点
- **优点**：便宜、体积小、易上手
- **缺点**：无法直接测距离

### 常见用途
- 人脸识别
- 二维码扫描
- 颜色识别
- 简单跟踪

### 入门资源
- **Intel RealSense SDK**：[github.com/IntelRealSense/librealsense](https://github.com/IntelRealSense/librealsense)
- **OpenCV入门**：[github.com/opencv/opencv](https://github.com/opencv/opencv)
- **推荐学习**：[从零开始学习单目视觉](https://github.com/uoip/monocular-vision-tutorial)

---

## 2. 双目相机 (Stereo Camera)

**两个镜头**，像人的双眼，通过视差计算距离。

### 核心特点
- **优点**：被动成像，室外效果好
- **缺点**：计算量大，对纹理要求高

### 常见用途
- 三维重建
- SLAM导航
- 避障

### 入门资源
- **ZED SDK**：[github.com/stereolabs/zed-sdk](https://github.com/stereolabs/zed-sdk)
- **OpenCV双目教程**：[docs.opencv.org/4.x/dd/d53/tutorial_py_depthmap.html](https://docs.opencv.org/4.x/dd/d53/tutorial_py_depthmap.html)
- **经典项目**：[github.com/uzh-rpg/rpg_svo](https://github.com/uzh-rpg/rpg_svo)（半直接法SLAM）

---

## 3. RGB-D相机

**彩色+深度**一体，同时提供颜色和距离信息。

### 核心特点
- **优点**：开箱即用，深度精度高
- **缺点**：室外阳光影响大

### 常见用途
- 手势识别
- 物体抓取
- 室内建图

### 入门资源
- **Intel RealSense**：[github.com/IntelRealSense](https://github.com/IntelRealSense)
- **Azure Kinect SDK**：[github.com/microsoft/Azure-Kinect-Sensor-SDK](https://github.com/microsoft/Azure-Kinect-Sensor-SDK)
- **ROS集成**：[wiki.ros.org/realsense2_camera](https://wiki.ros.org/realsense2_camera)

---

## 4. ToF相机

**飞行时间相机**，通过光的往返时间计算距离。

### 核心特点
- **优点**：帧率高，工作距离远
- **缺点**：分辨率较低

### 常见用途
- 人体姿态估计
- 人流量统计
- 室内导航

### 入门资源
- **PMD技术文档**：[pmdtec.com](https://www.pmdtec.com/)
- **ToF深度估计**：[github.com/facebookresearch/pytorch3d](https://github.com/facebookresearch/pytorch3d)
- **TI参考设计**：[ti.com/product/OPT8320](https://www.ti.com/product/OPT8320)

---

## 5. 事件相机

**异步相机**，只记录亮度变化，不拍完整图像。

### 核心特点
- **优点**：延迟极低（<1us），高动态范围
- **缺点**：数据处理复杂

### 常见用途
- 高速运动跟踪
- 无人机避障
- 低延迟控制

### 入门资源
- **Prophesee SDK**：[github.com/prophesee-ai](https://github.com/prophesee-ai)
- **事件视觉入门**：[github.com/uzh-rpg/event-based_vision_resources](https://github.com/uzh-rpg/event-based_vision_resources)
- **经典论文**：[Event-Based Vision: A Survey](https://arxiv.org/abs/1904.08405)

---

## 6. 鱼眼相机

**超广角镜头**，视野超过180度。

### 核心特点
- **优点**：视野广，减少盲区
- **缺点**：图像畸变严重

### 常见用途
- 全景监控
- 无人机导航
- 机器人避障

### 入门资源
- **鱼眼校正工具**：[github.com/ducha-aiki/fisheye-calibration](https://github.com/ducha-aiki/fisheye-calibration)
- **OpenCV鱼眼畸变校正**：[docs.opencv.org/4.x/db/d58/group__calib3d__fisheye.html](https://docs.opencv.org/4.x/db/d58/group__calib3d__fisheye.html)

---

## 7. 热成像相机

**红外相机**，检测物体温度。

### 核心特点
- **优点**：不受光照影响，可穿透烟雾
- **缺点**：分辨率低，价格贵

### 常见用途
- 夜间导航
- 人员检测
- 温度检测

### 入门资源
- **FLIR SDK**：[github.com/FLIR](https://github.com/FLIR)
- **热成像入门**：[learn.thermal.com](https://learn.thermal.com/)

---

## 8. 实用工具与资源

### 🛠️ 开发工具
| 工具 | 用途 | 链接 |
|------|------|------|
| OpenCV | 计算机视觉基础 | [github.com/opencv/opencv](https://github.com/opencv/opencv) |
| ROS | 机器人操作系统 | [github.com/ros](https://github.com/ros) |
| PyTorch3D | 3D视觉深度学习 | [github.com/facebookresearch/pytorch3d](https://github.com/facebookresearch/pytorch3d) |

### 📖 学习资源
- **视觉SLAM入门**：[github.com/gaoxiang12/slam_book](https://github.com/gaoxiang12/slam_book)
- **机器人感知课程**：[cs.stanford.edu/people/eroberts/courses/soco/projects/2009/p3/](https://cs.stanford.edu/people/eroberts/courses/soco/projects/2009/p3/)
- **Awesome Robotics**：[github.com/kiloreux/awesome-robotics](https://github.com/kiloreux/awesome-robotics)

### 🤝 社区与论坛
- **ROS Answers**：[answers.ros.org](https://answers.ros.org/)
- **Stack Overflow**：[stackoverflow.com/questions/tagged/robotics](https://stackoverflow.com/questions/tagged/robotics)
- **Reddit Robotics**：[reddit.com/r/robotics](https://www.reddit.com/r/robotics/)

---

## 🚀 入门建议

1. **从单目相机开始**：用USB摄像头 + OpenCV学习基础
2. **尝试RGB-D**：Intel RealSense D435i是很好的入门选择
3. **学习SLAM**：从ORB-SLAM开始理解视觉里程计
4. **多动手实践**：克隆GitHub项目，运行demo

---

## 📝 总结

| 相机类型 | 入门难度 | 主要用途 |
|----------|----------|----------|
| 单目 | ⭐⭐⭐ | 基础视觉任务 |
| 双目 | ⭐⭐ | 三维重建、SLAM |
| RGB-D | ⭐⭐ | 室内机器人、AR |
| ToF | ⭐⭐ | 手势识别、避障 |
| 事件相机 | ⭐ | 高速运动、低延迟 |

---

*欢迎贡献！如有补充请提交PR。*

*Last updated: 2024*

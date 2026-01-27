<a id="中文"></a>

# Panthera-HT 🐆

[![en](https://img.shields.io/badge/lang-English-blue.svg)](#english)[![中文](https://img.shields.io/badge/lang-简体中文-red.svg)](#中文)

面向学生和创客的开源六轴机械臂学习平台

<div align="center">
  <img alt="leader" src="images\head.jpg"/>
</div>

Panthera-HT是一款开源六轴机械臂，使用高擎机电的行星关节模组。我们面向开发者提供可复用的统一控制接口，用于算法验证、课程实验、系统集成及二次开发的标准化软硬件实验平台。

机械臂现有的控制方式包括C++、Python和ROS2，拥有的一些功能：位置/速度/力矩控制、阻抗控制、重力补偿模式、重力补偿-摩擦力补偿模式、主从遥操（双臂）、拖动示教等。此外，还支持在LeRobot框架下进行数据采集和推理。更多运行脚本请参考SDK文档。

## ✨ 项目起源与初心

这个项目的初心是**让学生党能以更低的价格玩到更高性能的关节电机机械臂**。

项目最初源自 [Ragtime-LAB/Ragtime_Panthera](https://github.com/Ragtime-LAB/Ragtime_Panthera) 的开源工作，我们在此基础上进行了完善和优化。感谢原作者 [wEch1ng(芝士榴莲肥牛)](https://github.com/wEch1ng) 的无私分享和开源精神！

为了方便学生学习**如何从0到1搭建和控制机械臂**，我们将从结构设计到控制算法统统开源，让每个人都能深入理解机械臂的工作原理。

后来项目原作者与高擎一拍即合，在高擎的支持下将项目完善落地，做成了一个更加完善的创客产品。但我们始终坚持开源理念，不对项目作出任何限制。

## 💡 设计理念

### 低成本 + 高性能

- **钣金框架**：选择高性价比的钣金作为整体框架，保证强度的同时降低成本
- **3D打印 + CNC加工**：配合3D打印和三轴CNC加工，实现灵活的结构设计
- **高性能关节模组**：使用高擎机电的行星关节模组，在成本和性能间取得平衡

### 完全开源 + 可扩展

- **结构开源**：提供SolidWorks原始设计文件、钣金展开图、3D打印STL文件
- **算法开源**：从底层控制到高级算法，所有代码完全开源
- **无限制修改**：你可以根据需求自由更换电机、修改结构、改变外观
- **模块化设计**：方便进行二次开发和功能扩展

### 教育导向

项目的核心目标是帮助学生和创客：
- 理解机械臂的机械结构设计
- 学习运动学和动力学算法
- 掌握电机控制和通信协议
- 实践从理论到实物的完整过程

## 📷 项目图片

<div align="center">
  <img src="./images/1.jpg" width="32%" />
  <img src="./images/2.jpg" width="32%" />
  <img src="./images/3.jpg" width="32%" />
  <br/>
  <img src="./images/4.jpg" width="32%" />
  <img src="./images/5.jpg" width="32%" />
  <img src="./images/6.jpg" width="32%" />
</div>

## ⚙️ 控制示例

### 位置速度控制：
<div align="center">
  <img src="./video/gif/pos&vel.gif" width="88%"/>
</div>

### 主从遥操：
<div align="center">
  <img src="./video/gif/Teleoperation.gif" width="88%"/>
</div>

### 主从遥操抓取：
<div align="center">
  <img src="./video/gif/Teleoperated_Grasping.gif" width="88%"/>
</div>

## 🗃️ 仓库

| 仓库                                                                              | 许可证         | 描述                                                    |
| --------------------------------------------------------------------------------- | -------------- | ------------------------------------------------------- |
| **[Panthera-HT_Main](https://github.com/HighTorque-Robotics/Panthera-HT_Main)**   | [MIT](LICENSE) | 主项目仓库，包含项目介绍、仓库链接和功能请求。          |
| **[Panthera-HT_Model](https://github.com/HighTorque-Robotics/Panthera-HT_Model)** | [MIT](LICENSE) | SolidWorks原始设计文件、钣金图、3D打印文件和物料清单（BOM）。 |
| **[Panthera-HT_SDK](https://github.com/HighTorque-Robotics/Panthera-HT_SDK)**     | [MIT](LICENSE) | Python SDK 开发包，提供快速上手的示例代码与开发工具链。 |
| **[Panthera-HT_ROS2](https://github.com/HighTorque-Robotics/Panthera-HT-ROS2)**   | [MIT](LICENSE) | ROS2 开发包，提供机械臂的驱动、控制与仿真支持。         |
| **[Panthera-HT_lerobot](https://github.com/HighTorque-Robotics/Panthera-HT_lerobot)** | [MIT](LICENSE) | LeRobot 集成包，支持模仿学习和机器人学习算法。 |

## 🚀 快速开始

### 硬件准备

1. 查看 [Panthera-HT_Model](https://github.com/HighTorque-Robotics/Panthera-HT_Model) 仓库获取完整的物料清单（BOM）
2. 准备钣金加工、3D打印和CNC加工的文件
3. 采购高擎机电的关节模组和其他电子元件

### 软件环境

1. 克隆SDK仓库：
```bash
git clone https://github.com/HighTorque-Robotics/Panthera-HT_SDK.git
cd Panthera-HT_SDK
```

2. 安装依赖并运行示例程序（详见SDK仓库的README）

### 第一个示例

参考 [Panthera-HT_SDK](https://github.com/HighTorque-Robotics/Panthera-HT_SDK) 中的示例代码，快速上手机械臂控制。

## 🤝 社区贡献

这个项目属于每一个热爱机器人的人！

### 完全开放

- ✅ **电机选择**：可以更换为其他品牌的关节模组
- ✅ **结构修改**：可以根据需求改变尺寸、材料、外观
- ✅ **算法优化**：欢迎提交更好的控制算法和功能
- ✅ **功能扩展**：添加视觉、力控、AI等新功能

### 我们需要你

项目在很多小细节上可能做得不够完善，我们需要社区的力量一起来完善：

- 📝 完善文档和教程
- 🐛 报告和修复bug
- 💡 提出新的功能建议
- 🔧 优化结构设计
- 📊 分享你的使用案例

欢迎提交 Issue 和 Pull Request！

## 🔗 相关文档与链接

**技术参数**：[机械臂各项参数](./images/parameters.jpg)

**视频演示**：
- 主从遥操打乒乓球：https://www.bilibili.com/video/BV1KprhBPE26/
- 移植LeRobot数据集进行模仿学习：https://www.bilibili.com/video/BV1GLi1BqETz/

**交流群**：
- QQ群：Panthera-HT交流群（1035440629）

**相关项目**：
- 夹爪设计参考：[UMI (Universal Manipulation Interface)](https://github.com/real-stanford/universal_manipulation_interface)

## 🚀 未来规划

我们将朝着两个方向持续发展：

### 高级传统控制
- 视觉伺服控制
- 使用 GraspNet 进行抓取
- 点云避障
- 更多传统控制算法

### 具身智能方向
- Pi0、Pi0.5 等前沿算法集成
- RoboTWin2.0 适配
- 端到端学习
- 多模态感知与控制

## 👥 贡献者

<a href="https://github.com/wEch1ng">
  <img src="https://github.com/wEch1ng.png" width="60px;" style="border-radius: 50%;" alt=""/>
</a>
<a href="https://github.com/tankail">
  <img src="https://github.com/tankail.png" width="60px;" style="border-radius: 50%;" alt=""/>
</a>

## ⚠️ 免责声明

> [!NOTE]
> 如果您基于此仓库构建或开发Panthera-HT，您将对其对您或他人造成的所有身体和精神损害承担全部责任。

---

<a id="english"></a>

# Panthera-HT 🐆

[![中文](https://img.shields.io/badge/lang-简体中文-red.svg)](#中文)[![en](https://img.shields.io/badge/lang-English-blue.svg)](#english)

An open-source six-axis robotic arm learning platform for students and makers

<div align="center">
  <img alt="leader" src="images\8.jpg"/>
</div>

Panthera-HT is an open-source six-axis robotic arm that uses HighTorque planetary joint modules. It provides developers with a reusable unified control interface, serving as a standardized hardware and software experimental platform for algorithm verification, course experiments, system integration, and secondary development.

The current control methods for the robotic arm include C++, Python, and ROS2, with features including: position/velocity/torque control, impedance control, gravity compensation mode, gravity compensation-friction compensation mode, master-slave teleoperation (dual arms), drag teaching, etc. Additionally, it supports data collection and inference under the LeRobot framework. For more operation scripts, please refer to the SDK documentation.

## ✨ Project Origin and Mission

The mission of this project is to **enable students to access high-performance joint motor robotic arms at a lower cost**.

The project originally stems from the open-source work of [Ragtime-LAB/Ragtime_Panthera](https://github.com/Ragtime-LAB/Ragtime_Panthera), which we have refined and optimized. Thanks to the original author [wEch1ng (芝士榴莲肥牛)](https://github.com/wEch1ng) for their selfless sharing and open-source spirit!

To help students learn **how to build and control a robotic arm from scratch (0 to 1)**, we have open-sourced everything from structural design to control algorithms, allowing everyone to deeply understand how robotic arms work.

Later, the original project author and HighTorque hit it off, and with HighTorque's support, the project was refined and brought to market as a more complete maker product. However, we always adhere to the open-source philosophy and impose no restrictions on the project.

## 💡 Design Philosophy

### Low Cost + High Performance

- **Sheet Metal Frame**: High cost-performance sheet metal as the main frame, ensuring strength while reducing costs
- **3D Printing + CNC Machining**: Combined with 3D printing and 3-axis CNC machining for flexible structural design
- **High-Performance Joint Modules**: Using HighTorque planetary joint modules, balancing cost and performance

### Fully Open Source + Scalable

- **Open Structure**: Provides SolidWorks original design files, sheet metal unfolding diagrams, 3D printing STL files
- **Open Algorithms**: All code from low-level control to advanced algorithms is fully open source
- **Unrestricted Modification**: You can freely replace motors, modify structures, and change appearance according to your needs
- **Modular Design**: Facilitates secondary development and feature expansion

### Education-Oriented

The core goal of the project is to help students and makers:
- Understand the mechanical structure design of robotic arms
- Learn kinematics and dynamics algorithms
- Master motor control and communication protocols
- Practice the complete process from theory to physical implementation

## 📷 Project Images

<div align="center">
  <img src="./images/1.jpg" width="32%" />
  <img src="./images/2.jpg" width="32%" />
  <img src="./images/3.jpg" width="32%" />
  <br/>
  <img src="./images/4.jpg" width="32%" />
  <img src="./images/5.jpg" width="32%" />
  <img src="./images/6.jpg" width="32%" />
</div>

## ⚙️ Control Examples

### Position and Speed Control:
<div align="center">
  <img src="./video/gif/pos&vel.gif" width="88%"/>
</div>

### Master-Slave Teleoperation:
<div align="center">
  <img src="./video/gif/Teleoperation.gif" width="88%"/>
</div>

### Master-Slave Teleoperated Grasping:
<div align="center">
  <img src="./video/gif/Teleoperated_Grasping.gif" width="88%"/>
</div>

## 🗃️ Repository

| Repository                                                                        | License        | Description                                                                                     |
| --------------------------------------------------------------------------------- | -------------- | ----------------------------------------------------------------------------------------------- |
| **[Panthera-HT_Main](https://github.com/HighTorque-Robotics/Panthera-HT_Main)**   | [MIT](LICENSE) | Main project repository, including project introduction, repository links, and feature requests. |
| **[Panthera-HT_Model](https://github.com/HighTorque-Robotics/Panthera-HT_Model)** | [MIT](LICENSE) | SolidWorks original design files, sheet metal unfolding diagrams, 3D printing files, and Bill of Materials (BOM). |
| **[Panthera-HT_SDK](https://github.com/HighTorque-Robotics/Panthera-HT_SDK)**     | [MIT](LICENSE) | Python SDK development package, providing quick-start example code and development toolchain. |
| **[Panthera-HT_ROS2](https://github.com/HighTorque-Robotics/Panthera-HT-ROS2)**   | [MIT](LICENSE) | ROS2 development package providing robotic arm drivers, control, and simulation support.        |
| **[Panthera-HT_lerobot](https://github.com/HighTorque-Robotics/Panthera-HT_lerobot)** | [MIT](LICENSE) | LeRobot integration package, supporting imitation learning and robot learning algorithms. |

## 🚀 Quick Start

### Hardware Preparation

1. Check the [Panthera-HT_Model](https://github.com/HighTorque-Robotics/Panthera-HT_Model) repository for the complete Bill of Materials (BOM)
2. Prepare files for sheet metal processing, 3D printing, and CNC machining
3. Purchase HighTorque joint modules and other electronic components

### Software Environment

1. Clone the SDK repository:
```bash
git clone https://github.com/HighTorque-Robotics/Panthera-HT_SDK.git
cd Panthera-HT_SDK
```

2. Install dependencies and run example programs (see SDK repository README for details)

### First Example

Refer to the example code in [Panthera-HT_SDK](https://github.com/HighTorque-Robotics/Panthera-HT_SDK) to quickly get started with robotic arm control.

## 🤝 Community Contribution

This project belongs to everyone who loves robotics!

### Fully Open

- ✅ **Motor Selection**: Can be replaced with joint modules from other brands
- ✅ **Structural Modification**: Can change size, materials, and appearance according to needs
- ✅ **Algorithm Optimization**: Welcome to submit better control algorithms and features
- ✅ **Feature Extension**: Add new features like vision, force control, AI, etc.

### We Need You

The project may not be perfect in many small details, and we need the community's help to improve it together:

- 📝 Improve documentation and tutorials
- 🐛 Report and fix bugs
- 💡 Propose new feature suggestions
- 🔧 Optimize structural design
- 📊 Share your use cases

Welcome to submit Issues and Pull Requests!

## 👥 Contributors

<a href="https://github.com/wEch1ng">
  <img src="https://github.com/wEch1ng.png" width="60px;" style="border-radius: 50%;" alt=""/>
</a>
<a href="https://github.com/tankail">
  <img src="https://github.com/tankail.png" width="60px;" style="border-radius: 50%;" alt=""/>
</a>

## 🔗 Related Documents and Links

**Technical Parameters**: [Robotic Arm Parameters](./images/parameters.jpg)

**Video Demonstrations**:
- Master-slave teleoperation playing table tennis: https://www.bilibili.com/video/BV1KprhBPE26/
- Porting LeRobot dataset for imitation learning: https://www.bilibili.com/video/BV1GLi1BqETz/

**Community**:
- QQ Group: Panthera-HT Community (1035440629)

**Related Projects**:
- Gripper Design Reference: [UMI (Universal Manipulation Interface)](https://github.com/real-stanford/universal_manipulation_interface)

## 🚀 Future Roadmap

We will continue to develop in two directions:

### Advanced Traditional Control
- Visual servoing control
- Grasping using GraspNet
- Point cloud obstacle avoidance
- More traditional control algorithms

### Embodied Intelligence
- Integration of cutting-edge algorithms like Pi0, Pi0.5
- RoboTWin2.0 adaptation
- End-to-end learning
- Multimodal perception and control

## ⚠️ Disclaimer

> [!Noth]
> If you build or develop Panthera-HT based on this repository, you will be fully responsible for all physical and mental damages caused to you or others.

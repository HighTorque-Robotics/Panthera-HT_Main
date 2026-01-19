# Panthera-HT 🌟

[![en](https://img.shields.io/badge/lang-English-blue.svg)](README.md) [![中文](https://img.shields.io/badge/lang-简体中文-brown.svg)](README_CN.md) 

基于高擎机电关节模组的开源六轴机械臂

<div align="center">
  <img alt="leader" src="images\head.jpg"/>
</div>

Panthera-HT是一款开源六轴机械臂，使用的电机都是高擎机电的行星关节模组。我们面向开发者提供可复用的统一控制接口，用于算法验证、课程实验、系统集成及二次开发的标准化软硬件实验平台。

机械臂现有的控制方式是纯Python脚本，拥有的一些功能：位置/速度/力矩控制、阻抗控制、重力补偿模式、重力补偿-摩擦力补偿模式、主从遥操（双臂）、拖动示教等，更多运行脚本请参考SDK文档。

## 📷 产品特写

<div align="center">
  <img src="./images/1.jpg" width="30%" />
  <img src="./images/2.jpg" width="30%" />
  <img src="./images/3.jpg" width="30%" />
  <br/>
  <img src="./images/4.jpg" width="30%" />
  <img src="./images/5.jpg" width="30%" />
  <img src="./images/6.jpg" width="30%" />
</div>

## ⚙️ 控制示例

### 位置速度控制：
<div align="center">
  <img src="./video/gif/pos&vel.gif" width="80%"/>
</div>

### 主从遥操：
<div align="center">
  <img src="./video/gif/Teleoperation.gif" width="80%"/>
</div>

### 主从遥操抓取：
<div align="center">
  <img src="./video/gif/Teleoperated_Grasping.gif" width="80%"/>
</div>

## 🗃️ 仓库

| 仓库                                                                                       | 许可证         | 描述                                            |
| ------------------------------------------------------------------------------------------ | -------------- | ----------------------------------------------- |
| **[Panthera-HT]([https:](https://github.com/HighTorque-Robotics/Panthera-HT_Main))**       | [MIT](LICENSE) | 主项目仓库，包含项目介绍、仓库链接和功能请求。  |
| **[Panthera-HT_SDK]([https:](https://github.com/HighTorque-Robotics/Panthera-HT_SDK))**    | [MIT](LICENSE) | SDK开发包，提供快速上手的示例代码与开发工具链。 |
| **[Panthera-HT_Model]([https:](https://github.com/HighTorque-Robotics/Panthera-HT_Main))** | [MIT](LICENSE) | SolidWorks原始设计文件和物料清单（BOM）。       |

## 🔗 相关文档与链接

[机械臂各项参数](./images/parameters.jpg)

开箱视频：(暂时无)

主从遥操打乒乓球：https://www.bilibili.com/video/BV1KprhBPE26/

移植LeRobot数据集进行模仿学习：https://www.bilibili.com/video/BV1GLi1BqETz/

## ⚠️ 免责声明 ⚠️

> [!NOTE]
> 如果您基于此仓库构建或开发Panthera-HT，您将对其对您或他人造成的所有身体和精神损害承担全部责任。


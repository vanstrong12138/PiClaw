# PiClaw: AgileX Robotics 技能集合库
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Language](https://img.shields.io/badge/language-Python-blue.svg)
![Platform](https://img.shields.io/badge/platform-Linux%20(Ubuntu)-green.svg)
PiClaw 是模块化技能集合仓库，聚焦机器人核心功能的快速集成与复用，覆盖机械臂控制、抓取、视觉感知、语音交互等关键场景，为机器人的二次开发和应用落地提供开箱即用的技能组件。

## 📋 目录
- [PiClaw: AgileX Robotics 技能集合库](#piclaw-agilex-robotics-技能集合库)
  - [📋 目录](#-目录)
  - [✨ 仓库特性](#-仓库特性)
  - [🚀 快速开始](#-快速开始)
    - [1. 克隆项目](#1-克隆项目)
    - [2. 提示Agent学习技能](#2-提示agent学习技能)
  - [📦 技能模块说明](#-技能模块说明)
  - [🤝 贡献指南](#-贡献指南)
  - [📄 许可证](#-许可证)
  - [📞 联系方式](#-联系方式)

## ✨ 仓库特性
- 🧩 **模块化设计**：每个技能独立封装，支持按需集成、单独调试，降低耦合度。
- 🎯 **场景化适配**：覆盖抓取、视觉、语音、机械臂控制等核心场景。
- 🚀 **易扩展**：统一的技能接口规范，新增自定义技能仅需遵循模板即可快速接入。


## 🚀 快速开始

### 1. 克隆项目

```Bash
git clone https://github.com/vanstrong12138/PiClaw.git
```

### 2. 提示Agent学习技能

以抓取技能为例：

```Bash
用户： 请学习vl_vision_skill
```

## 📦 技能模块说明

| 模块名称          | 功能说明                                                                  | 核心依赖       |
| ----------------- | ------------------------------------------------------------------------- | -------------- |
| `agx-arm-codegen` | 机械臂代码生成工具，自动生成轨迹规划、关节控制代码，支持自定义路径模板。  | pyAgxArm       |
| `grab_skill`      | 机器人抓取技能，包含夹爪控制、目标位姿校准、抓取策略（单点/自适应抓取）。 | pyAgxArm       |
| `vl_vision_skill` | 视觉感知技能，支持目标检测、视觉定位、图像分割。                          | SAM3，Qwen3-VL |
| `voice_skill`     | 语音交互技能，支持语音指令识别、语音反馈、自定义指令集配置。              | cosyoice       |

## 🤝 贡献指南

我们欢迎社区贡献，无论是修复bug、新增技能模块，还是优化文档，都可以按照以下步骤参与：

1. Fork 本仓库。

2. 新增功能需附带示例和测试用例。

3. 提交PR，描述清晰的修改内容、用途及测试结果。

4. 经过代码审核后合并。

## 📄 许可证

本仓库基于 MIT 许可证开源，详见 [LICENSE](./LICENSE) 文件。

## 📞 联系方式

- 问题反馈：提交 GitHub Issue（优先）

---

*Made with ❤️ for AgileX Robotics*


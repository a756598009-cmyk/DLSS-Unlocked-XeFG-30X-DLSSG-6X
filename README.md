# DLSS Unlocked XeFG 30X / DLSSG 6X

**XeFG 30× Multi-Frame Generation · DLSSG 6× Frame Generation**

[简体中文](#简体中文) | [English](#english)

An independent downstream project based on [ShyVortex/dlss-unlocked](https://github.com/ShyVortex/dlss-unlocked), focused on XeFG 30× multi-frame generation and DLSSG 6× frame generation compatibility, integration, configuration, and game testing.

基于 [ShyVortex/dlss-unlocked](https://github.com/ShyVortex/dlss-unlocked) 的独立下游项目，重点研究 XeFG 30× 多帧生成与 DLSSG 6× 帧生成兼容集成，并提供配置说明、部署指南和游戏测试记录。

---
整合包下载地址：
链接：https://pan.quark.cn/s/63af3159c11f?pwd=rB7B
提取码：rB7B

---


## 简体中文

### 项目简介

本项目基于上游 DLSS Unlocked 进行独立维护与功能集成，重点关注多帧生成技术的兼容性、运行配置和游戏实测。

项目主要研究以下两种帧生成路径：

- **XeFG 30× 多帧生成兼容集成**
- **DLSSG 6× 帧生成兼容集成**

同时保留上游项目已有的相关功能，并根据实际测试情况逐步完善配置方案、部署说明和兼容性文档。

### 核心功能

#### 1. XeFG 30× Multi-Frame Generation

- 研究和集成 XeSS/XeFG 相关帧生成组件。
- 以最高 30× 帧生成倍率为目标进行兼容性研究和测试。
- 关注不同游戏、运行环境、驱动及组件版本之间的兼容性。
- 记录实际测试结果和已知问题。

#### 2. DLSSG 6× Frame Generation

- 兼容集成 DLSSG 相关帧生成路径。
- 以 6× 帧生成倍率为目标进行配置和测试。
- 研究游戏原生帧生成接口与相关组件之间的兼容性。
- 根据测试结果持续优化配置和部署流程。

#### 3. 配置与部署

- 提供配置说明和安装指南。
- 整理常见兼容性问题及故障排查方法。
- 跟踪上游更新，并记录下游修改。
- 逐步完善不同游戏和运行环境的测试记录。

### 兼容性说明

功能是否可用取决于游戏、显卡、驱动、帧生成组件和具体配置。

文中提及的 30×、6× 为项目目标功能倍率，不代表所有游戏、显卡和配置均已验证支持。实际可用倍率、生成帧质量、延迟和性能表现应以具体测试结果为准。

### 安装与使用

使用教程（简体中文）

教程一：标准版安装与使用

将 .7z 压缩包复制到目标游戏的根目录，并解压或按照压缩包内的说明放置文件。

运行 「开关30倍帧生成」。

根据程序提示，输入对应的数字，选择需要启用的多帧生成方式。

完成选择后，启动游戏。后续操作与常规 OptiScaler 的使用流程基本一致。

版本说明： 此版本加入了 4 种 XeSS 30× 帧生成方式。具体模式以程序实际显示的选项为准。

教程二：滤镜版安装与使用（ReShade）

第一步：部署游戏文件

将 .7z 压缩包复制到目标游戏的根目录，并解压或按照压缩包内的说明放置文件。

运行 「开关30倍帧生成」。

根据程序提示，输入对应数字，选择需要启用的多帧生成方式。

第二步：启用滤镜功能

运行 「开关30倍帧生成_+更换最新红色版本+滤镜.exe」。

根据程序提示，输入数字 8，选择滤镜功能。

第三步：安装 ReShade

运行 ReShade_Setup_6.8.0.exe。

点击 Browse，选择游戏根目录中的游戏主程序 .exe 文件。

点击 Open。

按照安装向导依次点击 Next → Next → Finish，完成安装。

第四步：覆盖滤镜文件

解压滤镜文件。

找到其中的 reshade-shaders 文件夹。

将该文件夹复制到游戏根目录，并覆盖已有的同名文件夹。

启动游戏，按 Home 键呼出 ReShade 滤镜界面。

后续滤镜配置与常规 OptiScaler / ReShade 使用流程基本一致。

版本说明： 此版本加入了 4 种 XeSS 30× 帧生成方式。请根据实际菜单选项选择对应模式。

### 故障排查

遇到游戏无法启动、黑屏、闪退、帧生成选项不可用或画面异常时，建议依次检查：

- 游戏是否满足对应帧生成路径的基本要求。
- DLL 文件是否放在正确的游戏目录。
- 配置文件是否与当前组件版本匹配。
- 是否存在其他注入工具、覆盖层或代理 DLL 冲突。
- 游戏日志、组件日志及驱动版本是否提供进一步线索。

请在提交问题时附上游戏名称、显卡型号、驱动版本、组件版本、配置文件和相关日志。

### 上游项目与致谢

本项目基于 [ShyVortex/dlss-unlocked](https://github.com/ShyVortex/dlss-unlocked) 进行下游开发。

感谢上游作者及相关开源项目开发者的工作，包括：

- [DLSS Unlocked](https://github.com/ShyVortex/dlss-unlocked)
- [OptiScaler](https://github.com/optiscaler/OptiScaler)
- [OptiScaler-DLSSNR-PreSR-Multipass](https://github.com/wilsjo2/OptiScaler-DLSSNR-PreSR-Multipass)
- [dlssg_for_sm86](https://github.com/sdli1995/dlssg_for_sm86)
- [DLSS Enabler](https://github.com/artur-graniszewski/DLSS-Enabler)
- [REFramework](https://github.com/praydog/REFramework)

具体组件的作者、版权和许可证应以各自上游仓库及随附的第三方声明为准。

### 免责声明

本项目是独立的社区下游研究与集成项目，并非任何硬件厂商或游戏开发商的官方产品，也不代表相关厂商的认可或背书。

第三方组件、运行时文件及相关技术均受各自的许可证和使用条款约束。使用者应自行确认相关组件的使用与分发条件。

本项目按现状提供，不对兼容性、稳定性、性能或特定用途作任何保证。请自行评估使用风险，并遵守游戏及相关软件的使用条款。

---

## English

### Overview

DLSS Unlocked XeFG 30X / DLSSG 6X is an independent downstream project based on [ShyVortex/dlss-unlocked](https://github.com/ShyVortex/dlss-unlocked).

The project focuses on frame generation compatibility, integration, configuration, deployment, and reproducible game testing.

Its primary research targets are:

- **XeFG 30× Multi-Frame Generation compatibility**
- **DLSSG 6× Frame Generation compatibility**

The project also maintains relevant upstream functionality and documents downstream changes as development progresses.

### Core Features

#### 1. XeFG 30× Multi-Frame Generation

- Research and integration of relevant XeSS/XeFG frame generation components.
- Compatibility testing targeting up to 30× frame generation.
- Evaluation across games, drivers, runtime environments, and component versions.
- Documentation of test results and known issues.

#### 2. DLSSG 6× Frame Generation

- Compatibility integration of the DLSSG frame generation path.
- Configuration and testing targeting 6× frame generation.
- Investigation of compatibility between native game interfaces and supporting components.
- Iterative improvements to configuration and deployment workflows.

#### 3. Configuration and Deployment

- Installation and configuration documentation.
- Troubleshooting guidance for common compatibility issues.
- Upstream update tracking and downstream change documentation.
- Gradual expansion of game and environment compatibility records.

### Compatibility Notice

Feature availability depends on the game, GPU, driver, frame generation components, and configuration.

The 30× and 6× figures represent project feature targets. They do not imply universal support across all games, GPUs, or configurations. Actual available multipliers, frame quality, latency, and performance must be verified through testing.

### Installation and Usage

Usage Guide (English)

Tutorial 1: Standard Edition

Copy the .7z archive to the target game's root directory. Extract the archive or place its contents according to the included instructions.

Run "开关30倍帧生成" (30× Frame Generation Switch).

Follow the on-screen prompts and enter the corresponding number to select the desired multi-frame generation mode.

Launch the game. The remaining steps are generally similar to the standard OptiScaler workflow.

Version note: This release includes four XeSS 30× frame generation modes. Refer to the options displayed by the program for the available choices.

Tutorial 2: Filter Edition (ReShade)

Step 1: Deploy the game files

Copy the .7z archive to the target game's root directory. Extract the archive or place its contents according to the included instructions.

Run "开关30倍帧生成" (30× Frame Generation Switch).

Follow the on-screen prompts and enter the corresponding number to select the desired multi-frame generation mode.

Step 2: Enable the filter feature

Run "开关30倍帧生成_+更换最新红色版本+滤镜.exe".

When prompted, enter 8 to select the filter feature.

Step 3: Install ReShade

Run ReShade_Setup_6.8.0.exe.

Click Browse and select the game's main .exe file in the game root directory.

Click Open.

Follow the installer prompts by clicking Next → Next → Finish.

Step 4: Copy the filter files

Extract the filter archive.

Locate the reshade-shaders folder inside the extracted files.

Copy it into the game's root directory and overwrite the existing folder with the same name.

Launch the game and press Home to open the ReShade interface.

Continue configuring the filters using the standard OptiScaler / ReShade workflow.

Version note: This release includes four XeSS 30× frame generation modes. Select the appropriate mode based on the options displayed by the program.
### Troubleshooting

For launch failures, black screens, crashes, unavailable frame generation options, or visual artifacts, check:

- Whether the game meets the requirements of the selected frame generation path.
- Whether the required DLL files are installed in the correct directory.
- Whether the configuration matches the component version.
- Whether other injection tools, overlays, or proxy DLLs conflict.
- Whether game logs, component logs, or driver information provide additional clues.

When reporting an issue, include the game title, GPU, driver version, component version, configuration, and relevant logs.

### Upstream Project and Credits

This project is an independent downstream development effort based on [ShyVortex/dlss-unlocked](https://github.com/ShyVortex/dlss-unlocked).

Thanks to the upstream maintainers and open-source contributors, including:

- [DLSS Unlocked](https://github.com/ShyVortex/dlss-unlocked)
- [OptiScaler](https://github.com/optiscaler/OptiScaler)
- [OptiScaler-DLSSNR-PreSR-Multipass](https://github.com/wilsjo2/OptiScaler-DLSSNR-PreSR-Multipass)
- [dlssg_for_sm86](https://github.com/sdli1995/dlssg_for_sm86)
- [DLSS Enabler](https://github.com/artur-graniszewski/DLSS-Enabler)
- [REFramework](https://github.com/praydog/REFramework)

Please refer to each upstream repository and its accompanying third-party notices for accurate attribution and licensing information.

### Disclaimer

This is an independent community research and integration project. It is not an official product of, nor affiliated with or endorsed by, any hardware vendor or game developer.

Third-party components, runtime files, and related technologies remain subject to their respective licenses and terms. Users are responsible for verifying applicable usage and redistribution requirements.

This project is provided as is, without guarantees regarding compatibility, stability, performance, or fitness for a particular purpose. Use it at your own risk and comply with the applicable software and game terms.

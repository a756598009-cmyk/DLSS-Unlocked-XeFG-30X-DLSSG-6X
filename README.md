# DLSS Unlocked XeFG 30X / DLSSG 6X

**XeFG 30× Multi-Frame Generation · DLSSG 6× Frame Generation**

[简体中文](#简体中文) | [English](#english)

An independent downstream project based on [ShyVortex/dlss-unlocked](https://github.com/ShyVortex/dlss-unlocked), focused on XeFG 30× multi-frame generation and DLSSG 6× frame generation compatibility, integration, configuration, and game testing.

基于 [ShyVortex/dlss-unlocked](https://github.com/ShyVortex/dlss-unlocked) 的独立下游项目，重点研究 XeFG 30× 多帧生成与 DLSSG 6× 帧生成兼容集成，并提供配置说明、部署指南和游戏测试记录。

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

1. 前往项目的 [Releases](../../releases) 页面查看可用版本。
2. 阅读对应版本的更新说明和安装要求。
3. 按照项目提供的安装包或独立压缩包说明进行部署。
4. 根据目标游戏和组件要求调整配置。
5. 首次运行时建议使用保守设置，确认游戏正常启动后再逐步测试更高倍率。

如果当前没有可用的正式 Release，请以仓库源码和相关组件的官方文档为准。

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

1. Visit the project's [Releases](../../releases) page.
2. Review the release notes and requirements.
3. Follow the installation instructions for the available installer or standalone archive.
4. Configure the components for the target game.
5. Start with conservative settings, verify stability, and then test higher multipliers.

If no official release is available yet, refer to the source code and the documentation of the relevant upstream components.

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

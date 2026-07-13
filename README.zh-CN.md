# NMRiH Ping System（重制版）

> [!WARNING]
> 这是 [dysphie/nmrih-ping-system](https://github.com/dysphie/nmrih-ping-system) 的重制版。
> 原作者已在 GitHub 仓库中声明：**自 Torn Banner 收购该游戏后，原插件已停止维护**。
> 本重制版的创建目的在于让该插件在当前的 NMRiH 独立服务器上继续可用。

## 概述

本插件允许玩家指向游戏世界中的位置，创建一个可视化和可听见的标记（Ping），其他玩家也能看到和听到该标记。标记可用于沟通位置、目标、敌人、物品或游戏世界中的任何其他事物。

本重制版由 **Baimiao2534** 维护，为多语言支持做贡献。

## 致谢

- **原作者**：[dysphie](https://github.com/dysphie)
- **原仓库**：[dysphie/nmrih-ping-system](https://github.com/dysphie/nmrih-ping-system)
- **重制维护**：[Baimiao2534](https://github.com/Baimiao2534)

## 运行环境

- [SourceMod 1.12](https://www.sourcemod.net/downloads.php?branch=stable)（1.11 可用，但性能会有所下降）
- （可选）Client Preferences 扩展和插件，允许玩家隐藏标记（默认随 SourceMod 一起捆绑并启用）

## 安装方法

- 从 Releases 页面下载最新的 ZIP 压缩包
- 将压缩包内容解压到 `addons/sourcemod` 目录
- 在服务器控制台执行 `sm_reload_translations` 重新加载翻译
- 加载插件：`sm plugins load nmrih-ping`

## 目录结构

```
addons/sourcemod/
├── plugins/
│   └── nmrih-ping.smx
├── scripting/
│   └── nmrih-ping.sp
└── translations/
    ├── ping.phrases.txt       (英语)
    ├── chi/
    │   └── ping.phrases.txt   (简体中文)
    └── zho/
        └── ping.phrases.txt   (繁体中文)
```

## 使用方法

A. 打开语音菜单（默认按键：`3`），然后按下使用键（默认按键：`E`）

B. 绑定一个按键到 `sm_ping` 命令。例如：

```
bind mouse3 sm_ping
```

## 客户端偏好设置

玩家可以通过 `sm_settings` -> `Player Pings` 切换是否显示标记

## 翻译

本重制版包含以下语言的翻译：

- 英语
- 简体中文（chi）
- 繁体中文（zho）

## 许可证

本插件基于 **GNU General Public License v3.0（GPLv3）** 许可证发布，该许可证继承自原作者 dysphie 的原作。

- 在遵守许可证条款和条件的前提下，您可以自由使用、修改和分发本插件。
- 许可证副本可在 [LICENSE](LICENSE) 文件中查看。
- 对源代码的修改必须以相同的 GPLv3 许可证发布。

完整的许可证文本请参见 <https://www.gnu.org/licenses/gpl-3.0.html>。

# WinBridge Store

WinBridge 应用商店的资产仓库，提供 Wine 组件、Windows 应用安装包和浏览器扩展。

## 仓库结构

```
winbridge-store/
├── apps/                    # Windows 应用清单
│   ├── apps-developer.json  # 开发者工具（Notepad++, Sublime Text等）
│   ├── apps-media.json      # 媒体工具（VLC, foobar2000等）
│   ├── apps-office.json     # 办公软件（LibreOffice, SumatraPDF等）
│   └── apps-utilities.json  # 实用工具（7-Zip, Everything等）
├── assets/                  # Wine 资产清单
│   ├── assets-core.json     # 核心组件（Box64, 容器模板, PulseAudio）
│   ├── assets-graphics.json # 图形组件（DXVK, D8VK, VKD3D, GPU驱动）
│   └── assets-runtime.json  # 运行时组件（VC++, .NET, Direct3D等）
├── extensions/              # 浏览器扩展清单
│   ├── extensions-adblock.json
│   ├── extensions-developer.json
│   ├── extensions-privacy.json
│   ├── extensions-productivity.json
│   └── extensions-translate.json
├── icons/                   # 图标资源
│   ├── apps/                # 应用图标
│   ├── assets/              # Wine 组件图标
│   └── extensions/          # 浏览器扩展图标
└── README.md
```

## Release 标签说明

| Release | 内容 | 下载地址 |
|---------|------|----------|
| **v1** | Windows 应用安装包（7-Zip, Firefox, VLC等13款） | [Release v1](https://github.com/YangRQ-2006/winbridge-store/releases/tag/v1) |
| **v2** | Wine 图形组件（DXVK, D8VK, VKD3D, Direct3D等） | [Release v2](https://github.com/YangRQ-2006/winbridge-store/releases/tag/v2) |
| **v3** | Wine 核心组件（Box64, rootfs, 容器模板, PulseAudio） | [Release v3](https://github.com/YangRQ-2006/winbridge-store/releases/tag/v3) |
| **v4** | 浏览器扩展（uBlock Origin, 沉浸式翻译等） | [Release v4](https://github.com/YangRQ-2006/winbridge-store/releases/tag/v4) |

## 使用说明

### Wine 组件

Wine 组件用于在 Android 设备上运行 Windows 程序：

- **Box64** - x86_64 指令转译器
- **Container Pattern** - Wine 容器模板
- **PulseAudio** - 音频服务
- **DXVK/D8VK/VKD3D** - DirectX → Vulkan 转换层
- **GPU Drivers** - 高通 Turnip / 联发科 Vortek 驱动
- **Runtime** - VC++, .NET Framework, Direct3D等运行时

### Windows 应用

预打包的 Windows 应用安装包，可直接在 WinBridge 中安装运行：

- **办公软件** - LibreOffice, SumatraPDF, Foxit PDF
- **媒体工具** - VLC, foobar2000, IrfanView
- **开发者工具** - Notepad++, Sublime Text, XAMPP
- **实用工具** - 7-Zip, Everything, Process Explorer

### 浏览器扩展

为 WinBridge 内置浏览器提供的扩展：

- **广告拦截** - uBlock Origin, AdGuard
- **翻译工具** - 沉浸式翻译, Google 翻译
- **开发者工具** - Vue.js devtools, React Developer Tools
- **隐私保护** - Privacy Badger, HTTPS Everywhere
- **效率工具** - Notion Web Clipper, Todoist

## 许可证

MIT License

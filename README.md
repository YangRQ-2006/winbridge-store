# WinBridge Store

WinBridge 应用商店的后台数据仓库，收录常用 Wine 兼容性较好的办公/实用软件。

## 仓库结构

```
apps/
├── apps-office.json      # 办公软件
├── apps-utilities.json   # 实用工具
├── apps-media.json       # 多媒体软件
└── apps-developer.json   # 开发工具
```

## 当前收录软件

### 办公软件

| 软件 | 简介 | Wine 评级 | 价格 |
|------|------|-----------|------|
| [7-Zip](https://www.7-zip.org) | 免费开源的文件压缩与解压缩工具，支持 7z、ZIP、RAR 等多种格式 | Platinum | 免费 |
| [Notepad++](https://notepad-plus-plus.org) | 轻量级但功能强大的代码编辑器，支持语法高亮、多标签 | Platinum | 免费 |
| [VLC 媒体播放器](https://www.videolan.org) | 免费开源的跨平台媒体播放器，支持几乎所有音视频格式 | Gold | 免费 |
| [Mozilla Firefox](https://www.mozilla.org) | 快速、安全的开源网络浏览器，注重隐私保护 | Gold | 免费 |
| [LibreOffice](https://www.libreoffice.org) | 功能强大的开源办公软件套件，与 Microsoft Office 高度兼容 | Gold | 免费 |

### 实用工具

| 软件 | 简介 | Wine 评级 | 价格 |
|------|------|-----------|------|
| [XAMPP](https://www.apachefriends.org) | 轻量级 Apache + MySQL + PHP 开发环境 | Silver | 免费 |
| [GIMP](https://www.gimp.org) | 功能强大的开源图像编辑软件，Photoshop 免费替代 | Gold | 免费 |
| [Foobar2000](https://www.foobar2000.org) | 轻量级高保真音频播放器，资源占用极低 | Platinum | 免费 |
| [IrfanView](https://www.irfanview.com) | 小巧快速的图像查看器，支持 100 多种图片格式 | Platinum | 免费 |
| [CCleaner](https://www.ccleaner.com) | 系统清理优化工具，清理垃圾文件和注册表 | Gold | 免费版 |

### 多媒体软件

| 软件 | 简介 | Wine 评级 | 价格 |
|------|------|-----------|------|
| [Audacity](https://www.audacityteam.org) | 免费开源的音频编辑和录音软件，支持多轨道编辑 | Platinum | 免费 |
| [HandBrake](https://handbrake.fr) | 免费开源的视频转码工具，支持几乎所有视频格式 | Gold | 免费 |

### 开发工具

| 软件 | 简介 | Wine 评级 | 价格 |
|------|------|-----------|------|
| [Visual Studio Code](https://code.visualstudio.com) | 微软出品的免费代码编辑器，支持丰富的扩展插件 | Silver | 免费 |
| [Git](https://git-scm.com) | 分布式版本控制系统，现代软件开发必备工具 | Platinum | 免费 |

## 数据格式

每个 JSON 文件包含软件的基本信息、截图、ProtonDB 兼容性评级和 Winlator 运行提示。

```json
{
  "appId": 810001,
  "name": "7-Zip",
  "packageName": "7zip",
  "iconUrl": "https://...",
  "headerImage": "https://...",
  "screenshots": ["https://..."],
  "shortDescription": "...",
  "detailedDescription": "...",
  "genres": ["实用工具", "压缩软件"],
  "isFree": true,
  "price": "免费",
  "protonTier": "platinum",
  "totalReports": 128,
  "winlatorNotes": "...",
  "downloadUrl": "https://...",
  "officialSite": "https://..."
}
```

## 如何添加新软件

1. Fork 本仓库
2. 在对应分类的 JSON 文件中添加新条目
3. 提交 Pull Request

或直接在 [WinBridge 项目](https://github.com/YangRQ-2006/Win11Launcher) 中提交 Issue 请求添加。

## 许可证

MIT License

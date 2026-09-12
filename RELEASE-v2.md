# WinBridge Store v2 - 资产与扩展

## 📁 目录结构

```
v2/
├── packages/                    # Wine 资产包
│   ├── box64-0.4.0.tzst       # Box64 转译器 (4.0 MB)
│   ├── wine-9.0.tzst          # Wine 运行时 (62 MB)
│   ├── container_pattern.tzst  # 容器模板 (7.1 MB)
│   ├── pulseaudio.tzst        # 音频服务 (44 KB)
│   ├── graphics/              # 图形驱动
│   │   ├── dxvk-2.3.tzst     # DirectX 9/10/11 → Vulkan
│   │   ├── d8vk-0.4.tzst     # DirectX 8 → Vulkan
│   │   ├── vkd3d-1.9.tzst    # DirectX 12 → Vulkan
│   │   ├── turnip-24.1.tzst  # 高通 Adreno GPU
│   │   └── vortek-1.2.tzst   # 联发科 Mali GPU
│   └── wincomponents/         # Windows 运行时
│       ├── vcrun2019.tzst     # Visual C++ 2015-2019
│       ├── d3dcompiler_47.tzst # D3DCompiler 47
│       ├── dotnet48.tzst      # .NET Framework 4.8
│       └── winhttp.tzst       # Windows HTTP 服务
├── extensions-packages/       # 浏览器扩展
│   ├── ublock-origin-1.50.crx
│   ├── immersive-translate-1.5.crx
│   └── vue-devtools-6.5.crx
└── apps/                      # EXE 应用安装包
    ├── 7z2409-x64.exe
    ├── Firefox-Setup-155.0-x64-zhCN.exe
    └── ... (13 款应用)
```

## 🔗 JSON 数据源

- **资产清单**: `assets/assets-core.json`, `assets-graphics.json`, `assets-runtime.json`
- **扩展清单**: `extensions/extensions-*.json`

## 📦 文件说明

### 核心资产
| 文件 | 大小 | 说明 |
|------|------|------|
| box64-0.4.0.tzst | 4.0 MB | x86_64 指令转译器 |
| wine-9.0.tzst | 62 MB | Windows 程序运行环境 |
| container_pattern.tzst | 7.1 MB | Wine 前缀初始化模板 |
| pulseaudio.tzst | 44 KB | 音频服务 |

### 图形驱动
| 文件 | 大小 | GPU 厂商 |
|------|------|----------|
| dxvk-2.3.tzst | 9 MB | 通用 |
| d8vk-0.4.tzst | 3 MB | 通用 |
| vkd3d-1.9.tzst | 4 MB | 通用 |
| turnip-24.1.tzst | 3 MB | 高通 |
| vortek-1.2.tzst | 2 MB | 联发科 |

### 运行时组件
| 文件 | 大小 | 说明 |
|------|------|------|
| vcrun2019.tzst | 15 MB | Visual C++ 运行时 |
| d3dcompiler_47.tzst | 2 MB | 着色器编译器 |
| dotnet48.tzst | 60 MB | .NET Framework |
| winhttp.tzst | 1 MB | HTTP 服务 |

## 🧩 扩展商店

扩展数据源使用 Microsoft Edge Add-ons，支持以下分类：
- 广告拦截 (adblock)
- 隐私保护 (privacy)
- 生产力工具 (productivity)
- 开发者工具 (developer)
- 翻译工具 (translate)

## 📝 更新日志

### v2 (2025-01-15)
- ✨ 新增资产分类管理
- ✨ 新增扩展商店支持
- 📦 整理 Release 结构
- 🔗 添加 JSON 数据源

# XMBOX-Release

XMBOX视频播放器更新源

## 仓库结构

```
XMBOX-Release/
├── apk/
│   ├── release/           # 正式版本
│   │   ├── mobile.json           # 手机版版本信息
│   │   ├── leanback.json         # TV版版本信息
│   │   ├── mobile-arm64_v8a.apk  # 手机版 ARM64
│   │   ├── mobile-armeabi_v7a.apk # 手机版 ARMv7
│   │   ├── leanback-arm64_v8a.apk # TV版 ARM64
│   │   └── leanback-armeabi_v7a.apk # TV版 ARMv7
│   └── dev/              # 开发版本
│       ├── mobile.json           # 手机版开发版信息
│       ├── leanback.json         # TV版开发版信息
│       ├── mobile-arm64_v8a.apk  # 手机版开发版 ARM64
│       ├── mobile-armeabi_v7a.apk # 手机版开发版 ARMv7
│       ├── leanback-arm64_v8a.apk # TV版开发版 ARM64
│       └── leanback-armeabi_v7a.apk # TV版开发版 ARMv7
└── README.md
```

## JSON 文件格式

版本信息文件采用以下格式：

```json
{
  "name": "3.0.7",
  "desc": "版本更新说明\n支持多行描述",
  "code": 307
}
```

### 字段说明

- `name`: 版本名称，对应 `versionName`
- `desc`: 版本描述，支持换行符 `\n`
- `code`: 版本号，对应 `versionCode`，用于版本比较

## 版本说明

### 正式版 (Release)
- **当前版本**: v3.0.7 (code: 307)
- **功能**: 稳定版本，适合日常使用
- **更新频率**: 定期更新

### 开发版 (Dev)
- **当前版本**: v3.0.8-dev (code: 308)
- **功能**: 测试新功能，可能不稳定
- **更新频率**: 频繁更新
- **注意**: 仅供测试使用

## 应用类型

### Mobile 版本
- 适用于手机和平板设备
- 触摸操作优化
- 标准 Android 界面

### Leanback 版本
- 专为 Android TV 和机顶盒设计
- 遥控器操作优化
- 10-foot UI 界面

## 支持架构

- **ARM64-v8a**: 64位ARM架构（推荐）
- **ARMv7a**: 32位ARM架构（兼容性）

## 更新源地址

### 主源（GitHub）
```
https://raw.githubusercontent.com/Tosencen/XMBOX-Release/main/
```

### 镜像源（Gitee）
```
https://gitee.com/ochenoktochen/XMBOX-Release/raw/main/
```

## 自动更新机制

应用会自动检测网络环境，选择最快的更新源：

1. 首先测试 GitHub 主源
2. 如果主源较慢或无法访问，切换到 Gitee 镜像
3. 智能缓存测速结果，24小时内复用

## 手动更新

### 获取版本信息
```bash
# 正式版手机版
curl "https://raw.githubusercontent.com/Tosencen/XMBOX-Release/main/apk/release/mobile.json"

# 正式版TV版
curl "https://raw.githubusercontent.com/Tosencen/XMBOX-Release/main/apk/release/leanback.json"

# 开发版
curl "https://raw.githubusercontent.com/Tosencen/XMBOX-Release/main/apk/dev/mobile.json"
```

### 下载APK
```bash
# 下载正式版手机版 ARM64
wget "https://raw.githubusercontent.com/Tosencen/XMBOX-Release/main/apk/release/mobile-arm64_v8a.apk"
```

## 维护说明

本仓库用于 XMBOX 应用的自动更新功能，包含：

- 版本信息 JSON 文件
- 对应版本的 APK 文件
- 支持正式版和开发版双渠道
- 提供 GitHub 和 Gitee 双源访问

---

**XMBOX** - 基于 [FongMi/TV](https://github.com/FongMi/TV) 二开的影视播放器应用

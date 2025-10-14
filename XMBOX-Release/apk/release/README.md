# XMBOX Release Files

## 📁 文件结构

```
apk/release/
├── mobile.json          # 最新版本信息 (手机版)
├── leanback.json        # 最新版本信息 (TV版)
├── v3.0.7/              # v3.0.7版本文件
│   ├── mobile.json      # v3.0.7版本信息
│   ├── leanback.json    # v3.0.7版本信息
│   ├── mobile-arm64_v8a.apk
│   ├── mobile-armeabi_v7a.apk
│   ├── leanback-arm64_v8a.apk
│   └── leanback-armeabi_v7a.apk
└── v3.0.8/              # v3.0.8版本文件
    ├── mobile.json      # v3.0.8版本信息
    ├── leanback.json    # v3.0.8版本信息
    ├── mobile-arm64_v8a-v3.0.8.apk
    ├── mobile-armeabi_v7a-v3.0.8.apk
    ├── leanback-arm64_v8a-v3.0.8.apk
    └── leanback-armeabi_v7a-v3.0.8.apk
```

## 📱 版本说明

### v3.0.8 (最新版本)
- **发布时间**: 2025-10-14
- **版本代码**: 308
- **主要更新**: UI交互体验全面优化

### v3.0.7
- **发布时间**: 2025-09-26  
- **版本代码**: 307
- **主要更新**: 全面优化稳定性和用户体验

## 🔗 下载链接

### 最新版本 (v3.0.8)
- **手机版 ARM64**: [mobile-arm64_v8a-v3.0.8.apk](v3.0.8/mobile-arm64_v8a-v3.0.8.apk)
- **手机版 ARMv7**: [mobile-armeabi_v7a-v3.0.8.apk](v3.0.8/mobile-armeabi_v7a-v3.0.8.apk)
- **TV版 ARM64**: [leanback-arm64_v8a-v3.0.8.apk](v3.0.8/leanback-arm64_v8a-v3.0.8.apk)
- **TV版 ARMv7**: [leanback-armeabi_v7a-v3.0.8.apk](v3.0.8/leanback-armeabi_v7a-v3.0.8.apk)

### 历史版本
- **v3.0.7**: [查看v3.0.7版本文件](v3.0.7/)

## 📋 版本信息

每个版本目录都包含对应的JSON配置文件，包含：
- `name`: 版本号
- `desc`: 版本描述和更新内容
- `code`: 版本代码
- `downloads`: 下载链接映射 (仅根目录文件)

## 🔐 签名信息

所有APK文件均使用多重签名保护：
- ✅ v1 (JAR签名) - 最佳兼容性
- ✅ v2 (APK签名方案v2) - 全文件签名
- ✅ v3 (APK签名方案v3) - 支持密钥轮换
- ✅ v4 (APK签名方案v4) - 增量签名

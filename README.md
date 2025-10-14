# XMBOX-Release

XMBOX视频播放器更新源

## 文件说明

- `mobile.json` - 手机版版本信息
- `leanback.json` - TV版版本信息
- `*.apk` - 对应版本的APK文件

## 更新源

- GitHub: `https://raw.githubusercontent.com/Tosencen/XMBOX-Release/main/`
- Gitee: `https://gitee.com/ochenoktochen/XMBOX-Release/raw/main/`

## JSON格式

```json
{
  "name": "3.0.8",
  "desc": "版本更新说明",
  "code": 308,
  "downloads": {
    "arm64_v8a": "v3.0.8/mobile-arm64_v8a-v3.0.8.apk",
    "armeabi_v7a": "v3.0.8/mobile-armeabi_v7a-v3.0.8.apk"
  }
}
```
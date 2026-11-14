# Fs20modConverterV3

FS19 mod → FS20（移动版）转换器 · 发布仓库 + 云更新通道。

## 应用内更新

APK 启动后进入「设置 → 云更新」会自动读取本仓库根目录的 `version.json`，
比较 versionCode，有新版本即可一键下载并安装，无需手动找链接。

## version.json

```json
{
  "versionCode": 1302,
  "versionName": "1.3.2.0",
  "url": "https://raw.githubusercontent.com/.../apk",
  "size": 1460000,
  "notes": "更新说明"
}
```

每次发版：上传新 APK → 同步改 version.json（versionCode 必须递增）→ push。

## 目录

- `Fs20modConverterV3_<ver>.apk` —— 已签名安装包
- `Fs20modConverterV3_工程源码.zip` —— 工程源码
- `version.json` —— 云更新清单

签名密钥不入库，单独保管。

## 历史版本

见 git 提交记录。

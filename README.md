# 理论考试练习系统 Android 测试版

本仓库仅用于公开分发 Android APK。项目源码仓库仍保持私有；这里不包含源码、数据库、账号密码、MeFrp 凭据或私钥。

## APK 信息

| 项目 | 值 |
| --- | --- |
| applicationId | `com.theoryexam.mobile.dev` |
| 版本 | `1.0.0-dev.10`（versionCode 10） |
| 签名 | Android Debug 测试签名 |
| SHA-256 | `5d0089f664c63d52ade066679b38320c12b418de54613c716dd19a443e78ebb2` |
| 验收设备 | Android 15 / API 35 |

**这是 Debug 测试包，不是正式生产版。** 它没有正式发布签名，也不保证与之后的正式 APK 连续升级。请勿将其用于需要正式发布保证的场景。

## 下载与校验

前往 [GitHub Releases](https://github.com/MilchstraBe-Endless10/theory-exam-android-downloads/releases)，下载 `theory-exam-mobile-dev.10.apk` 和同名 `.sha256` 文件。Linux/macOS 可运行：

```sh
sha256sum -c theory-exam-mobile-dev.10.apk.sha256
```

Windows PowerShell 可运行：

```powershell
Get-FileHash .\theory-exam-mobile-dev.10.apk -Algorithm SHA256
```

计算结果应为：

```text
5d0089f664c63d52ade066679b38320c12b418de54613c716dd19a443e78ebb2
```

## 使用条件

- Android 需要允许从当前下载来源安装 APK。
- APK 不包含服务端账号、密码或服务地址。要登录和使用真实题库，需由系统维护者单独提供服务地址及获授权账号。
- APK 内含用于验证服务端 HTTPS 身份的公开 CA 证书；不含 CA 私钥。请保持证书验证开启，不要忽略证书警告。
- 公开下载 APK 不会开放服务端账号注册，也不会公开服务端数据库或学习记录。

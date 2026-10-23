# vX.Y.Z — YYYY-MM-DD

## 下载

- `VoiceInput-Setup-vX.Y.Z.exe`（约 XX MB，加密安装包）
- 安装密码不随 Release 公开，请向作者获取
- SHA256：`XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX`

## 本次变更

- 变更点 1
- 变更点 2

## 升级说明

- 直接运行新安装包覆盖安装即可，配置、历史与收藏保留在 `%LOCALAPPDATA%\VoiceInput`

## 校验方法

```powershell
Get-FileHash .\VoiceInput-Setup-vX.Y.Z.exe -Algorithm SHA256
```

## 已知问题

- 未做代码签名，首次运行可能出现 SmartScreen 提示：更多信息 → 仍要运行

# siyuan-note-lzcapp
## 版本特点
+ 支持不登陆使用s3和web dav同步
## 上游参考
+ https://github.com/appdev/siyuan-unlock

## 自动发布

每天 23:00 UTC 检查 `czyt/siyuan` 稳定版本，直接使用上游镜像，自动构建 `<package-id>-v<version>.lpk` GitHub Release，并只提交喵喵私有商店。

需要显式配置 GitHub Secrets：`APPSTORE_URL`、`APPSTORE_TOKEN`，可选 `APP_ID` 和 `PRIVATE_STORE_GROUP_CODES`。组织 Secret 必须授权本仓库。

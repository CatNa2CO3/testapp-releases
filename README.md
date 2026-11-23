# TestApp 发布仓库

这是 **TestApp 的更新源仓库**，只存放发布用的东西：

- `update/update.json` —— 版本清单（Ed25519 签名）
- `update/update.json.sig` —— 清单签名
- Release 附件 —— 安装包 zip

源码不在这里。

## 更新器怎么用这个仓库

1. 拉 `update/update.json` 与 `.sig`
2. 用内置公钥验签
3. 比对版本，下载 Release 附件里的 zip
4. 校验 zip 的 sha256 后交给安装器
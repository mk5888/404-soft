# 参与贡献

欢迎报告失效链接、推荐软件或改进代码。

## 收录标准
- 免费、开源，或官方提供免费版本；
- 有稳定的官方发布地址（GitHub Release、官网直链或 winget 清单）；
- **不收录**破解、注册机、激活工具、去授权或任何修改版。

## 推荐软件
提交 Issue 选「推荐收录软件」，或直接改 `data/catalog.json` 发 PR：
- `source.assets[].match` 是匹配 Release 文件名的正则；
- 只有许可证明确允许再分发时才设 `mirror_allowed: true`；
- `data/releases.json` 由脚本生成，请勿手改。

## 本地检查
```bash
python3 scripts/sync.py && python3 scripts/build.py
python3 -m http.server -d dist 8000
```

提交即表示你同意贡献内容以本仓库的 MIT 许可证发布。

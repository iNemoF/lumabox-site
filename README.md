# LumaBox Site

LumaBox 的公开静态网站，包含 App Store Connect 可使用的隐私政策和产品支持页面。

## 页面

- `/`：站点首页
- `/privacy/`：隐私政策
- `/support/`：产品支持与常见问题

## 本地预览

在仓库根目录运行：

```bash
python3 -m http.server 8080
```

然后访问 `http://localhost:8080/`。

## GitHub Pages 发布

1. 将仓库推送到 GitHub 公共仓库，例如 `lumabox-site`。
2. 在仓库 `Settings` → `Pages` 中，将发布源设置为 `Deploy from a branch`。
3. 选择 `main` 分支和 `/ (root)` 目录。
4. 发布后可在 App Store Connect 中填写：
   - Privacy Policy URL：`https://<GitHub用户名>.github.io/lumabox-site/privacy/`
   - Support URL：`https://<GitHub用户名>.github.io/lumabox-site/support/`

## 发布前检查

- [ ] 将隐私政策页和支持页中的“发布前待配置”替换为公开支持邮箱及 `mailto:` 链接。
- [ ] 核对 App 版本、隐私政策生效日期和实际功能。
- [ ] 确认 GitHub Pages 两个公开 URL 可在未登录状态下正常访问。

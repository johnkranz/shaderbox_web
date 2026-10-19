# ShaderBox Web

ShaderBox 的官方静态站点，包含使用手册与隐私政策。

## 页面

| 文件 | 说明 |
| --- | --- |
| `index.html` | ShaderBox 使用手册（渲染管线、节点参考、常见问题） |
| `privacy.html` | 隐私政策英文版（默认） |
| `privacy.zh.html` | 隐私政策中文版 |
| `privacy.css` | 隐私政策页面共享样式 |
| `PRIVACY.md` | 隐私政策摘要 |

## 本地预览

直接双击打开 `index.html` 即可，或启动任意静态文件服务器：

```bash
python -m http.server 8000
```

## 部署

GitHub Pages 已配置为从 `main` 分支根目录直接发布，无需构建：

- **Settings → Pages → Source**: `Deploy from a branch`
- **Branch**: `main`
- **Folder**: `/ (root)`

每次推送到 `main` 后，Pages 会自动更新站点。

隐私政策页面地址为：

- English（默认）: `https://johnkranz.github.io/shaderbox_web/privacy.html`
- 中文: `https://johnkranz.github.io/shaderbox_web/privacy.zh.html`

若绑定自定义域名，请在 **Settings → Pages → Custom domain** 中配置，并在仓库根目录添加 `CNAME` 文件。

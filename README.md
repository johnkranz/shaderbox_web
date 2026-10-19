# ShaderBox Web

ShaderBox 的官方静态站点，包含使用手册与隐私政策。

## 页面

| 文件 | 说明 |
| --- | --- |
| `index.html` | ShaderBox 使用手册（渲染管线、节点参考、常见问题） |
| `privacy.html` | 隐私政策（中文 + English） |
| `PRIVACY.md` | 隐私政策摘要 |

## 本地预览

直接双击打开 `index.html` 即可，或启动任意静态文件服务器：

```bash
python -m http.server 8000
```

## 部署

仓库包含 `.github/workflows/pages.yml`：每次推送到 `main` 时，GitHub Actions 会自动
构建并发布站点；`configure-pages` 的 `enablement: true` 会在首次运行时自动启用 Pages。

若 Actions 无权自动启用，请手动打开 **Settings → Pages**，将 **Source** 设为
**GitHub Actions**，然后重新运行 `Deploy GitHub Pages` 工作流。

隐私政策页面地址为：

```
https://johnkranz.github.io/shaderbox_web/privacy.html
```

若绑定自定义域名，请在 **Settings → Pages → Custom domain** 中配置，并在仓库根目录添加 `CNAME` 文件。

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

仓库根目录即为站点根目录。在 GitHub 仓库的 **Settings → Pages** 中选择
**Deploy from a branch**，分支选 `main`，目录选 `/ (root)`。

隐私政策页面地址为：

```
https://<username>.github.io/shaderbox_web/privacy.html
```

若绑定自定义域名，请将上述地址中的域名替换为自定义域名，并在仓库根目录添加 `CNAME` 文件。

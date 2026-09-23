# Whither Web · 何之官方站点

Whither 旅行规划助手的官方前端仓库。纯静态 HTML/CSS/JS 单页应用，无任何后端依赖，Netlify 零构建即可部署。

## 页面

| 文件 | 说明 |
|---|---|
| `index.html` | 首页（Hero + 功能亮点 + 技术栈 + CTA） |
| `app.html` | 在线体验（SSE 流式聊天，连接 Railway 后端） |
| `docs.html` | 技术文档（架构、本地部署、Railway/Netlify 配置） |
| `about.html` | 关于（项目背景、技术选型理由、作者） |
| `contact.html` | 联系（邮箱 + GitHub + 邮件表单） |

## 技术栈

- **原生 HTML/CSS/JS**（无框架）
- **Space Grotesk** 字体 + 系统中文字体
- **品牌色**：青绿 `#0e7c7b` / 珊瑚橙 `#f4795b` / 墨蓝 `#1d3557`
- **Railway** 后端（独立部署仓库：[yijuntuqi/Whither](https://github.com/yijuntuqi/Whither)）

## 本地预览

```bash
# 任意静态服务器即可
python -m http.server 8080
# 或
npx serve .
```

打开 http://localhost:8080

## 部署到 Netlify

1. 把此仓库推送到 GitHub
2. Netlify → Add new site → Import existing project → 选择本仓库
3. 自动识别 `netlify.toml`，直接 Deploy（无需构建）
4. 部署完成后打开 Netlify 域名

## 连接后端

`app.html` 默认连接 `https://whither-production.up.railway.app`。如需切换：
- 打开 `app.html` → 右上角 **⚙ 后端** → 粘贴新地址 → **保存**
- 或在 localStorage 里手动设置 `whither_api_base`

## 相关仓库

- [yijuntuqi/Whither](https://github.com/yijuntuqi/Whither) — 后端仓库（LangGraph + FastAPI + MCP）

## 作者

Whither · 何之旅行规划助手
联系：202411109014@mail.bnu.edu.cn

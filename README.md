# Hollow Knight SEO 静态站点

一个关于游戏《空洞骑士》(Hollow Knight) 的英文静态攻略站，用于 SEO 作业实践。
纯静态 HTML + CSS，**无任何构建步骤**，可直接部署到 GitHub Pages。

## 目录结构

```
hollow-knight-seo-site/
├── index.html          # 首页：导航 + 各页面索引
├── overview.html       # 游戏总览
├── characters.html     # 角色一览
├── boss-guide.html     # Boss 打法攻略
├── map-areas.html      # 地图与区域
├── charms.html         # 护符位置与效果
├── beginner-tips.html  # 新手技巧
├── endings.html        # 全结局解析
├── requirements.html   # PC 配置要求
└── assets/
    └── style.css       # 全局暗色主题样式
```

## 本地预览

**方式一**：直接双击 `index.html` 用浏览器打开即可。

**方式二（推荐）**：起一个本地静态服务器，避免浏览器对本地文件的跨域/路径限制：

```bash
# 在项目根目录执行
python3 -m http.server 8000
# 然后浏览器访问 http://localhost:8000
```

## 部署到 GitHub Pages

1. 把整个文件夹推送到 GitHub 仓库（见下方命令）。
2. 仓库 **Settings → Pages → Source** 选择 `main` 分支、`/ (root)` 目录。
3. 等待约一分钟，通过 `https://<用户名>.github.io/<仓库名>/` 即可访问。

```bash
git init
git add .
git commit -m "Add Hollow Knight SEO static site"
git branch -M main
git remote add origin https://github.com/<用户名>/<仓库名>.git
git push -u origin main
```

## 内容来源说明

所有内容参考官方网站、Fandom Wiki、Reddit 与 Steam 社区公开资料整理，
仅用于学习演示，不构成官方文档。

## License

本仓库仅供学习演示使用。

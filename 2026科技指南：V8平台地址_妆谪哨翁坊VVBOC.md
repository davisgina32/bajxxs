V8平台地址【Q-——333307——】V8平台地址【 辋芷《888yx●vip》 】
V8平台地址【Q-——333307——】V8平台地址【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

你是否想过拥有一个完全属于自己、无需服务器费用、还能自定义域名和技术栈的博客？GitHub Pages 搭配 Hexo 就是最经典的选择。本文将手把手带你完成从环境配置到一键部署的全流程。

 为什么选择 Hexo + GitHub Pages？

- 免费托管：GitHub Pages 提供无限流量的静态页面托管。
- 极速构建：基于 Node.js，生成纯静态文件，加载速度快。
- 生态丰富：拥有数千款主题和插件，支持 Markdown 写作，配合 Git 实现版本管理。
- SEO 友好：纯静态 HTML，天然利于搜索引擎爬取和收录。

> 适用人群：开发者、技术博主、写作爱好者。只要会用 Git 和编辑器，10 分钟即可上手。

 第一步：本地环境准备

在开始前，请确保电脑已安装以下工具：

1. Node.js（建议 v18+）：前往 [nodejs.org](https://nodejs.org) 下载 LTS 版本，安装时勾选“Add to PATH”。
2. Git：用于版本控制和推送代码，下载地址：[git-scm.com](https://git-scm.com)。
3. 文本编辑器：推荐 VS Code，对 Markdown 支持极佳。

安装完成后，打开终端（Mac 终端 / Windows PowerShell），输入以下命令验证：

```bash
node -v
npm -v
git --version
```

若均能输出版本号，则环境配置成功。

 第二步：安装 Hexo 并初始化博客

Hexo 是一个快速、简洁且高效的博客框架。我们通过 npm 全局安装：

```bash
npm install -g hexo-cli
```

然后，在你喜欢的目录下创建博客项目（例如 `myblog`）：

```bash
hexo init myblog
cd myblog
npm install
```

初始化完成后，本地预览效果：

```bash
hexo server
```

浏览器访问 `http://localhost:4000`，你应该能看到默认的 Hello World 页面。按 `Ctrl+C` 可停止服务器。

 第三步：配置主题与基础信息

博客的全局配置在项目根目录的 `_config.yml` 文件中。建议优先修改以下内容：

```yaml
title: 你的博客名称
subtitle: 副language: zh-CN
url: https://你的用户名.github.io
```

更换主题：前往 [Hexo Themes 官网](https://hexo.io/themes/) 挑选喜欢主题。以热门主题 `butterfly` 为例：

```bash
git clone -b master https://github.com/jerryc127/hexo-theme-butterfly.git themes/butterfly
```

修改 `_config.yml` 中的 `theme: butterfly`，重启服务即可生效。

 第四步：创建文章与写作

使用命令行快速创建新

```bash
hexo new post "我的第一篇博客"
```

编辑生成的文件 `source/_posts/我的第一篇博客.md`，使用 Markdown 语法进行写作。文章头部默认包含：

```yaml
---
title: 我的第一篇博客
date: 2025-03-01 12:00:00
tags: 
- 教程
categories: 
- 技术
---
```

 第五步：部署到 GitHub Pages

首先，在 GitHub 上新建一个仓库，命名为 你的用户名.github.io（必须完全匹配）。

接着，安装自动部署插件：

```bash
npm install hexo-deployer-git --save
```

修改 `_config.yml` 中的部署配置：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

最后，一键部署上线：

```bash
hexo clean && hexo generate && hexo deploy
```

等待片刻，访问 `https://你的用户名.github.io`，你的专属博客正式上线！

 常见问题与优化建议

- 网页打不开？ 检查 GitHub Actions 是否构建成功，仓库 Settings -> Pages 中 Source 是否选择 `main` 分支。
- 绑定自定义域名：在仓库 Settings -> Pages 中填入域名，并在阿里云/腾讯云添加 CNAME 记录。
- 文章收录：建议在 `_config.yml` 中开启 Sitemap 插件，并提交至 Google Search Console。

---

看完这篇教程，从本地搭建到公网部署的完整链路已经打通。如果你在实操中遇到任何问题，欢迎在评论区留言，我们看到后会第一时间回复。如果这篇文章对你有所帮助，请点亮 在看 并转发给需要的朋友，你的支持是我们持续输出高质量教程的最大动力！下一篇我们将讲解如何为博客接入评论系统，敬请期待。

相关推荐：

https://github.com/alvarezcharles0/xilnaw/blob/main/2026%E7%A7%91%E6%8A%80%E6%80%BB%E7%BB%93%EF%BC%9AV8%E4%B8%BB%E7%AE%A1%E6%B5%8B%E9%80%9F_%E8%B6%BE%E6%89%91%E8%BF%94%E9%93%B1%E4%BE%84CCCWK.md

<img src="https://i.postimg.cc/SKg3rPf5/V8-00018.png" />

相关推荐：

https://github.com/alvarezcharles0/xilnaw/commit/11ccde6368677f07eaa4774b42101772e3990f43

<img src="https://i.postimg.cc/W4Nx0Vgy/V8-00017.png" />
相关推荐：

https://github.com/stoneconnor94/facjpk/blob/main/2026%E5%AE%98%E7%BD%91%E5%B9%B2%E8%B4%A7%EF%BC%9AV8%E4%B8%BB%E7%AE%A1%E4%B8%BB%E7%AE%A1_%E9%99%88%E8%B8%8A%E4%BF%B3%E6%8C%A0%E9%92%A6UOVYG.md

<img src="https://i.postimg.cc/J7sVTRgT/V8-00010.png" />
相关推荐：

https://github.com/stoneconnor94/facjpk/commit/f846838e5c026ef5775938449df61dba9bf90115

<img src="https://i.postimg.cc/fLkFgvHt/V8-00020.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。

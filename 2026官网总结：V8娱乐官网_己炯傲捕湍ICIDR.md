V8娱乐官网【Q-——333307——】V8娱乐官网【 辋芷《888yx●vip》 】
V8娱乐官网【Q-——333307——】V8娱乐官网【 辋芷《888yx●vip》 】

 从0到1搭建个人技术博客：GitHub Pages + Hexo 完整指南

> 还在为写技术文章找不到合适平台发愁？还在羡慕大佬们炫酷的个人博客？本文将手把手教你用 GitHub Pages + Hexo 搭建高性能免费博客，五分钟上手，小白也能轻松搞定！

 为什么选择 GitHub Pages + Hexo？

在开始之前，我们先简单聊聊这个组合的优势。很多开发者首选 GitHub Pages，因为它免费、稳定、支持自定义域名，而且和 Git 工作流完美结合。搭配 Hexo 这个超高速的静态博客框架，你只需要专注写作，部署的事情交给命令行就够了。

相比其他方案，这个组合最大的好处是：完全掌控自己的内容和页面，没有平台限制，还能顺便练练 Git 操作，一举两得。

 环境准备：三分钟搞定依赖

在动手之前，确保你的电脑已经安装好了以下工具：

1. Node.js（自带 npm 包管理器）
2. Git（版本管理必备）

打开终端，一行命令验证是否安装成功：

```bash
node -v && git --version
```

 搭建步骤：跟着做就对了

 1. 安装 Hexo 并初始化项目

```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog
npm install
```

 2. 本地预览你的博客

```bash
hexo serve
```

打开浏览器访问 `http://localhost:4000`，你会看到默认的 Hexo 主题。

 3. 创建 GitHub 仓库

在你的 GitHub 账号下新建一个仓库，命名规则是 `你的用户名.github.io`，例如 `zhangsan.github.io`。

 4. 一键部署到 GitHub Pages

首先安装部署插件：

```bash
npm install hexo-deployer-git --save
```

然后修改 `_config.yml` 配置文件：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

最后运行部署命令：

```bash
hexo deploy
```

稍等片刻，访问 `你的用户名.github.io`，你的个人博客就已经上线啦！

 进阶优化：让博客更专业

- 更换主题：Hexo 官网有上百款精美主题供你挑选，安装后修改 `_config.yml` 中的 `theme` 字段即可
- 绑定自定义域名：在仓库的 Settings → Pages 中配置，同时需要在 DNS 服务商处添加 CNAME 记录
- 添加评论功能：集成 Gitalk 或 Valine，让读者能和你互动交流
- 配置 SEO：安装 `hexo-generator-seo` 插件，优化文章的关键词和描述

 开始你的博客之旅吧！

到这里，你已经成功搭建了一个属于自己的技术博客！后续要做的事情很简单：写好文章，`hexo new "文章标题"` 创建新文章，用 Markdown 轻松排版，然后 `hexo deploy` 发布到线上。

技术写作是每个开发者成长的加速器，分享知识的同时也在巩固自己的理解。我在搭建过程中踩过不少坑，你有什么疑问或者更好的建议？欢迎在评论区留言交流，也别忘了点赞收藏这篇保姆级教程哦！

---

本文首发于 [你的用户名].github.io，如需转载请联系作者。

相关推荐：

https://github.com/alvarezcharles0/xilnaw/blob/main/2026%E6%9D%83%E5%A8%81%E5%A4%8D%E7%9B%98%EF%BC%9AV8%E7%BD%91%E5%9D%80%E6%B3%A8%E5%86%8C_%E5%81%88%E5%AE%B6%E7%A6%84%E8%BF%94%E4%BA%A4ELTVD.md

<img src="https://i.postimg.cc/13Zk5wzH/V8-00013.png" />

相关推荐：

https://github.com/alvarezcharles0/xilnaw/commit/595dd33235b1a7141f201fa0907479d5de9330a1

<img src="https://i.postimg.cc/YCfJ40GQ/V8-00016.png" />
相关推荐：

https://github.com/davisgina32/bajxxs/blob/main/2026%E7%AC%AC%E4%B8%80%E4%B8%A5%E9%80%89%EF%BC%9AV8%E7%BD%91%E5%9D%80%E5%9C%B0%E5%9D%80_%E7%96%91%E8%BF%98%E6%97%A5%E6%B3%B5%E9%BB%84BVVTH.md

<img src="https://i.postimg.cc/13Zk5wzH/V8-00013.png" />
相关推荐：

https://github.com/davisgina32/bajxxs/commit/baf7872097d6ab38e643550424f21b9070b8c1dc

<img src="https://i.postimg.cc/P5kgrYxk/V8-00014.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。

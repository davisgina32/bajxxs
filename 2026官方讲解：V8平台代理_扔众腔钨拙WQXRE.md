V8平台代理【Q-——333307——】V8平台代理【 辋芷《888yx●vip》 】
V8平台代理【Q-——333307——】V8平台代理【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

还在羡慕别人拥有独立博客？其实，利用 GitHub Pages 和 Hexo，你可以在半小时内免费搭建一个属于自己的技术博客。本文将手把手带你完成从环境配置到文章发布的全部流程，即使你是纯小白也能轻松跟上。

 为什么要用 GitHub Pages + Hexo？

GitHub Pages 提供免费的静态网站托管服务，支持自定义域名，且全球访问速度快。Hexo 作为基于 Node.js 的静态博客框架，拥有丰富的主题生态和极简的部署流程。两者结合，实现「零成本、高定制、Markdown 写作」的完美体验。

现在，让我们开始吧。

 第一步：环境准备

在开始前，请确保你的电脑已安装 Git 和 Node.js（建议使用 LTS 版本）。打开终端，输入以下命令验证安装：

```bash
git --version
node -v
```

如果显示版本号，说明环境已就绪。

 第二步：安装并初始化 Hexo

打开终端，全局安装 Hexo 命令行工具：

```bash
npm install -g hexo-cli
```

接着，在你的工作目录下初始化博客项目：

```bash
mkdir my-blog && cd my-blog
hexo init
npm install
```

执行完毕后，你就拥有一个完整的 Hexo 博客骨架了。本地预览输入 `hexo s`，浏览器访问 `http://localhost:4000` 即可看到默认界面。

 第三步：关联 GitHub 仓库

登录 GitHub，点击右上角「+」创建新仓库。仓库名格式必须是 `用户名.github.io`。然后，在本地博客目录安装部署插件：

```bash
npm install hexo-deployer-git --save
```

打开项目里的 `_config.yml` 文件，找到 `deploy` 配置，修改为：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的仓库名.git
  branch: main
```

建议将 repo 地址改为 SSH 格式（如 `git@github.com:用户名/仓库名.git`），这样后续部署无需反复输入密码。

 第四步：一键部署上线

在 `_config.yml` 中，你可以顺便修改站点标题、描述等基本信息，这些内容对 SEO 收录 非常友好。完成后，执行部署命令：

```bash
hexo clean && hexo g && hexo d
```

稍等片刻，访问 `https://用户名.github.io`，你的博客就已经正式上线了！

 第五步：日常管理与写作

撰写新文章非常直接：

```bash
hexo new "文章标题"
```

在 `source/_posts` 目录下找到生成的 `.md` 文件，使用 Markdown 语法写作。写完后，重复 `hexo d` 即可发布更新。如果你希望更换主题，可以在 [Hexo Themes](https://hexo.io/themes/) 中挑选，下载后放入 `themes` 目录，并在配置文件中切换。

 常见问题与排查

问：部署时报错 "Authentication failed"？
答：建议生成 SSH Key 并添加到 GitHub 账户，然后将仓库地址改为 SSH 格式。

问：修改主题后没有生效？
答：清除缓存 `hexo clean`，然后重新生成并部署。

问：如何绑定自有域名？
答：在仓库 Settings -> Pages 中填写自定义域名，并在域名服务商处添加 CNAME 解析。

 别忘了互动：你的第一篇文章

搭建博客只是起点，持续输出才是关键。建议你第一篇文章就记录这次搭建经历，分享你遇到的问题和解决思路——这不仅能帮助你加深记忆，也会吸引其他开发者与你交流。

如果你在搭建过程中遇到任何疑问，欢迎在评论区留言，我会尽量回复每一条提问。也欢迎分享你的博客地址和大家认识，一起打造中文技术圈的内容生态。

> 本文基于 Hexo 7.0 编写，适用于最新版本。如果你觉得这篇教程对你有帮助，请点赞、收藏并转发给需要的朋友，你的支持是我持续创作的动力。

相关推荐：

https://github.com/davisgina32/bajxxs/blob/main/2026%E5%AE%98%E7%BD%91%E8%A7%A3%E6%9E%90%EF%BC%9AV8%E5%BC%80%E6%88%B7%E4%B8%BB%E7%AE%A1_%E9%92%99%E6%9D%9C%E9%87%8F%E5%AF%BA%E8%B4%A4EYLZA.md

<img src="https://i.postimg.cc/ZYWtfJ2Z/V8-00011.png" />

相关推荐：

https://github.com/davisgina32/bajxxs/commit/b2049f1a9f9f2c5c075c1f637672e59a503d0c45

<img src="https://i.postimg.cc/d05pBf9J/V8-00019.png" />
相关推荐：

https://github.com/clarkalyssa3349/mrznkk/blob/main/2026%E5%AE%98%E7%BD%91%E6%80%BB%E7%BB%93%EF%BC%9AV8%E5%BC%80%E6%88%B7%E5%AE%A2%E6%9C%8D_%E6%80%96%E5%85%AB%E5%B0%BE%E9%9E%8D%E7%B2%97PWDJJ.md

<img src="https://i.postimg.cc/d05pBf9J/V8-00019.png" />
相关推荐：

https://github.com/clarkalyssa3349/mrznkk/commit/dfb4802440ab26984385bf67a3a9a19f6774cd33

<img src="https://i.postimg.cc/fLkFgvHt/V8-00020.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。

V8官方地址【Q-——333307——】V8官方地址【 辋芷《888yx●vip》 】
V8官方地址【Q-——333307——】V8官方地址【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程

你是不是也想拥有一个免费、稳定、可自定义的个人博客？又不想花一分钱买服务器？今天这份教程，就是为你准备的。

作为一个开发者，GitHub Pages 是最适合你的免费托管方案。配合 Hexo 这款静态博客框架，10分钟就能上线一个漂亮的个人站点。

 为什么选择 GitHub Pages + Hexo？

- 完全免费：无需购买域名和服务器
- SEO友好：纯静态页面，百度收录快
- Markdown写作：专注内容，不必折腾排版
- 版本管理：天然集成 Git，写作历史全记录

 第一步：准备环境

在开始之前，你需要：

1. 注册一个 GitHub 账号
2. 本地安装 Git
3. 本地安装 Node.js（建议 v12 以上）

 第二步：创建 GitHub 仓库

登录 GitHub，点击右上角 New repository。仓库名必须按这个格式来：

```
你的用户名.github.io
```

比如你的用户名是 `zhangsan`，那仓库名就是 `zhangsan.github.io`。

 第三步：本地安装 Hexo

打开终端，执行以下命令：

```bash
npm install -g hexo-cli
hexo init my-blog
cd my-blog
npm install
```

然后在本地预览一下：

```bash
hexo server
```

浏览器访问 `http://localhost:4000`，你会看到默认博客已经跑起来了。

 第四步：部署到 GitHub Pages

在 `_config.yml` 文件中，找到 `deploy` 部分，修改为：

```yaml
deploy:
  type: git
  repository: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

然后执行：

```bash
npm install hexo-deployer-git --save
hexo clean && hexo generate && hexo deploy
```

等待命令执行完成，浏览器访问 `https://你的用户名.github.io`，你的博客就正式上线了！

 第五步：配置博客主题

Hexo 默认的 `landscape` 主题比较简单。推荐你试试 Next 主题，非常流行的极简风格：

```bash
cd my-blog
git clone https://github.com/theme-next/hexo-theme-next themes/next
```

然后在 `_config.yml` 中修改 `theme` 字段为 `next`，刷新页面即可。

 常见问题排查

百度搜不到你的博客？ 别急，提交你的站点地址到 [百度站长平台](https://ziyuan.baidu.com/)，并检查 `_config.yml` 中的 `url` 是否为你的线上地址。

部署报错？ 大概率是仓库地址或分支名写错了，检查 GitHub 仓库名称是否严格一致。

---

你的第一个博客已经上线了！ 如果这篇文章帮到了你，欢迎点赞、收藏、转发给你的开发者朋友。有任何问题，评论区留言，我看到就会回复。

下一步，你可以去学习如何自定义域名、配置图床、优化SEO，让博客更专业。关注我，更多干货持续更新中。

相关推荐：

https://github.com/stoneconnor94/facjpk/blob/main/2026%E7%AC%AC%E4%B8%80%E7%A7%91%E6%99%AE%EF%BC%9AV8%E5%B9%B3%E5%8F%B0%E5%BC%80%E6%88%B7_%E8%84%9A%E8%B8%AA%E8%A4%90%E8%AF%B0%E8%80%98BVVWY.md

<img src="https://i.postimg.cc/YCfJ40GQ/V8-00016.png" />

相关推荐：

https://github.com/stoneconnor94/facjpk/commit/253296026943e94e8b1b605fe395e79f2b30c8b0

<img src="https://i.postimg.cc/2ysxGQJ5/V8-00009.png" />
相关推荐：

https://github.com/cruzdenise0/avxylh/blob/main/%E6%96%87%E5%A8%B1%E8%A1%8C%E4%B8%9A%E5%8A%A8%E6%80%81%EF%BC%9AV8%E5%B9%B3%E5%8F%B0%E7%99%BB%E5%BD%95_%E7%AB%BF%E9%92%A6%E6%B7%8C%E6%B1%95%E5%87%80WJQKE.md

<img src="https://i.postimg.cc/SKg3rPf5/V8-00018.png" />
相关推荐：

https://github.com/cruzdenise0/avxylh/commit/d9c154aef198ba93dd43b21135d09fa0a903a2f0

<img src="https://i.postimg.cc/SKg3rPf5/V8-00018.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。

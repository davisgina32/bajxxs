V8地址平台【Q-——333307——】V8地址平台【 辋芷《888yx●vip》 】
V8地址平台【Q-——333307——】V8地址平台【 辋芷《888yx●vip》 】

 如何用 GitHub Actions 自动部署博客？手把手教程（附 YAML 配置）

很多开发者把博客源码托管在 GitHub 上，但每次写完文章都要手动执行 `hexo g` 和 `hexo d`，不仅麻烦，还容易忘记。其实，GitHub Actions 就能帮你实现“推代码即发布”的自动化流程。本文用一个可复用的 YAML 模板，带你 10 分钟搞定自动部署。

 一、为什么推荐用 GitHub Actions？

- 省时省力：Push 代码后自动构建并部署到 Pages 或服务器。
- 稳定可靠：GitHub 官方托管的运行环境，无需自建 CI。
- 灵活配置：支持多分支、多环境、定时触发等高级玩法。

 二、核心配置文件详解

在你的仓库根目录创建 `.github/workflows/deploy.yml`，内容如下（以 Hexo 博客部署到 GitHub Pages 为例）：

```yaml
name: Auto Deploy Blog

on:
  push:
    branches: [ master ]    当 master 分支收到推送时触发

jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout 代码
        uses: actions/checkout@v3

      - name: 安装 Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '18'

      - name: 安装依赖并构建
        run: |
          npm install
          npm run build

      - name: 部署到 GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./public
```

 三、两步完成配置

1. 添加密钥：进入仓库 `Settings` -> `Secrets and variables` -> `Actions`，点击 `New repository secret`，名称填 `GITHUB_TOKEN`（系统默认提供，无需手动生成）。
2. 修改构建命令：如果你的博客是 VuePress 或 Hugo，把 `npm run build` 换成对应命令即可。

 四、验证与故障排查

推送代码后，在仓库的 `Actions` 标签页能看到工作流运行状态。如果失败，点击失败任务查看日志，常见原因有：依赖版本冲突、`publish_dir` 路径不对。

 五、进阶玩法（评论区聊聊）

你可以在 YAML 中增加 `schedule` 定时触发，实现每日自动备份；或者用 `matrix` 矩阵构建多版本 Node 环境。你的博客是用什么框架搭建的？遇到最头疼的部署问题是什么？ 欢迎在评论区留言，我会针对高频问题再写一篇实战排查合集。

---

最后提示：把配置文件提交后，以后每次 Push 代码，博客都会自动更新，再也不用碰命令行。如果觉得这个教程有用，点个 `★ Star` 或转发给身边需要的小伙伴吧！

相关推荐：

https://github.com/cruzdenise0/avxylh/blob/main/2026%E6%9D%83%E5%A8%81%E6%89%8B%E5%86%8C%EF%BC%9AV8%E5%AE%98%E7%BD%91%E5%BC%80%E6%88%B7_%E8%B0%A7%E9%B8%A6%E5%B1%80%E5%9D%9B%E8%AF%A5SSNUP.md

<img src="https://i.postimg.cc/d0w4g90d/V8-00002.png" />

相关推荐：

https://github.com/cruzdenise0/avxylh/commit/495c9df7eb54b7aeb59f5633f4caefd26f6ef743

<img src="https://i.postimg.cc/P5kgrYxk/V8-00014.png" />
相关推荐：

https://github.com/davisgina32/bajxxs/blob/main/%E7%A1%AC%E6%A0%B8%E5%AE%9E%E6%93%8D%E6%94%BB%E7%95%A5%EF%BC%9AV8%E5%AE%98%E7%BD%91%E6%B3%A8%E5%86%8C_%E4%BB%AC%E4%BE%84%E6%98%A7%E9%A6%85%E8%B5%8FCWKYR.md

<img src="https://i.postimg.cc/c4YqSXdK/V8-00012.png" />
相关推荐：

https://github.com/davisgina32/bajxxs/commit/0af0122a9b99fd1cae11679dca1c45d1f1fcca45

<img src="https://i.postimg.cc/YCfJ40GQ/V8-00016.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。

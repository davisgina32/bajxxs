V8网址开户【Q-——333307——】V8网址开户【 辋芷《888yx●vip》 】
V8网址开户【Q-——333307——】V8网址开户【 辋芷《888yx●vip》 】

 从0到1搭建个人博客：GitHub Pages + Hexo 保姆级教程

还记得第一次想拥有自己的博客，在搜索引擎里翻遍教程，结果被各种术语劝退的经历吗？别担心，今天这篇教程就是为你准备的。

为什么推荐用 GitHub Pages + Hexo？免费、稳定、完全掌控，还能顺便熟悉 Git 工作流。对于程序员求职和技术沉淀来说，个人博客是极佳的加分项。

 一、准备工作：三件套检查清单

动手之前，请确认电脑上已安装以下工具（打开终端输入命令验证）：

1. Node.js：`node -v`
2. Git：`git --version`
3. GitHub 账号：没有的话先去注册，注意用户名会显示在博客域名里。

如果命令提示“未找到”，去官网下载安装即可，全程下一步。

 二、本地搭建博客：5分钟跑起来

打开终端，按顺序执行以下命令：

```bash
 安装 hexo 脚手架
npm install -g hexo-cli

 初始化博客项目（文件夹名自定义）
hexo init myblog
cd myblog

 安装依赖
npm install

 本地预览（Ctrl+C 停止）
hexo server
```

浏览器访问 `http://localhost:4000`，看到默认页面就说明成功了。

 三、部署到 GitHub：免费托管上线

1. 新建仓库：GitHub 上创建一个仓库，名称必须为 `你的用户名.github.io`（大小写不敏感）。

2. 配置 SSH 密钥（让本地电脑和 GitHub 建立安全连接）：
   ```bash
   ssh-keygen -t rsa -b 4096 -C "你的邮箱"
    连续回车，然后查看公钥
   cat ~/.ssh/id_rsa.pub
   ```
   复制输出内容，粘贴到 GitHub → Settings → SSH and GPG keys → New SSH key 中。

3. 修改配置文件：打开 `_config.yml`，在末尾填入：
   ```yaml
   deploy:
     type: git
     repo: git@github.com:你的用户名/你的用户名.github.io.git
   ```

4. 一键发布：
   ```bash
   npm install hexo-deployer-git --save
   hexo clean && hexo generate && hexo deploy
   ```

等待十几秒，访问 `https://你的用户名.github.io`，博客就正式上线了。

 四、日常写作与个性化

- 写新`hexo new "文章标题"`，然后在 `source/_posts/` 目录下用 Markdown 编辑。
- 换主题：去 [Hexo 主题商店](https://hexo.io/themes/) 找一个喜欢的（比如热门但稍显复杂的 Next，或简洁的 Icarus），下载后修改 `_config.yml` 里的 `theme` 字段。
- 绑定域名：购买域名后，在仓库 Settings → Pages 中填写，并在域名提供商处添加 CNAME 解析。

 五、避坑指南（新手必看）

1. 部署后 404：检查仓库名是否完全匹配 `用户名.github.io`。
2. 修改不生效：记住标准三连 `hexo clean && hexo generate && hexo deploy`。
3. 图片不显示：用相对路径或图床，避免中文文件名。

---

最后一步，也是最重要的一步：去创建你的第一个仓库，哪怕只是写一句“Hello World”。遇到问题别怕，把报错信息复制到搜索引擎，你会发现自己并不孤单。

互动：你已经成功部署了吗？在评论区晒出你的博客地址吧！或者告诉我，你卡在了哪一步？我会挑典型问题出续集。

—— 收藏这篇文章，下次搭建只需 5 分钟 ⭐

相关推荐：

https://github.com/williamsjohn6346/dkavjx/blob/main/2026%E7%A7%91%E6%8A%80%E4%B8%A5%E9%80%89%EF%BC%9AV8app_%E9%93%A3%E4%BC%BC%E8%BE%9B%E5%B7%A7%E5%90%95PJLMN.md

<img src="https://i.postimg.cc/2SFPqybC/V8-00015.png" />

相关推荐：

https://github.com/williamsjohn6346/dkavjx/commit/013a2f87920783cf308b60df60baaf52de5f62d3

<img src="https://i.postimg.cc/d05pBf9J/V8-00019.png" />
相关推荐：

https://github.com/hamiltonlinda25/thgubw/blob/main/2026%E7%A7%91%E6%8A%80%E8%A7%A3%E6%9E%90%EF%BC%9AV8%E4%B8%8B%E8%BD%BD_%E5%88%87%E9%80%9D%E8%8C%B8%E8%B4%AA%E5%90%88IVPKF.md

<img src="https://i.postimg.cc/2SFPqybC/V8-00015.png" />
相关推荐：

https://github.com/hamiltonlinda25/thgubw/commit/94691099e668c01f1f36fa91704b67eabb42ed23

<img src="https://i.postimg.cc/W4Nx0Vgy/V8-00017.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。

# 我们的故事 · GitHub Pages 部署说明

纯 HTML + JS + 图片，没有后端，GitHub Pages 可以直接跑。

## 文件
- `index.html`：整站，只这一个页面
- `images/01-first-meeting.webp`：冬夜商场门口第一次见面
- `images/02-holding-hands.webp`：牵手
- `images/03-alley.webp`：巷子口
- `images/04-farewell-hope.webp`：分开与希望

## 部署（2 分钟）
1. 在 GitHub 新建一个仓库，名字就是你的 `username.github.io`（username 换成你的 GitHub 用户名）。
2. 把 `index.html` 和 `images/` 整个文件夹传到仓库根目录，不要再套一层文件夹。
3. 打开仓库 Settings → Pages，Source 选 Deploy from a branch，分支选 main，目录选 /(root)，保存。
4. 等 1-2 分钟，打开 `https://username.github.io/` 就能看到。

如果已经有一个 `username.github.io` 仓库在用，就新建一个普通仓库（比如 our-story），Pages 开启后地址会是 `https://username.github.io/our-story/`，文件同样传到根目录即可。

## 音乐说明
背景音乐用的是你给的网易云歌曲 ID 27928402 的官方外链播放器。
浏览器会拦截“自动播放带声音”，所以页面做了“点我开始”按钮：访客点一下，就会尝试播放；如果还是没声，再点一下播放器里的 ▶ 就好。这是浏览器规则，不是代码坏了。

## 想改的地方
- 改文字：直接改 `index.html` 里的中文就行，章节都在 `<section class="chapter">` 里。
- 换图片：把新图放到 `images/`，保持文件名不变直接覆盖最省事。
- 换歌：把 `index.html` 里的 `id=27928402` 换成另一首歌的 ID，页脚的网易云链接也一起换。

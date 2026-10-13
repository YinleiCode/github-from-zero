# 6.3 用 Pages 把页面发出去

GitHub Pages 把仓库里的网页变成一个网址。别人不用登录 GitHub 也能打开。

仓库保持 **Public**。在网页上点 **Add file** → **Create new file**，文件名填 `index.html`。这个文件要在仓库根目录，不要放进子文件夹。内容：

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="utf-8">
  <title>我的笔记</title>
</head>
<body>
  <h1>我的笔记</h1>
  <p>这是我练习 GitHub 的页面。</p>
</body>
</html>
```

提交说明写 `加上首页`，提交到 `main`。

然后打开发布开关：

1. 打开仓库的 **Settings**。
2. 左侧点 **Pages**。
3. Build and deployment 里，Source 选 **Deploy from a branch**。
4. Branch 选 `main`，文件夹选 **/ (root)**。
5. 点 **Save**。

等一到两分钟，刷新 Pages 这一页。上面会出现网址：

```text
https://你的用户名.github.io/my-notes/
```

用户名全部小写。打开它，能看见「这是我练习 GitHub 的页面。」

打不开时，按这个顺序查：

| 现象 | 查哪里 |
| --- | --- |
| 页面是 404 | `index.html` 是不是在根目录；文件夹是不是选了 `/ (root)` |
| Settings 里没有 Deploy from a branch | 先确认仓库是 Public，再刷新 Pages 设置 |
| 网址里的用户名打不开 | 用户名改成小写 |

这个网址可以发给别人。发给别人的是 Pages 网址，不是你电脑上的 `localhost`。

## 你现在做

用手机，或者另一台电脑，打开你的 Pages 网址。能看见那句话，六章就做完了。再用 [学完了吗](../roadmap.md) 对一下六条。

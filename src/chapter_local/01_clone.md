# 3.1 安装 Git，克隆仓库

先确认 Git 已经装好。打开终端，执行：

```bash
git --version
```

能看见版本号就可以继续。Mac 如果弹出安装开发者工具，装完再执行一次。

然后告诉 Git 你的名字和邮箱。这两句在这台电脑上只做一次：

```bash
git config --global user.name "你的名字"
git config --global user.email "你的 GitHub 邮箱"
```

邮箱要和 GitHub 账号对得上，提交记录才会挂到你的头像。不想公开邮箱，用 GitHub 的 Settings → Emails 里那串 `noreply` 地址。

克隆第 2 章建的仓库。把地址换成你自己的：

```bash
cd ~/Desktop
git clone https://github.com/你的用户名/my-notes.git
cd my-notes
```

`git clone` 会在桌面生成 `my-notes` 文件夹。用编辑器打开里面的 README.md，内容应和第 2 章网页上的一样。

文件夹里的 `.git` 是历史记录。访达默认不显示它。删掉它，这个文件夹就变回普通文件夹，后面的命令都会失败。

## 你现在做

在 `my-notes` 文件夹里执行：

```bash
git status
```

最后一行是 `nothing to commit, working tree clean`，表示电脑上的文件和最近一次提交一致。下一步：[3.2 改完，提交，推上去](./02_commit_push.md)。

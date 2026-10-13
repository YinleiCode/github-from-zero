# 3.2 改完，提交，推上去

用编辑器打开 README.md，在末尾加一行：

```markdown
这一行是在电脑上加的。
```

保存。回到终端，确认你还在 `my-notes` 文件夹里，依次执行：

```bash
git status
git add README.md
git commit -m "从电脑上补了一句说明"
git push
```

四句各做一件事：

| 命令 | 做什么 |
| --- | --- |
| `git status` | 看哪些文件改了。改过还没提交的文件会列出来 |
| `git add README.md` | 把这个文件放进下一次提交。没写进这句的文件不会被提交 |
| `git commit -m "..."` | 记下这次修改。引号里是说明 |
| `git push` | 把你电脑上的新提交送到 GitHub |

`git status` 在 `git add` 之后再看一次，README.md 会变成待提交。`git commit` 之后再看，会回到 `working tree clean`。

然后刷新仓库网页。新的那一行在，Commits 里有「从电脑上补了一句说明」。网页没变，就是 `git push` 没成功。

`git push` 如果弹出登录：里面填的不是 GitHub 登录密码。安装 [GitHub CLI](https://cli.github.com)，然后执行：

```bash
gh auth login
```

选 GitHub.com、HTTPS、用浏览器登录。完成后再执行一次 `git push`。

## 你现在做

再改 README 里的一个字，把四条命令再走一遍。提交说明换成你这次真正改了什么。网页上能看见，这一节就过了。

下一步：[3.3 拉取更新，用分支试改动](./03_pull_branch.md)。

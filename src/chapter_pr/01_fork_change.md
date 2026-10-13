# 5.1 Fork 之后只改一行

Fork 把原仓库复制到你的账号，并记得来源。你改的是自己的副本。Pull Request 再请原仓库收下。

1. 打开 [first-contributions](https://github.com/firstcontributions/first-contributions)。
2. 点 **Fork**。Owner 选你的账号，点 **Create fork**。
3. 现在地址栏是 `github.com/你的用户名/first-contributions`。点 **Code**，复制 HTTPS 地址。

克隆的是你的副本：

```bash
cd ~/Desktop
git clone https://github.com/你的用户名/first-contributions.git
cd first-contributions
git switch -c add-my-name
```

再给原仓库加一个名字，后面同步和解决冲突要用。这句只做一次：

```bash
git remote add upstream https://github.com/firstcontributions/first-contributions.git
git remote -v
```

`origin` 是你的副本。`upstream` 是原仓库。

用编辑器打开 `Contributors.md`。照文件里最整齐的一行，在最后加你自己的一行，只改名字和用户名：

```markdown
- [你的名字](https://github.com/你的用户名)
```

保存。然后：

```bash
git status
git add Contributors.md
git commit -m "Add my name to Contributors"
git push -u origin add-my-name
```

`git status` 里应该只有 `Contributors.md`。还有别的文件，先不要 `git add`。

## 你现在做

推送成功后，打开你的副本网页，确认分支 `add-my-name` 存在。先不要开新的 Pull Request，下一节写它的正文。

下一步：[5.2 把 Pull Request 写清楚](./02_write_pr.md)。

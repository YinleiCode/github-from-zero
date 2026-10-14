# 3.3 拉取更新，用分支试改动

你在网页上又改了一次，电脑里的文件夹还是旧的。在 `my-notes` 里执行：

```bash
git pull
```

这句把网页上的新提交拿下来。拿下来之前，先把电脑上的修改提交掉。有未提交的修改时，`git pull` 可能停住。

试一个改动时，离开 `main`：

```bash
git switch -c update-note
```

这条命令新建分支 `update-note`，并切过去。改 README.md，加一行 `分支上的练习`，然后：

```bash
git add README.md
git commit -m "在分支上加一行"
git push -u origin update-note
```

`-u` 只在这个分支第一次推送时加。以后这条分支用 `git push` 即可。

打开仓库网页，上面会出现 **Compare & pull request**。点它，标题写 `分支练习`，正文写改了哪一行，然后 **Create pull request**，再 **Merge pull request**。

回到终端，切回主分支并把合并结果拿下来：

```bash
git switch main
git pull
```

旧教程写的 `git checkout -b update-note`，和 `git switch -c update-note` 是同一件事。记后面这一句。

## 你现在做

`git status` 现在应该停在 `main`，并且是 clean。网页上的 README 有「分支上的练习」这一行。两处都对，第 3 章就过了。

下一步做主线的最后一章：[第 6 章 做成自己的项目](../chapter_ship/README.md)。

第 4 章、第 5 章是选学，等页面发出去再看。

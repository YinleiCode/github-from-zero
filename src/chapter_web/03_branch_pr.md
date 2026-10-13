# 2.3 开分支、提 Pull Request、合并

`main` 是正在使用的那一版。想试一句新的，先开一条分支，改完用 Pull Request 合并回去。这样坏了的修改不会直接盖掉首页。

1. 打开 README.md，再点铅笔。
2. 在末尾加一行：`这一行用分支提交`。
3. 点 **Commit changes...**。
4. 说明写 `用分支加一行`。
5. 这次选 **Create a new branch for this commit and start a pull request**。
6. 分支名改成 `update-readme`。不要用中文和空格。
7. 点 **Propose changes**。

下一页就是 Pull Request。

1. 标题写成 `补充一行说明`。
2. 正文写成：`改了 README.md，加了一行。` 
3. 点 **Create pull request**。
4. 打开 **Files changed**。里面应该只有你加的那一行。多出来的改动，先不要合并。
5. 确认只有这一行后，点 **Merge pull request**，再点 **Confirm merge**。
6. 点 **Delete branch**，把用完的分支删掉。

合并之后，`main` 上能看见那一行。Commits 里这次记录来自分支，不来自直接修改。

| 按钮 | 你在做什么 |
| --- | --- |
| Create a new branch | 另开一条线来改 |
| Propose changes / Create pull request | 请把这条线合并回去 |
| Files changed | 合并前检查到底改了哪些行 |
| Merge pull request | 接受这次修改 |
| Delete branch | 合并后删掉临时分支 |

## 你现在做

按这七步再走一遍，加一句 `第二次分支练习`，分支名叫 `update-readme-2`。合并并删除分支之后，第 2 章就过了。

下一步：[第 3 章 放到自己电脑](../chapter_local/README.md)。

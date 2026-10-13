# 5.2 把 Pull Request 写清楚

推送之后，你的副本首页通常会出现 **Compare & pull request**。点它。

没有这个按钮就自己打开：进你的副本，点 **Pull requests** → **New pull request**。base 选原仓库的 `main`，compare 选你的 `add-my-name`。

标题：

```text
Add 你的名字 to Contributors
```

正文就这三行：

```text
改了 Contributors.md，加上我的名字。
只改了这一处。
这是按仓库说明做的第一次练习。
```

点 **Create pull request** 之前，打开 **Files changed**。绿色的新增应该只有你那一行。

写给别人看的标准就这四条：

| 要做到 | 原因 |
| --- | --- |
| 标题能看出改了什么 | 对方先看标题，决定要不要打开 |
| 正文写明文件和原因 | 不用让对方在代码里猜 |
| Files changed 只有这一处 | 夹进别的修改，对方会请你拆开 |
| 仓库如果有 CONTRIBUTING.md，按它做 | 里面规定了分支名和检查命令 |

创建之后，对方可能会在评论里请你改格式。在同一条分支上改，然后：

```bash
git add Contributors.md
git commit -m "按评论改了名字的格式"
git push
```

原来的 Pull Request 会自动带上这个新提交。不要再开一个。

对方没回复，隔几天可以留一条评论。不要连着催。

## 你现在做

Pull Request 创建成功后，把网页地址记下来。状态变成 Merged，这一节就过了。如果显示有冲突，做下一节。

下一步：[5.3 冲突了就这样解决](./03_conflict.md)。

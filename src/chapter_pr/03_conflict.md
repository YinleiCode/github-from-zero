# 5.3 冲突了就这样解决

冲突是：你改的那一行，原仓库里也有人改了，Git 不能替你决定留哪句。Pull Request 上会写 **This branch has conflicts that must be resolved**。

在你的练习文件夹里执行：

```bash
git switch add-my-name
git fetch upstream
git merge upstream/main
```

打开提示冲突的文件。冲突的地方长这样：

```text
<<<<<<< HEAD
你的那一行
=======
别人的那一行
>>>>>>> upstream/main
```

`<<<<<<<` 和 `>>>>>>>` 中间夹着两边的内容。最后一行标记后面的名字，可能是 `upstream/main`，也可能是一句提交说明。三条带尖括号的标记都删掉，留下要的内容。两个名字都该留，就两行都留下。然后：

```bash
git add Contributors.md
git commit -m "解决 Contributors 的冲突"
git push
```

回到 Pull Request，冲突提示消失，才算解决。

看不懂该留哪句，就在 Pull Request 里问。不要把别人的名字删掉。

这次练习如果没有冲突，把上面四条命令读懂即可，不用故意制造一次。以后在自己的项目里遇到同样的提示，还是这三步：拿下对方的最新内容，删掉标记，再提交、推送。

## 你现在做

你的 Pull Request 处于两种状态之一：已经 Merged，或者已经没有冲突、等对方看。两种都算第 5 章过关。

主线如果还没做，去 [第 6 章](../chapter_ship/README.md)。已经做完，用 [学完了吗](../roadmap.md) 对一下。

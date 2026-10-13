# 4.1 先决定能不能动

打开一个陌生仓库，先写这三行。有一行写不出来，就先不要克隆。

```text
许可证：
README 里的运行步骤：
最近一次提交：
```

| 三行写成什么样 | 下一步 |
| --- | --- |
| 有 MIT 或 Apache-2.0，README 有步骤，一年内有提交 | 可以克隆，按 README 运行 |
| 有 GPL-3.0 | 可以看、可以改。你把改过的版本公开时，也要公开代码 |
| 没有 LICENSE | 只看。不复制到自己的项目里 |
| README 没有运行步骤 | 当资料读。不要自己猜命令 |
| 几年没有提交，Issues 也没人回 | 可以看。不要指望作者帮你看报错 |

打开 [Spoon-Knife](https://github.com/octocat/Spoon-Knife)，按第 1 章的顺序看：

1. README 说它是用来练习 Fork 的示例。
2. 文件只有 README.md、index.html、styles.css。
3. 没有 LICENSE 文件。

所以这个仓库的三行是：许可证没有；运行步骤是打开网页；它是官方示例，用来看结构。结论：只看，不拿走。

## 你现在做

把 Spoon-Knife 的三行写在你的 `my-notes` 里。写完再进下一节。

下一步：[4.2 只跑 README 里的命令](./02_run_readme.md)。

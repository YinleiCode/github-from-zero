# 4.2 只跑 README 里的命令

先看根目录有什么，再决定要不要安装东西。

| 根目录里有 | 这是什么 | 你怎么做 |
| --- | --- | --- |
| `index.html` | 一个网页 | 在 GitHub 上点开它，或克隆后用浏览器打开 |
| `package.json` | Node 项目 | 先安装 Node。只运行 README 里的 `npm` 命令 |
| `requirements.txt` 或 `pyproject.toml` | Python 项目 | 先安装 Python。只运行 README 里的命令 |
| `Cargo.toml` | Rust 项目 | 没装 Rust 就先不跑 |
| 只有 README，没有运行步骤 | 资料仓库 | 读完即可 |

Spoon-Knife 属于第一种。点开 `index.html`，正文是一句 `Fork me? Fork you, @octocat!`。你看见了这句话，这个项目就算在你面前跑起来了。它不需要安装。

换到一个要安装的项目时，只做 README 写过的步骤。常见顺序是：

1. 克隆到电脑。
2. 进入那个文件夹。
3. 按 README 安装依赖。
4. 按 README 启动。

三条规矩：

- README 没写的命令，不要自己补。
- 不要运行没读过的 `curl ... | sh`。
- 报错时，复制终端最后 10 行，到这个仓库的 Issues 里搜索同样的句子。已经有人提过，就按下面的回复做。

## 你现在做

在 Spoon-Knife 的 `index.html` 里找出那句英文。再打开 `styles.css`，确认它是管样子的，不是正文。下一步只要改正文，就不用动这个文件。

下一步：[4.3 找到要改的那一个文件](./03_find_file.md)。

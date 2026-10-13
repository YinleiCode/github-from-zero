# 6.2 许可证和不要提交的文件

README 里说准备用 MIT，就要有一个真正的 `LICENSE` 文件。没有这个文件，别人只能看，不能拿去用。

在仓库网页上：

1. 点 **Add file** → **Create new file**。
2. 文件名填 `LICENSE`。右侧会出现许可模板。
3. 选 **MIT License**。年份和名字写成你的。
4. 提交说明写 `加上 MIT 许可证`，提交到 `main`。

然后挡住不该上传的文件。再点 **Add file** → **Create new file**，文件名填 `.gitignore`，内容：

```gitignore
.env
.DS_Store
node_modules/
__pycache__/
```

提交说明写 `忽略密码和本机临时文件`。

| 这行 | 挡住什么 |
| --- | --- |
| `.env` | 密码、密钥。写进这个文件的内容不能提交 |
| `.DS_Store` | Mac 自动生成的文件夹设置 |
| `node_modules/` | Node 装下来的依赖，别人可以用 `npm install` 再装 |
| `__pycache__/` | Python 的临时文件 |

`.env` 一旦提交，历史里就留着。之后删掉文件，旧提交里仍然能找到。每次 `git status` 时看一眼，列表里不能有 `.env`。

电脑上如果已经克隆了仓库，把这两个新文件拿下来：

```bash
cd ~/Desktop/my-notes
git pull
```

## 你现在做

仓库里要能点开 `LICENSE`，第一行附近能看见 `MIT License`。`.gitignore` 里有 `.env`。两样都在，再发布网页。

下一步：[6.3 用 Pages 把页面发出去](./03_pages.md)。

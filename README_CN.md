# Strange
阅读源码最好的方式，是从第一个 commit 读到最后一个。`strange` 脚本就是帮助我们 checkout 到我们想看的 commit。

English version goes [here](README.md).

## 使用
- 首先，我们需要将 `strange` 加到环境变量中。
- Checkout 到项目的第一个 commit。
```bash
strange start 
```

- Checkout 到当前 commit 的下一个 commit。
```bash
strange next
```

- Checkout 到第 n 个 commit 。如果是负数，则是从最新的 commit 往前数。
```bash
strange -n 5    # checkout to 5th commit.
strange -n -1   # checkout to the lastest commit. 
```

- 像 git 一样 checkout.
```bash
strange checkout master
```

- 如果 master 分支更新了, 我们需要执行 `strange clean` 去更新 commit 列表。我们将 commit 列表存储在 `.git/strange_log`。

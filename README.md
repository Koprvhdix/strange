# Strange
The Doctor Strange of git repository. The best way to read source code, such as etcd, is reading code from the first commit to the last. The shell `strange` is to help us checkouting the commit we want.

[中文文档/Chinese Documentation](README_CN.md)

## Usage
- First of all, we should add `strange` to $PATH.
- Checkout to the first commit of the repository.
```bash
strange start 
```

- Checkout to the next commit of the current commit.
```bash
strange next
```

- Checkout to the nth commit.
```bash
strange -n 5    # checkout to 5th commit.
strange -n -1   # checkout to the lastest commit. 
```

- Checkout as git.
```bash
strange checkout master
```

- When the master branch updates, we should run `strange clean` to update the commit list. The commit list of master branch will be in `.git/strange_log`. 

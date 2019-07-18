# Strange
The Doctor Strange of git repository. The best way to read source code, such as etcd, is read code from the first commit. The shell `strange` is to help us checkout the commit we want.

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

- When the master branch update, we should run `strange clean` to update the commit list. The commit list of master branch will be in `.git/strange_log`. 

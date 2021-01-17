# git-training

## 터미널 환경

- Windows
  - Git Bash (PowerShell보다 익숙함..)



## 1) 시작하기

### clone

```shell
git clone https://github.com/gimsesu/git-training.git git-training
```



## 2) 원격 저장소 추가하기

### 원격 저장소 목록 확인

```shell
$ git remote
origin
```

### 원격 저장소 정보 자세히 보기

```shell
$ git remote -v
origin  https://github.com/gimsesu/git-training.git (fetch)
origin  https://github.com/gimsesu/git-training.git (push)
```

### upstream 원격 저장소 추가

```shell
$ git remote add upstream https://github.com/CodeSoom/git-training.git
```

```shell
$ $ git fetch upstream
From https://github.com/CodeSoom/git-training
 * [new branch]      main       -> upstream/main
```

upstream 추가 후 원격 저장소 정보 확인

```shell
$ git remote
origin
upstream
```

```shell
$ git remote -v
origin  https://github.com/gimsesu/git-training.git (fetch)
origin  https://github.com/gimsesu/git-training.git (push)
upstream        https://github.com/CodeSoom/git-training.git (fetch)
upstream        https://github.com/CodeSoom/git-training.git (push)
```

Sourcetree 모습

![git_gimsesu_1](../\images\git_gimsesu_1.png)



## 협업 시작하기

git status

```shell
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        docs/gimsesu.md
        images/git_gimsesu_1.png
```

### Step #1 - 작업 브랜치 만들기

```shell
$ git switch -c gimsesu upstream/main
Switched to a new branch 'gimsesu'
Branch 'gimsesu' set up to track remote branch 'main' from 'upstream'.
```

### Step #2 - upstream 원격 저장소의 최신 상태를 반영하기

```shell
$ git fetch upstream main
From https://github.com/CodeSoom/git-training
 * branch            main       -> FETCH_HEAD

$ git rebase upstream/main
Current branch gimsesu is up to date.
```


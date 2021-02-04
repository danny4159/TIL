# git 기초

> 분산버전관리시스템(DVCS)

## 0. git 저장소(repository) 초기화

```bash
$ git init
Initialized empty Git repository in C:/Users/danny/Desktop/md/.git/
(master) $
```

* `.git`숨김 폴덕 생성되고, bash 환경에서는 `(master)`로 브랜치 정보가 나타난다.

## 작업 흐름

### 1. `add`



현재 작업 중인 파일의 변경사항을 `staging area`로 변경한다.

* staging area : 커밋(버전)으로 기록할 대상의 파일들의 목록

add 전 상황

```bash
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        123.txt

nothing added to commit but untracked files present (use "git add" to track)
```

add 후 상황

```bash
$ git add .

danny@DESKTOP-E4I6D1A MINGW64 ~/Desktop/md (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   123.txt
```



### 2. commit

``` bash
$ git commit -m 'First commit'
[master (root-commit) d4d5d02] First commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 123.txt
```

* 특정시점을 스냅샷처럼 기록한다.
* commit시 메시지는 반드시 잘 작성해야한다.
  * 지금 기록한 코드의 이력을 나타낼 수 있도록



## 기타 명령어

### log

지금까지 기록된 커밋들을 확인할 수 있음

```bash
danny@DESKTOP-E4I6D1A MINGW64 ~/Desktop/md (master)
$ git log
commit d4d5d02f52f64b35e221ff0b290054d0ecae3708 (HEAD -> master)
Author: danny4159 <danny4159@naver.com>
Date:   Thu Feb 4 14:13:06 2021 +0900

    First commit


$ git log --oneline
d4d5d02 (HEAD -> master) First commit

$ git log -2
commit d4d5d02f52f64b35e221ff0b290054d0ecae3708 (HEAD -> master)
Author: danny4159 <danny4159@naver.com>
Date:   Thu Feb 4 14:13:06 2021 +0900
    First commit

$ git log --oneline -1
d4d5d02 (HEAD -> master) First commit

```


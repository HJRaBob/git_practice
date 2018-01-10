## 깃 기초

### add
> index에 commit 할 파일을 저장
>`git reset head file_name` 으로 index에서 삭제 할 수 있다.

### commit
> index에 저장된 내용을 local 저장소에 저장

### push
> commit된 내용을 원격 저장소에 저장

### pull
>원격 저장소에 있는 내용을 로컬 저장소로 가져옴.
>자동적으로 `merge commit이 생긴다.

### 깃 명령어

`git status`: 변경 내역, add 상태 등을 확인

* `git log`: commit 기록 확인
    * `git log -p`: 변경 내용까지 같이 확인

    * `git show head`: `git log -p`를 head만 보여줌

* `git reflog`: 돌아갈 수 있는 commit head 확인

* `git checkout`: 지정한 commit 또는 branch 으로 이동

### 충돌 상황

* 집에서 수정한 파일을 pull 하지 않고 수정을 한 경우
    >태깅을 확인하여 코드를 알맞은 형태로 고치고 태깅 삭제


## branch

### branch 기본
1. branch 생성
    ```
    $ git branch branch_name
    ```

1. branch 확인
    ```
    $ git branch
    ```

1. branch 변경
    ```
    $ git checkout branch_name
    //branch를 생성하면서 이동
    $ git checkout -b branch_name
    ```

1. branch 삭제
    ```
    $ git branch -d branch_name
    //merge 여부와 상관없이 삭제
    $ git branch -D branch_name
    ```

### merge

1. 명령어
    ```
    $ git merge branch_name
    ```
1. Fast-forward
    >브렌치가 뻗을 필요 없이 진행해도 됐을 병합

### 충돌 상황
    
* 한 파일을 다른 브런치에서 동시에 수정한다면
    >태깅을 확인하여 코드를 알맞은 형태로 고치고 태깅 삭제

## 깃 기초

### add
> index에 commit 할 파일을 저장

### commit
> 실제 저장

### push
> commit된 내용을 원격 저장소에 저장

### pull
>원격 저장소에 있는 내용을 로컬 저장소로 가져옴

### 깃 명령어

* `git status`: 변경 내역, add 상태 등을 확인

* `git log`: commit 기록 확인
    * `git log -p`: 변경 내용까지 같이 확인

    * `git show head`: `git log -p`를 head만 보여줌

    * `git reflog`: 돌아갈 수 있는 commit head 확인

    * `git checkout`: 지정한 commit 또는 branch 으로 이동 

## 충돌 상황

1. 집에서 수정한 파일을 pull 하지 않고 수정을 한 경우
> 태깅을 확인하여 코드를 알맞은 형태로 고치고 태깅 삭제

# git의 3가지 영역
- ### Working Directory(unstaged)
- ### Staging Area
- ### repository
<br>

# tracked file 과 untracked file
- ### tracked file : git에 한번 올려서 커밋했던 파일(추적됨)
- ### untracked file : git에 관리되지 않던 새로 추가하는 파일(추적되지 않음)
<br>

# 자주 사용하는 git 명령어
| 명령어 | 설명 |
| ------ | ------ |
| git config --global user.name "사용자이름" | 사용자이름 설정 |
| git config --global user.email "이메일 주소" | 사용자이메일 설정 |
| git init | local 저장소 생성 |
| git status | 현재 저장소의 상태 알아보기 |
| git add . | 변경 사항을 staging area (Index) 에 올리기 |
| git commit -m "commit 메세지" | staging area 에 있는 내용을 commit 하기 |
| git branch 브랜치명 | 새로운 branch 만들기 |
| git branch | branch 목록 보기 |
| git checkout 브랜치명 | branch 이동 |
| git merge 합칠 브랜치명 | branch 합치기(merge) |
| git branch -d 브랜치명 | branch 삭제 |
| git  checkout  HEAD~ | 커서(HEAD) 를 이전 commit 으로 이동하기 |
| git reset --soft HEAD~ | commit 취소 하기(--soft : commit 취소) |
| git reset --mixed HEAD~ | commit 취소 하기(--mixed : staging area, commit 취소) |
| git reset --hard HEAD~ | commit 취소 하기(--hard : working dir, staging area, commit 모두 취소) |
| git  stash  list | 임시 저장된 목록 보기 |
| git  stash  save | 추적되지 않는 파일을 제외하고 변경사항 저장 |
| git  stash  save  -u | 추적되지 않는 파일도 포함해서 변경사항 저장 |
| git  stash  pop | 저장된 변경사항을 지우면서 적용 시키기 |
| git  stash  apply  [ stash id ] | 저장된 변경사항을 유지하면서 적용 시키기 |
| git  stash  drop [ stash id ] | 저장된 변경사항을 삭제하기 |
| git checkout . | working directory의 변경된 내용 모두 삭제하기 |
| git  clean  -fd | untracked file 과 directory 를 모두 삭제하기 |
| git reset | staging area -> working directory 이동(staging area 내용 취소) |
| git remote -v | remote 저장소 목록 보기 |
| git remote add 저장소이름 저장소주소 | remote 저장소 등록 |
| git push -u 저장소이름 브랜치명 | 등록된 remote 저장소에 업로드 하기 |
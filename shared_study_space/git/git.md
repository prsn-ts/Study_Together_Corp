# git의 3가지 영역
- ### Working Directory(unstaged)
- ### Staging Area(index)
- ### repository(local, remote 등)
![git의 3가지 영역](https://github.com/prsn-ts/Study_together_corp/blob/master/picture/git/area.png)

<br><br>

# tracked file 과 untracked file
- ### tracked file : git에 한번 올려서 커밋했던 파일(추적됨)
- ### untracked file : git에 관리되지 않는 새로 추가하는 파일(추적되지 않음)
<br><br>

# 자주 사용하는 git 명령어
| 명령어 | 설명 |
| ------ | ------ |
| git config --global user.name "사용자이름" | 사용자 이름 설정 |
| git config --global user.email "이메일주소" | 사용자 이메일 설정 |
| git init | local 저장소 생성 |
| git log | commit 내역 보기 |
| git status | 현재 저장소의 상태 알아보기 |
| git status -u | 현재 저장소의 상태 알아보기(untracked file 포함) |
| git add . | 변경 사항을 staging area(Index) 에 올리기 |
| git commit -m "commit 메시지" | staging area 에 있는 내용을 commit 하기 |
| git branch 브랜치명 | 새로운 branch 만들기 |
| git branch | branch 목록 보기 |
| git checkout 브랜치명 | branch 이동 |
| git merge 합쳐질 브랜치명 | branch 합치기(merge) |
| git branch -d 브랜치명 | branch 삭제 |
| git checkout HEAD~ | 커서(HEAD) 를 이전 commit 으로 이동하기 |
| git reset --soft HEAD~ | 최근 commit 취소 하기(--soft : commit 취소) |
| git reset --mixed HEAD~ | 최근 commit 취소 하기(--mixed : staging area, commit 취소) |
| git reset --hard HEAD~ | 최근 commit 취소 하기(--hard : working dir, staging area, commit 모두 취소) |
| git stash list | 임시 저장된 stash id 목록 보기 |
| git stash save | 변경사항 임시 저장(추적되지 않는 파일 포함 X) |
| git stash save -u | 변경사항 임시 저장(추적되지 않는 파일도 포함 O) |
| git stash pop | stash 목록 중 가장 최신 stash id를 지우면서(remove) 가져오기 |
| git stash apply | stash 목록 중 가장 최신 stash id를 유지하면서(keep) 적용 |
| git stash apply [ stash id ] | stash 목록 중 stash id에 맞는 데이터를 가져와 적용 |
| git stash apply --index [ stash id ] | stash 목록 중 stash id에 맞는 데이터를 가져와 영역별 데이터 유지하면서 적용 |
| git stash drop | stash 목록 중 가장 최신의 저장된 stash id 삭제하기 |
| git stash drop [ stash id ] | stash 목록 중 특정 stash id 삭제하기 |
| git checkout . | working directory의 변경된 내용 모두 삭제하기 |
| git clean -fd | untracked file 과 directory 를 모두 삭제하기(__복구 불가__) |
| git reset | staging area -> working directory 이동(staging area 내용 취소) |
| git remote -v | remote 저장소 목록 보기 |
| git remote add 저장소이름 저장소주소 | remote 저장소 등록 |
| git push 저장소이름 브랜치명 | 등록된 remote 저장소에 업로드 하기 |

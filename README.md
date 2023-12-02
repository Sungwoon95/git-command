# 깃 명령어 모음

## 깃 저장소 생성
`git init` 깃 저장소 생성
`ls -a` 명령어로 숨김 폴더 `.git` 확인 가능

## 로컬 저장소 <-> 원격 저장소 연결
`git remote add origin https://github.com/~` 원격 저장소 연결
`git remote -v` 연결된 원격 저장소 확인

## 추가, 변경 사항 스테이징 영역에 추가
`git add <filename>` 새롭게 추가되었거나, 변경된 파일을 git 스테이징 영역에 추가
`git add .`으로 모든 파일 추가 가능

## 변경 사항 커밋 메시지 작성
`git commit -m 'text'` 변경 사항에 대한 커밋 메시지 작성
`git commit --amend` 직전 커밋 내용 덮어쓰기
(`I`키로 수정, 수정 후 `ESC => :wq => Enter` )
## 변경 사항 업로드
`git push origin main` 변경 사항을 git 원격 저장소에 업로드

## 원격 저장소와 동기화
`git pull`

## 커밋 로그 확인
`git log`
`git log --oneline` 커밋 로그를 편하게 볼 수 있음

## 깃 브랜치
`git branch <branch>` 브랜치 생성
`git switch <branch>` 해당 브랜치로 이동

## 삭제 파일 복구
`git checkout -- <filename>`

## 원격 저장소와 병합
`git merge <branch>`

## 과거 커밋 이동
`git reset <commit_id>` 기록에 남지 않음
`git revert <commit_id>` 기록에 남음

## 변경 사항 보류
`git stash push -m 'text'` stash 영역으로 이동
`git stash list` stash list 확인
`git stash show <stash_id> -p` stash 자세히 보기
`git stash apply` 가장 최근의 stash 불러오기
`git stash apply <stash_id>` stash 불러오기

## 다른 브랜치의 커밋 가져오기
`git cherry-pick <commit_id>`

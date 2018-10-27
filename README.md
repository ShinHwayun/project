# git 명령어
## 1. 설정과 초기화
### _전역 사용자명/이메일 구성하기_
git config--global user.name "Your name"
git config--global user.email "Your email address"
### _저장소 복제하기_
git clone <저장소url>
### _새로운 원격 저장소 추가하기_
git remote add <원격 저장소> <저장소url>


## 2. 기본적인 사용법
### _새로운 파일을 추가하거나 존재하는 파일 스테이징하고 커밋하기_
git add <파일>
git commit -m "<메시지>"
### _add 명령에서 Git 대화 모드를 사용하여 파일 추가하기_
git add -i
### _수정되고 추적되는 모든 파일의 변경 사항 커밋하기_
git commit -m “<메시지>” -a
### _마지막 커밋 고치기_
git commit -m “<메시지>” - -amend
### _이전 커밋을 수정하고 커밋 메시지를 재사용하기_
git commit -C HEAD - -amend


## 3. 브랜치
### _지역 브랜치 목록 보기_
git branch
### _원격 브랜치 목록 보기_
git branch -r
### _지역과 원격을 포함한 모든 브랜치 목록 보기_
git branch -a
### _현재 브랜치에서 새로운 브랜치 생성하기_
git branch <새로운 브랜치>
### _다른 시작 지점에서 브랜치 생성하기_
git branch <새로운 브랜치> <브랜치를 생성할 위치>
### _기존의 브랜치를 새로운 브랜치로 덮어쓰기_
git branch -f <기존 브랜치> [<브랜치를 생성할 위치>]
### _다른 브랜치를 현재 브랜치로 합치기_
git merge <브랜치>
### _브랜치 삭제하기_
git branch -d <삭제할 브랜치>


## 4. Git 이력
### _모든 이력 보기_
git log
### _6개월 동안의 커밋 로그 보기_
git log - -since=”6 hours”
### _이틀 전까지의 커밋 로그 보기_
git log - -before=”2 days”
### _파일의 줄 단위의 이동과 원본 파일 정보 보기_
git blame -C -C <파일>


## 5. 원격 저장소
### _저장소 복제하기_
git clone <저장소>
### _새로운 원격 저장소 추가하기_
git remote add <원격 저장소> <저장소 url>


## 6. 그 외 자주 사용되는 명령어
### _브랜치명 브랜치를 만들고 바로 이동_
git checkout
### _브랜치 삭제_
git branch -d(D) test
### _현재상태(머지나 추가사항) 확인_
git status
### _임시저장_
git stash
### _임시저장한파일 불러오기_
git stash pop
### _깃랩에서 삭제한거 서버와 동기화_
git remote prune origin
### _브랜치네임 서버에서 삭제하기_
git push origin


# markdown 문법
**markdown** 은 마크업 언어의 일종으로, 존 그루버(John Gruber)와 아론 스워츠(Aaron Swartz)가 만들었다.
읽기쓰기가 쉽다는 장점이 있으나, 멀티미디어 삽입이 불편하고 확장 문법이 많다는 단점이 있다.
확장자는 __.md__ 를 쓴다.

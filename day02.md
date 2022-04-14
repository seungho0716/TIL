# github 
- clone
원격 저장소를 통째로 복제해서 내컴퓨터로 옮기는 명령어
git clone url
이름 변경 하고싶을때는 URL 뒤에 변경할 이름 작성
- pull
원격 저장소의 변경 사항을 가져와 로컬 저장소를 업데이트 하는명령어
git pull 저장소 이름 브랜치 이름 형태로 작성

- .gitignore
특정 파일 혹은 폴더에 대해 git이 버전관리를 하지 못하게 할때 사용
touch .gitignore 로 파일 생성후 파일안에서 작업

- branch
 계속 서비스되고 있는 master 를 냅두고 개인적으로 작업하는 공간을 만드는것
 원본을 건드리지 않고 작업 협업할때 주로 사용
 
 1. 브랜치 목록 확인
 git branch
 2. 브랜치 생성 
 git branch 브랜치명
 3. 해당 브랜치로 이동
 git switch 브랜치명
**3-1** 브랜치 이동과 동시에 생성
git switch -c 브랜치명
4. 브랜치 병합
git merge 브랜치명
**주의** 병합할때는 master 같이 유지할곳에서 병합할 브랜치를 입력해서 병합
5. 브랜치 삭제
git branch -d 일반삭제
gti branch -D 강제삭제 병합되지 않은 브랜치도 삭제가능
6. 로그 확인 (그래프까지)
git log --oneline --all --graph

- git reset [옵션] <커밋 ID>
특정 커밋 상태로 되돌아감
트정 커밋으로 되돌아 갔을때 해당 커밋 이후 쌓아 놨던 커밋 증발
--soft
돌아가려는 커밋으로 되돌아가고 
이후 commit된 파일들을 stagin area로 돌려놓음(commit 하기전 상태)
다시 커밋할수 있는 상태
--mixed
돌아가려는 커밋으로 되돌아가고
이후 commit된 파일들을 add하기전으로 돌려놓음
옵션 안썼을시 기본값
--hard
돌아가려는 커밋으로 되돌아가고
이후 commit된 파일들 삭제
단 untracked 파일은 untracked로 남음

이미 삭제한 커밋으로 다시 돌아가고 싶을시
git reflog 사용

git revert <커밋 아이디>의 형태로 사용
특정 사건을 없었던 일로 만드는 명령어 이전 커밋을 취소한다는 새로운 커밋을 만듬
git reset은 커밋 내역을 삭제하지만 git revert는 새로 커밋을 쌓음

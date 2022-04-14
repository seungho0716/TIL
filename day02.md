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

# 1. CLI 명령어

1. 파일을 생성하는 명령어(touch)
2. 디렉토리를 생성하는 명령어(mkdir)
3. 핸져 경로의 파일 내역들을 확인하는 명령어(ls)

​	3-1. 숨김폴더, 파일까지 확인(ls-a)

4. 파일을 이동하는 명령어(mv)

​	4-1. 만약에 이동을 지시한 디렉토리가 없다면?

​	->이름이 변경된다

5. 삭제하는 명령어(rm)
6. 현재 경로를 파악하는 명령어(pwd)

​	->절대 경로로 나의 경로를 파악할 수 있다.

​	*절대경로 : /c/Users/studen/Desktop/CLI

​	*상대경로 : ..(상위경로), (현재경로)

# 2. 마크다운 문법

#=>강조 h1~h6까지 6단계

순서가 없는 목록 생성  : -, +, *

순서가 있는 목록 생성 : 숫자.

들여쓰기 TAB

내어쓰기 SHIFT + TAB

기울임 : *글자* 

굵게 :  **글자**

취소선 : ~~취소선~~

코드(`)

인라인 코드 : '코드'

블록코드 : ```언어

코드

```

```

링크

[표시글자](링크)

이미지

![대체 텍스트](이미지 주소 링크)

인용

> 인용하고 싶은 구문

표

|파이프와-하이픈 이용하여 작성

ctrl +t 로 생성가능

원본 소스 보기

ctrl +/

구분선
---
# 3 git
- git = > 분산 버전관리 프로그램  수정사항을 쉽게 확인하기 위해 이용
- github = > 서비스
- git 설정
1. 초기설정
- git config --global user.name "유저명"
- git config --global user.email"깃허브 메일"
2. .설정확인
- git config --global --list
3. 폴더를 저장소로 만들기 최초 1회 진행
- git init
4. 파일 만들기
- touch 파일명.확장자
- 파일 수정
- ctrl + s 저장
5. git에 연결
- git add 파일명.확장자
6. 파일의 상태 파악
- git status
7. 변경사항 기록
- git commit -m "기록한이유"
8. 변경사항 내역 확인
- git log --oneline

# 4 github
 - git hub = 서버에 백업 및 협업을 하기 위해 이용 
1. git hub 들어가서
 - new repository 만들기
 - url 복사
 2. git git hub 연결
 - git remote add origin 복사한url
 3. 연결 확인
- git remote -v
- 오타 났을경우 git remote rm origin 으로 삭제
4. github에 변경사항 백업
- git push origin master


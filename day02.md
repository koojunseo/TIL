# 2일차 정리
## github
### github 가입 및 설정
- git config --global user.name과 user.email을 통해 설정한 정보로 github 가입
- 가입 후 우측 상단 프로필 클릭 후 settings를 클릭하고 왼쪽 안내 바에서 repositories 선택
- repository default branch의 입력 창에서 main 지우고 master로 작성 후 update 클릭
---
### 원격 저장소 생성 및 연결
- new repository 클릭 후 저장소의 이름, 설명, 공개 여부 선택 후 create repository 클릭
- 원격 저장소의 주소 복사 후 vscode open
- git init을 통해 TIL폴더 로컬 저장소로 지정
- git remote add <이름> <주소> 로 원격 저장소 연결
- 원격 저장소 조회는 git remote -v
- 원격 저장소 연결 삭제는 git remote rm <이름>
---
### 원격 저장소에 업로드
- 로컬 저장소에 커밋 생성 후 업로드
- git commit -m "메세지"
- 커밋 생성 후 git push <저장소 이름> <브랜치 이름> 형식으로 업로드
- add -> status -> commit-> log -> push 순
- vscode 자격증명 진행
- 원격 저장소에서 정상 업로드 확인
### .gitignore
- 특정 파일 혹은 폴더에 대해 git이 버전 관리를 하지 못하도록 지정하는 것
- 반드시 이름을 .gitignore로 작성
- .gitignore 파일은 .git 폴더와 동일한 위치에 생성
- 제외 하고 싶은 파일은 반드시 git add 전에 .gitignore에 작성
- .gitignore를 쉽게 작성하기 위해서 gitignore.io에서 자신의 개발 환경에 맞는 것을 찾아서 전체 복사, 붙여넣기 하기
---
### clone, pull
- clone은 원격 저장소의 커밋 내역을 모두 가져와서, 로컬 저장소를 생성하는 명령어
- git clone <원격 저장소 주소>
- pull은 원격 저장소의 변경 사항을 가져와서, 로컬 저장소를 업데이트하는 명령어
- git pull <저장소 이름> <브랜치 이름>

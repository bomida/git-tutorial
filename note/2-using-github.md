## 목차
### Github편
- [준비물](#준비물)
- [준비 작업](#준비- 작업)
- [Github 저장소(Repository) 만들기](#Github-저장소(Repository)-만들기)
- [Github에 소스 올리기](#Github에-소스-올리기)
- [Github에 소스 push 하기](#Github에-소스-push-하기)
- [Github의 소스 내려받기](#Github의-소스-내려받기)


<br>

## 🛠 준비물
- [Github](https://github.com) 계정을 개설해 주세요.
- [Sourcetree](https://www.sourcetreeapp.com)
- [Git](https://git-scm.com)
- IDE(VS Code, Atom etc...) 저는 강의 내용에 따라[VS Code](https://code.visualstudio.com)를 사용했습니다.

<br>

## 👏 이제 따라 해볼까요?
### 준비 작업
 1. 프로젝트 폴더를 만들고 VS Code에서 열어줍니다.
 2. `git init`으로 Git의 관리 항 둡니다.
 3. 아래 작업을 이전에 해줬으면 넘어가도 좋습니다.
 ```
 git config --global user.name "내 이름"
 git config --global user.email "메일 주소"
 ```
 4. 프로젝트 안의 파일들을 메시지를 작성하여 커밋해줍니다.
 ```
 git add -A
 git commit -m "메시지"
 ```
 
<br>

### Github 저장소(Repository) 만들기
  1. [Github](https://github.com)에 접속하여 새로운 repository를 만들어줍니다.
  2. 레포지토리 이름을 작성해주고, 설명을 적어서 습니다.
   <br>그리고 하단에 'Initialize this repository with:' 부분은 체크를 하지말아주세요.
  3. 이제 레포지토리를 생성시켜줍니다.
  <img width="804" alt="스크린샷 2021-10-29 오전 2 04 46" src="https://user-images.githubusercontent.com/93115007/139302924-d0b34560-cbe4-4bec-acab-2bd9af20a8c6.png">


<br><br>

### Github에 소스 올리기
  - VS Code
    1. 앞서 준비 작업한 VS Code를 가져오세요.
    2. 터미널에서 `git status`를 입력해보고 모든 작업이 commit 되어 있는 확인해줍니다.
    <br>혹시 빠진 작업이 있다면 커밋 해줍니다.
    3. 그리고 `git remote`를 입력해주세요. (이 작업은 현 폴더의 원격 레포지토리르 확인하는 명령어입니다.)
    <br>현재 시점으로는 설정한 바가 없기 때문에 아무것도 뜨지 않는 것이 정상입니다.
    4. 만약, 컴퓨터에서 처음 사용하는 계정이라면 이 [링크](https://www.yalco.kr/_02_github_token/)를 보고 먼저 해결해주세요.
    5. 이제 깃허브에 레포지토리 창을 돌아가서 아래의 이미지를 참고해서 1번 명령어를 전부 복사해 VS Code 터미널에 입력해줍니다.
       - 이 명령어는, github 레포지토리를 origin이란 이름의 저장소로 설정하겠다는 뜻입니다.<br>
       - 여기서 origin이란 이름은 브랜치의 기본 이름인 main처럼 기본으로 설정되어있는 이름입니다.<br>
       - 두번 째 줄에 있는 push 명령어는, 폴더의 현 브랜치에 커밋된 내용들을 origin의 레포지토리의 브랜치에 올리겠다는 뜻입니다.
    6. 이제 깃허브 창을 새로고침해보면 파일들이 로컬로부터 push한 파일들이 올라와 있는 것을 확인할 수 있습니다.
    7. 다시 터미널로 돌아와 `git remote`를 입력해보면, origin이라는 원격 레포지토리 이름이 나옵니다.
  <img width="1126" alt="스크린샷 2021-10-29 오전 3 02 02" src="https://user-images.githubusercontent.com/93115007/139310546-d2dc2dba-9152-4f20-9af1-4e6b8f98f55f.png">

  
  - Sourcetree
    1. 소스트리를 실행한 뒤 프로젝트 폴더와 연결 시켜줍니다.
    2. 상단바에 저장소 > 원격저장소추가를 선택해주세요.
    3. 원격 이름은 origin이라 넣고, 그 밑에 URL/경로에는 아래 이미지를 참고해 2번(깃허브 레포지토리 주소)를 복사해 붙여넣습니다.
    4. 사용자명에는 깃허브 유저명을 입력해주고 확인을 눌러주면 소스트리 왼쪽바의 원격 탭에 origin이 뜬걸 확인할 수 있습니다.
  <img width="500" alt="스크린샷 2021-10-29 오전 3 02 02" src="https://user-images.githubusercontent.com/93115007/139311390-54028fba-3a45-41a2-b128-47dab10d4020.png">
  <img width="1126" alt="스크린샷 2021-10-29 오전 3 11 20" src="https://user-images.githubusercontent.com/93115007/139312028-31ed5cb6-1d9d-4e5f-b2c3-5817ad7c5dd0.png">

<br>

### Github에 소스 push 하기
  - VS Code
    1. push를 하는 방법은 `git push origin main`을 입력해주세요.
    <br> main은 디폴값으로 정해진 브랜치 이름으로 각자 정해놓은 브랜치 이름을 써주세요.
    <br> 참고로 저는 원래 브랜치 이름이 Master라고 되어있었는데 Mac
    <br> OS와 윈도우는 대소문자를 구분하지 않는대도 불구하고 명령어가 먹히지 않아서
    <br> master가 아닌 Master그대로 입력해야 먹혔답니다. 해결 방법은 그냥 브랜치 이름을 변경 했습니다.
    2. push가 이뤄지고, Github에 추가 된 것을 깃헙 창에서 새로고침을 하면 볼 수 있습니다.

  - Sourcetree
    1. push를 하고싶다면 상단에 푸시를 눌러주세요.
    2. 그리고 로컬의 main 브랜치를 체크해 올리는걸로 설정한 뒤 확인버튼을 눌러주세요.

<br>

### 다루지 않을 파일 설정
  - .gitignore이란 파일을 통해서 공개적으로 깃허브에 공개되면 안되는 것들을 관리할 수 있습니다.
  - VS Code
    1. 프로젝트 폴더 최상우 공간에 `.gitignore`이라는 이름으로 새로운 파일을 생성합니다.
    <br> (이 파일은 숨김 파일로 지정이 되니 확인하고싶다면, `command + shift + .`로 숨김파일 보기를 해주세요.)
    2. 그리고 노출을 원하지 않는 파일 명을 적어줍니다.
       - 만약 신규 파일과 gitignore파일을 생성하고 `git status`를 입력하면 신규 파일과 gitignore파일 두개가 보일거예요.
       <br> 하지만 gitignore파일에 신규 파일 이름을 적고 저장한 다음 `git status`를 다시 입력하면 신규 파일이 보이지 않는걸 확인할 수 있습니다.
       <br> 그리고 커밋을 하면 신규 파일을 제외하고 커밋된 걸 확인 할 수 있습니다.
 
<br>

 ### Github의 소스 내려받기
  - 
 
<br>

### 작업 주고받기
  - 
 
<br>

### 브랜치 주고받기
  -  
  
<br>


 
 
 
 
<br><br><br>

출처: 얄팍한 코딩사전 님의 <a href= "https://youtu.be/GaKjTjwcKQo">가장 쉬운 Git 강좌 - (하) Github편<a>을 보고 정리한 것입니다.

<h1 align="center">Git tutorial : for beginner</h1>
<p align="center">Quick learn How to use the Git!<br>(when you work alone)</p>

<br> 

## ✔️ 체크사항
- git입문자들을 위한 초급 강의 입니다.
- mac OS 기준으로만 정리하였습니다.

## 🛠 준비물
- [Sourcetree](https://www.sourcetreeapp.com)
- [Git](https://git-scm.com)
- IDE(VS Code, Atom etc...) 저는 강의 내용에 따라 [VS Code](https://code.visualstudio.com)를 사용했습니다.
- 위의 세가지를 모두 다운 받아 주세요.

## 👏 이제 따라 해볼까요?

### Git 저장소 만들기
1. VS Code에서 연결할 폴더를 열어줍니다.
2. VS Code에서 터미널을 열어주세요. (단축키는 command + `)
3. `git init`을 입력합니다. 그러면 빈 저장소가 만들어졌다는 메시지가 뜰 거예요.
<br>(하지만 보이지 숨김 폴더로 생성되었기 때문에 `command+ shift + .`을 누르면 .git이라는 폴더를 볼 수 있습니다.)
<br>*소스트리에서는 새로 만들기 > 로컬 저장소 생성을 누르고 폴더를 연결해 줍니다. 그리고 생성된 git에 더블클릭해서 들어가주세요.*
4. 아래의 명령어를 하나씩 입력해서 사용자의 이름과 이메일을 등록합니다.
```
git config --global user.name "내 이름"
git config --global user.email "본인 이메일주소"
```
> 등록한 이름과 이메일을 확인하고 싶다면 아래의 명령어를 입력 해보세요.
```
git config user.name
git config user.email
```

### 현재 시점을 저장하기
- 폴더에 처음 연결 했을 시에는 우선적으로 커밋을 먼저 해줍니다.
<bt>터미널을 통한 커밋 방법은 `git add -A`를 입력하고, `git commit -m "설명 적기"`을  입력해주세요.
<br>*소스트리에서는 파일 상태란에서 파일들을 선택 후 좌측상단의 커밋 버튼을 눌러서 설명을 적은 뒤 커밋 버튼을 눌러주세요.*
- `git status`를 입력해보면 현재 상황을 볼 수 있습니다.
<br>Untracked files라는 문구가 나온다면 아직 git의 감시하에 있지 않다는 뜻!
<br>*소스트리에서는 파일 상태란에서 볼 수 있습니다.*
- 커밋했던 내역들을 확인하기 위해서는 `git log`라는 명령어를 입력하면 볼 수 있습니다.
<br>이때, 터미널의 맨 밑에 기존의 입력 줄이 안 뜨고 글자도 안 쳐진다면 vi에디터라는게 실행중이므로,
<br>`:q`을 입력하면 빠져나올 수 있습니다.

### 과거 돌아가기 - Reset
- 한 번 과거로 돌아가면 다시는 돌아올 수 없는 단편적인 방법
- VS Code
    1. `git status`를 입력해 내역들을 띄운 다음 내가 돌아가 시점의 일련번호 앞 6자리만 복사를 합니다.
    2. 그런다음 `git reset 일련번호 6자리 --hard`라고 입력합니다.
- Sourcetree
    1. 돌아가고 싶은 시점의 칸에서 마우스 우 클릭으로 `master를 이 커밋으로 초기화`를 클릭해주세요.
    2. 사용 승인 모드 에서 hard를 설정해주세요.
    3. 경고창이 뜨면 '예'를 눌러주세요.
  
### 과거 돌아가기 - Revert
- Revert를 
- 돌아가 시점이 아닌, 취소할 시점을 찾습니다.
- VS Code
    1. `git status`를 입력해 내역들을 띄운 다음 내가 돌아가 시점의 일련번호 앞 6자리만 복사를 합니다.
    2. 그런다음 `git revert 일련번호 6자리`라고 입력합니다.
    3. 
- Sourcetree
    1. 
  
  
  
<br>
<br>
<p align="center">출처: 얄팍한 코딩사전 님의 <a href= "https://www.youtube.com/watch?v=FXDjmsiv8fI&t=791s">가장 쉬운 Git 강좌 - (상) 혼자작업편<a>을 보고 정리한 것입니다.</p>

<h1 align="center">Git tutorial</h1>
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
1. 

<br>
<br>
<p align="center">출처: 얄팍한 코딩사전 님의 <a href= "https://www.youtube.com/watch?v=FXDjmsiv8fI&t=791s">가장 쉬운 Git 강좌 - (상) 혼자작업편<a>을 보고 정리한 것입니다.</p>

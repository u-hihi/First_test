# First\_test

test



안녕하세요. 첫번째 테스트입니다. ㅋ

26.5.26 수정했습니다.

마크다운 문법 예시입니다.(code창 가서 확인해보세요)
# 제목1
## 제목2
### 제목3
#### 제목4

첫 번째 문장    코드창에서 한 줄을 띄우면 새로운 문단이 됩니다.

두 번째 문장

**굵은 글씨**

*기울임*

~~삭제된 내용~~

- 목록1
- 목록2

1. 순서 있는 목록1
2. 순서 있는 목록2

- [x] 체크 박스
- [ ] 빈 박스

'한 줄 코드입니다.'

'''여러 줄 코드입니다.'''

[링크이름](https링크주소를 입력하세요)

![설명](이미지 주소)

> 인용문입니다.

| 이름 | 나이 |     표
|---|---|
| 철수 | 20 |
| 영희 | 22 |

--- 구분선

여기에는 무엇을 할까요?

GitHub의 사용법에 대해 알아봅시다.(초보자 가이드용)

자주 쓰는 용어 및 명령어부터 배워보고 나머지는 차근차근 배워보도록 해요!

Git: 내 컴퓨터에서 변경 기록을 저장하는 도구

GitHub: 그 기록을 인터넷에 올려두는 공간

가장 기본인 Git부터 설치해봅시다.

git-scm.com에서 Git Bash를 깔아줍니다.
- Bash를 깔았으면 들어가서 아래 명령어를 입력해 버전을 확인해요.

명령어: git --version

GitHub에서 계정을 만들어 줍니다.(GitHub 계정 만들기)

Git Bash에 들어가 최초 설정을 해봅시다.(이름 등록)
- 아래의 명령어를 치면 됩니다.

명령어: git config --global user.name "사용자이름"

명령어: git config --global user.email "내이메일@gmail.com"

### 작업 순서
저장소(repository)는 프로젝트 하나를 담는 폴더라고 생각하면 돼요.
1. GitHub에 들어가서 repository를 만들어 줍니다.
- Repository name: 저장소 이름 입력(영어 권장, 띄어쓰기 대신 - 사용)
- Desription: 설명 입력(선택사항)
- Public / Private: Public은 누구든 볼 수 있고 Private는 나만 볼 수 있어요.
- Add a README: README file이란 프로젝트 설명서 파일이라고 생각하면 돼요.
- 다 끝냈다면 Creat repository버튼을 눌러요.(저장소 생성 완료)
- 저장소 삭제는 상단의 settings로 들어가 Danger Zone에서 Delete this repository를 눌러요.(저장소 삭제: 복구x)
2. 내 컴퓨터로 clone(복제)을 합니다.(내 컴퓨터로 가져오기)
- 방금 만든 저장소를 내 컴퓨터로 복사해오는 작업이에요.
- clone을 하면 "현재 내가 있는 폴더" 안에 프로젝트 폴더가 생겨요.

다른 곳에 만들고 싶다면 cd를 하여 이동하고 원하는 폴더가 없다면 mkdir를 사용하여 폳더를 만들어요.

명령어 : git clone 복사한 주소

- 주소는 만든 repository에 들어가서 초록색 <> code버튼을 누르고 HTTPS, SSH, GitHub CLI 중 하나를 선택하여 주소를 복사해요.
만들고 나서 ls를 통해 폴더가 잘 만들어졌는 지 확인해요.

2-1. HTTPS, SSH, GitHub CLI 방법에 대해 알아볼까요?

HTTPS: 브라우저 로그인(or 토큰), 설정이 제일 간단하다.

SSH: SSH키로 인증(공개키/개인키 대조 인증), 보안이 강하지만 설정이 복잡하다.

GitHub CLI: gh 로그인, 터미널에서 바로 처리 가능하지만 gh를 별도로 설치해야된다.

2-2. 사용되는 명령어를 알아봅시다.
> cd(Change Directory) 폴더이름: 다른 폴더로 이동합니다.

> mkdir(MaKe DIRectory) 폴더이름: 새로운 폴더를 만듭니다.

> ls(LiSt): 현재 위치한 곳의 목록을 봅니다.

> pwd(Pring Working Directory): 지금 위치를 출력합니다.

> ~ :홈

> . :현재 위치, 모든 파일  ex) cd . :현재 위치로 이동합니다.

> .. :상위 위치 ex) cd .. :한 단계 위로 올라갑니다.

3. 사용할 폴더로 이동합니다. (cd)

명령어: cd ~/사용할 폴더 위치
4. README.md 파일을 수정합니다.
메모장, VS Code 등을 사용해서 수정할 수 있어요.
- 메모장 명령어: notepad README.md
- VS Code 명령어: code README.md
- VS Code로 프로젝트 폴더 전체를 열 때 명령어: code .
5. 상태를 확인합니다.(status)

명령어: git status

명령어를 치고 나서 modified: README.md가 보이면 정상이에요.
6. 저장할 파일을 선택합니다.(add)

**명령어: git add .**
7. 파일을 저장합니다.(commit)

**명령어: git commit -m "내가 뭘 했는지 메모"**
- 여기서 m은 memo의 약자압니다.
8. GitHub에 파일을 올립니다.(push)

**명령어: git push origin main**
9. 다음번 작업 시작할 때  

**명령어: git pull origin main**

라는 명령어로 시작해요.

pc가 2대 이상 사용될 땐 pull(불러오기)을 해야됩니다. 만약 하지 않았다면 작업을 마치고 push가 거절됩니다. 협업할 때 충돌(conflict)이 날 수 있으니 pull은 필수!

여기까지 했다면 기본 흐름 전체를 다 해보신거예요!


clone은 처음 한 번만 하면 되고, pull은 매번 작업 시작 전에 실행하면 돼요.


#### branch
브랜치는 코드의 독립된 작업 공간입니다.

만약 브랜치 없이 작업한다면 새 기능을 개발하다가 버그가 발생한다면 운영 중인 서비스도 같이 망가지기 때문에 사용됩니다.

새로운 브랜치로 새 기능의 개발을 완료한다면 원래의 브랜치와 병함할 수 있습니다

- 브랜치 생성

명령어: git branch 브랜치명

- 브랜치 이동

명령어: git switch 브랜치명

- 브랜치 생성과 이동을 동시에 할 땐

명령어: git switch -c 브랜치명

여기서 c는 create의 약자입니다.

- 브랜치 합치기

명령어: git switch main (main으로 이동 후)

명령어: git branch 브랜치명 (브랜치를 main에 합치기)

-브랜치 삭제

명령어: git branch -d 브랜치명(merge 완료된 브랜치 삭제)

명령어: git branch -D 브랜치명(merge 안 해도 강제 삭제)

여기서 d는 delete의 약자입니다.

branch는 주로 협업할 때 사용됩니다.

#### conflict
conflict란 충돌 해결인데 같은 파일 같은 줄을 두 곳에서 수정하면 Git이 어떤 걸 써야 할지 몰라서 충돌이 납니다.

해결 방법은 VS Code로 README.md를 열면 
#### 내 컴퓨터에서 삭제
git branch -d test

#### GitHub에서 삭제
git push origin --delete test

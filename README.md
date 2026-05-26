# First\_test

test



안녕하세요. 첫번째 테스트입니다. ㅋ

26.5.26 수정했습니다.

마크다운 문법 예시입니다.(code창 가서 확인해보세요)
# 제목1
## 제목2
### 제목3
#### 제목4

첫 번째 문장
                        한 줄을 띄우면 새로운 문단이 됩니다.
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

Git:
GitHub:

git-scm.com에서 Git Bash를 깔아줍니다.(Git 설치)
- Bash를 깔았으면 아래 명령어를 입력해 버전을 확인해요.
git --version

GitHub에서 계정을 만들어 줍니다.(GitHub 계정 만들기)

Git Bash에 들어가 최초 설정을 해봅시다.(이름 등록)
- 아래의 명령어를 치면 됩니다.
git config --global user.name "사용자이름"
git config --global user.email "내이메일@gmail.com"

#### 저장소 만들기
저장소(repository)는 프로젝트 하나를 담는 폴더라고 생각하면 돼요.
1. GitHub에 들어가서 repository를 만들어 줍니다.
- README.md도 같이 만들어줍니다.
- README file이란 프로젝트 설명서 파일이라고 생각하면 돼요.
2. 내 컴퓨터로 clone(복제)을 합니다.(내 컴퓨터로 가져오기)
- 방금 만든 저장소를 내 컴퓨터로 복사해오는 작업이에요.
- clone을 하면 "현재 내가 있는 폴더" 안에 프로젝트 폴더가 생겨요.
다른 곳에 만들고 싶다면 cd를 하여 이동하고 원하는 폴더가 없다면 mkdir를 사용하여 만들어요.
명령어 : git clone 복사한 주소
- 만든 repository에 들어가서 초록색 <> code버튼을 누르고 HTTPS, SSH, GitHub CLI 중 하나를 선택하여 주소를 복사해요.
만들고 나서 ls를 통해 폴더가 잘 만들어졌는 지 확인해요.

2-1. HTTPS, SSH, GitHub CLI 방법에 대해 알아볼까요?
HTTPS
SSH
GitHub CLI

2-2. 사용되는 명령어를 알아봅시다.
> cd
> mkdir
> ls
> ~
> .
> ..

3. 사용할 폴더로 이동합니다.
4. README.md 파일을 수정합니다.
메모장, VS Code 등을 사용해서 수정할 수 있어요.
- 메모장 명령어: notepad README.md
- VS Code 명령어: code README.md
- VS Code로 프로젝트 폴더 전체를 열 때 명령어: code .
5. 뭐가 바뀌었는지 확인합니다.
명령어: git status
6. 저장할 파일을 골라요.


#### 내 컴퓨터에서 삭제
git branch -d test

#### GitHub에서 삭제
git push origin --delete test

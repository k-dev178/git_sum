# git그리고github
## 버전관리란?
게임에서의 세이브 파일 같은거임.
그림판이나 엑셀, ppt 작업할때 ctrl+z 키를 눌러서 한단계식 뒤로 갈 수 있는것처럼
git도 내가 원하는 시점(버전)으로 이동할 수 있게 해줌.

원하는 시점(버전)으로 이동할 수 있게 해주는 것이 '버전관리'임. 그리고 이것을 도와주는 툴을 '버전 관리 시스템'이라고 함.

프로그래밍으로 예시를 들면..
팀 프로젝트 최초의 소스코드(00 버전)를 올려 놓고, 이것을 팀원 A가 수정을 해서 01버전이 됨.

그런데 팀원 B와 C가 동시에 작업해서 동시에 02버전을 저장한다면??

그래서 버전관리를 해야함.

## git, github란?
### git
내가 원하는 시점에 깃발을 꽂고, 문제가 생기면 그 깃발로 돌아간다면 편안하게 소스 코드를 추가하거나 삭제할 수 있을거임. 이 깃발을 꽂을 수 있게 해주는 툴 또는 소스 코드 버전관리 시스템을 git이라고 함.

### github
그런데 다른사람이랑 프로젝트는 어떻게 할거임?
git은 다른사람이랑 연결은 안시켜줌.. git만으로는 인터넷으로 다른사람의 소스파일을 가져오기 힘듦.(물론 LAN연결이 되어있어서 ssh나 공유폴더 이런거 쓰면 모르겠지만)

그래서 필요한게 github임.
이건 다른사람이 편하게 내 소스코드를 가져오기 쉽게 호스팅해주는 서비스.
대표적인게 github이고 이거 외에 gitlab, bitbucket이 있음.

또 이렇게 github에 공개 저장소로 올려놓으면 언제 어디서든지 내 소스코드를 평가(?)하고 수정할 수 있다는 거임. ~(그래서 github를 하면 코딩을 더 열심히 하게 됨)~ 이런거를 오픈소스라고 함.

# git 설치하고 로컬 저장소에서 커밋 관리하기
## git 설치

```bash
brew install git
```

## 로컬 저장소 만들기

```bash
mkdir documents/git_p
```

README.txt 생성
```txt
개발자 티셔츠 쇼핑몰 오픈소스
```

```bash
cd documents/git_p
git init
```

## 첫 번째 커밋 만들기
```bash
git config --global user.email "이메일"

git config --global user.name "유저이름"
```

```bash
git add README.txt
git commit -m "사이트 설명 추가"
```

README.txt 수정
```txt
개발자 티셔츠 쇼핑몰 오픈소스 짱
```

```bash
git add README.txt
git commit -m "설명 업데이트"
```

## 다른 커밋으로 이동
```bash
git log
```

이거 치면 대충
```
commit 643ffeiarrha4rhl4hawfe9hef

설명 업데이트

commit 9489an4h9agpg98anpg8anerp9

사이트 설명 추가

```

이렇게 뜸.

```bash
git checkout 643ffei # 앞 7자리
```

다시 최신으로 돌아가려면
```bash
git checkout -
```

# github 원격 저장소에 커밋 올리기
## 원격 저장소 만들기
걍 깃허브가서 만들어

## 원격 저장소에 커밋 올리기
```bash
git remote add origin repo 링크
git branch -M main
git push origin main
```

# github 원격 저장소의 커밋을 로컬 저장소에 내려받기
## 원격 저장소의 커밋을 로컬 저장소에 내려받기
```bash
git clone 링크 .
```
.을 붙이는게 좋음

## README.txt 수정

README.txt 수정
```txt
개발자 티셔츠 쇼핑몰 오픈소스 짱

개발자목록
1. 고양이
2. 문어
```

```bash
git add README.txt
git commit -m "개발자 목록 추가"
git push origin main
```

## 수정된 README.txt pull
```bash
git pull origin main
```
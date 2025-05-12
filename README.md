## node.js backend 2기 1팀 git 연습 레포지토리
git 배운거 써먹어 보아요~
지금은 dev 라는 branch 에 본인 소개 html 을 올려보는 간단한 사용법을 연습해봅니다!

대충 git 은 이렇게 코드를 주고 받는구나~ 를 이해하는 데 중점을 둡니다.

### git clone
```shell
git clone https://github.com/gyunam-bark/nb02-git-playground.git
```
먼저 git repository 를 복사해옵니다.

#### 디렉토리 구조
```text
nb02-git-playground
├ README.md
```
이렇게 README.md 만 있는 휑한 상태이면 정상입니다!

이제, 우리가 작업 중인 dev brunch 로 바꾸어볼까요?

### git switch
```shell
git switch dev
```
switch 명령어를 입력하면 branch 를 수정할 수 있습니다.

```shell
branch 'dev' set up to track 'origin/dev'.
Switched to a new branch 'dev'
```

이렇게 dev 로 변했다라고 뜨면 됩니다.

### git pull
```shell
git pull
```
이제 dev 에 있는 개발 중인 파일을 pull 받습니다.

#### 디렉토리 구조
```text
nb02-git-playground
├ pages
  ├ gyunam.html
  ├ ...
├ index.html
├ README.md
```
이렇게 파일들이 늘어나면 완벽합니다!

### 코드 수정
1. pages 디렉토리 안에 **이름.html** 파일 만들기.
2. gyunam.html 안에 있는 코드 복사 붙여넣기 후 수정하기.
```html
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <!-- 이름 -->
  <title>본인이름</title>
</head>

<body>
  <!-- 이름 -->
  <h1>본인이름</h1>
  <!-- 좋아하는 음식 -->
  <strong>좋아하는 음식</strong>
  <p>본인좋아하는음식</p>
</body>

</html>
```
주석이 적혀있지만, 몇가지 단어만 수정하면 됩니다. :)

어차피 git 을 사용하는게 목표니까요!

3. index.html 에 이름 추가하기.
```html
<!DOCTYPE html>
<html>

<head>
  <title>1팀</title>
</head>

<body>
  <header>
    <h1>1팀 목록</h1>
    <nav>
      <ul>
        <li><a href="./pages/gyunam.html">박규남</a></li>
        <!-- 아래에 추가 -->
        <li><a href="./pages/gyunam.html">본인이름</a></li>
        <!-- 위에 추가 -->
      </ul>
    </nav>
  </header>

</body>

</html>
```

### index.html 열어서 확인해보기

### git add
```shell
git add .
```

### git commit -m ""
```shell
git commit -m ""
```

### git push
```shell
git push origin dev
```

### 에러가 발생하면 뭐가 원인인지 검색해보기
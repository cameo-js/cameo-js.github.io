---
layout: page
subheadline: "블로그만들기-1"
title: "Github Pages"
teaser: "Github Pages를 이용해서 Website 구축하기"
header:
    image_fullwidth: "headers/header_img3.jpg"
    caption: Image by Jeremy Bishop
    caption_url: "https://unsplash.com/jeremybishop"
categories:
    - tools
comments: true
show_meta: false
---

Github은 [Github Pages][1]라는 서비스를 통해서 Website를 구축하게 해준다. 하지만 크게 두가지 전제조건이 들어가는데 하나는 git을 다룰 줄 알아야 하고 다른 하나는 [Github의 회원가입][2]이 되어있어야 한다.

[Github Pages][1]에 tutorial 형태로 잘 설명되어 있지만 간략하게 정리해본다.

### 1. 저장소 만들기
[https://github.com/new][3] 링크에서 저장소를 만들면 되는데 Page로 제공하기 위해는 규칙이 있는데 그 규칙은 저장소의 이름이 `username.github.io` 와 같은 패턴이어야 한다.<br/>
username은 개인(your username) 혹은 단체(organization name)을 이용할 수 있다.

### 2. 저장소 가져오기
다음의 명령어를 통해서 로컬 디렉토리에 해당 저장소를 가져온다.<br/>
`git clone https://github.com/username/username.github.io`

### 3. Website에 보여줄 컨텐츠 제작
해당 디렉토리에가서 웹사이트로 보여줄 근사한? 컨텐츠를 제작한다.

	cd username.github.io
	echo "Hello World" > index.html

### 4. Push!!
작업된 컨텐츠 파일을 Github 저장소에 올리면 본인의 저장소명 형태인 `http://username.github.io` 사이트에서 확인이 가능하다.

	git add --all
	git commit -m "Initial commit"
	git push -u origin master

### 추가정보
추가정보는 [Github help 페이지][4]에서 확인할 수 있다.

[1]: https://pages.github.com/
[2]: https://github.com/join
[3]: https://github.com/new
[4]: https://help.github.com/categories/github-pages-basics/
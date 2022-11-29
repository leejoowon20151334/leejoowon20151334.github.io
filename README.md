과제 - Remote Repository의 README.md 자신의 프로젝트를 Build한 과정을 기술
==========

1. jekyll 설치
----------
 - 기존에 ruby가 존재하는 관계로 아래 명령어를 실행하였다.
```
gem install --user-install bundler jekyll
```
 - 에러가 발생하여 확인해 보니 rbenv가 system의 기본 버전을 사용하여 발생하는 문제였다.
 - 아래 명령어를 실행하여 변경하였다.
```
rbenv global 2.7.2
```
 - 아래 명령어를 통해 jekyll 기본 파일을 생성했다.
```
jekyll new . --force
```
 - 아래 명령어를 통해 jekyll server를 실행하였다.
```
bundle exec jekyll serve
```
 - localhost:4000에 페이지가 생성된 것을 확인하였다.

2. 테마 변경
-----------
 - 아래 주소의 테마를 내려받아 기존 폴더에 복사하였다.
 - http://jekyllthemes.org/themes/dash/
 - 아래와 같은 에러가 발생하였다.
```
An error occurred while installing http_parser.rb (0.8.0), and Bundler cannot continue.Make sure that gem install http_parser.rb -v '0.8.0'
```
 - 아래 블로그를 참조하여 에러를 해결하였다.
 - https://withhsunny.tistory.com/87

3. _config 수정
----------
 - title, email 등을 아래와 같이 변경하였다.
```
title: jwlee51
email: jwlee51@kookmin.ac.kr
```

4. post 추가
------------
 - ./_posts/ 경로에 post를 추가하였다.


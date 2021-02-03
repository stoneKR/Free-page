# Git 사용에 필요한 메모
----------
### 명령어
-----------
1. cd [폴더 이름] : 해당 디렉토리로 이동
```
$ cd .. : 하위 폴더로 이동
$ cd 디렉토리 이름 : 해당 디렉토리로 이동
$ cd /c/workspace : 절대경로 workspace로 한번에 이동
```
2. mkdir [폴더 이름] : 디렉토리 생성
```
$ mkdir test : 현재 위치에 test 디렉토리 생성
```
3. touch [파일 이름] : 빈 파일 생성
```
$ touch test.txt : 현재 위치에 test.txt 파일을 생성
```
4. ls : 현재 디렉토리 폴더 , 파일을 보여줌
```
$ ls
```
### Git 사용
----------
+ 사용자 등록
user.email과 user.name을 등록한다.
```
$ git config --global user.email "[이메일 주소]"
$ git config --global user.name "[이름]"
```
+ 저장소 생성 및 commit
```
$ git init
```
>init을 하면, master branch가 생성됨 (git basg 현재 폴더명에 branch 이름(master)추가)

git bash에서 뒤에 (master)와 같이 branch 이름이 보이면 git 저장소가 설정된 폴더다.

init 이후에 해당 폴더에 .git의 숨김 폴더는 건들지 않는다.


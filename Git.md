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
  > user.email과 user.name을 등록한다.
  ```
  $ git config --global user.email "[이메일 주소]"
  $ git config --global user.name "[이름]"
  ```

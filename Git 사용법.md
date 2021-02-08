# Git 사용에 필요한 메모

----------


### Git Bash 설치
------------
> Git을 사용하기에 앞서 Git Bash 툴을 이용하여 진행합니다
> 설치는 https://git-scm.com/ 에서 합니다.

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

# Git 사용


### git config 
----------

+ 사용자 등록 git config (최초 1회 실행)  

```
// git commit에 사용될 username
git config --global user.name "your_name"
 
// git commit에 사용될 email
git config --global user.email "your_email@example.com"
 
// 설정한 내용을 확인할 수 있다.
git config --list
```

+ 해당 작업은 <u>최초 1회만</u> 실행!
----------
### git init
  
------------
+ git init : 현재 디렉토리를 로컬저장소로 설정한다.
```

// 로컬저장소로 설정할 프로젝트 위치로 이동한다.
cd D:/workspace/
 
// 로컬저장소로 설정한다.
// (master) 브랜치로 보이면 성공한 것이다.
git init
 
// 만약 init을 취소하려면 아래의 명령어를 입력한다.
rm -r .git
```

### git status(로컬저장소의 현재 상태)
------------

+ git status를 사용함으로 로컬저장소의 현재 상태를 보여준다.


### git add(Staging Area로 이동)  
-------------

+ 파일을 준비영역(Staging Area)으로 옮긴다. (GitHub와 연동하려면 git remote로 원격 저장소와 연결해야 함)

```
// a.html 파일만 추가
git add a.html
 
// 워킹 디렉터리 내 모든 파일을 추가
git add .
 
// 명령 프롬프트에서 상호작용하면서 추가 (나갈땐 q를 입력)
git add -i
 
// 진행중인 파일일 경우, Staging Area에서 워킹 디렉터리로 옮겨온다. 
$git rm --cached a.html
$git rm -r --cached .
$ git commit -m "메세지"
```



$ git log
```

commit 된 list 를 보여줌

log를 통해보면, 7자리로 commit id가 지정된 모습을 확인 할 수 있다.

+ 이전 commit 돌아가기

```
$ git reset --hard [commit 아이디]
```

때떄로 이전 commit 상태로 돌아가고 싶을 때가 있다

reset 기능을 통해 해당  commit 상태로 되돌리는 것이 가능함

> --hard : commit 당시 상태로 완전히 되돌림
>
> --soft : commit만 취소하고 파일들은 현재 상태를 유지
>
>(soft는 즉, commit id는 삭제되지만 해당 commit id로 지정한 파일은 사라지지 않는다)



### 원격 저장소에 연동하기

------------------

원격 저장소에 연동하기에 앞서, 로컬 저장소는 다음과 같이 구성되어 있다.

```
1. 작업 디렉토리 : 실제 파일들이 존재
2. 인덱스 : 준비 영역의 역활
3. 헤드 : 최종 확정본(commit)
```

> git add를 하면 : 인덱스에 추가
>
> git commit을 하면 : 헤드에 추가, 실제로 변경 내용을 확정
>
> 이후에 git push 를 통해 원격 저장소에 반영을 하게 된다.
>
> 
>
> push 는 로컬 저장소에 원격 저장소를 연결하고 사용해야 함
>
> github 사이트에서 연동할 repository를 생성해두고 진행

+ 원격 저장소 연동하기

```
$ git remote add origin [연동할 github repository url].git
```

이제 해당 로컬 저장소와 원격 저장소가 연동된다

잘 연동되었는지 확인 하려면 아래와 같이 작성하면 된다

```
$ git remote -v
```

콘솔창에 내 github repisitory 주소가 잘 나오면 문제가 없는 것 이다

+ 원격 저장소에 올리기

```
$ git push origin master
```

데이터가 전송되는 모습이 나오면서, commit한 데이터가 github에 올라간 모습을 확인 할 수 있다

### 기본적인 명령어
----------------
```
1. 화면 초기화 : Ctrl + L
2. 한 행의 처음과 끝 : Ctrl + A, Ctrl + E
3. 목록 보기 : ls 또는 dir
4. 파일의 내용 보기 : cat
5. 특정 문자를 검색 : grep
6. 디렉터리로 이동 : cd
7. 디렉터리 생성 : mkdir
8. 파일 삭제 : rm
9. 파일 생성 : touch
```

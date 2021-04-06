## MariaDB 설치

--------

1. https://downloads.mariadb.org/mariadb/10.3.11/
2. [mariadb-10.3.11-winx64.msi](https://downloads.mariadb.org/interstitial/mariadb-10.3.11/winx64-packages/mariadb-10.3.11-winx64.msi/from/https%3A//archive.mariadb.org/) 55MB
3. **Next**
4. I accept the terms in the License~ **체크**  **Next**
5. 정보 입력창 전부 **체크** 후 **Next**
6. **Finish**



## HeidiSQL실행

----------

- 아직 MariaDB Server에 연결된 상태는 아님

    1. **신규** 선택
    2. **암호 1234** 
    3. 왼쪽 세션에서 **Rename** 변경 Name **localhost** 후 **저장** 후 **열기**

- 열린 화면이 MariaDB Server에 접속된 HeideSQL 모습



## Path 추가

-----

- MariaDB의 실행 파일이 있는 경로를 Path에 추가하기
  1. Windows **시작**에서 마우스 오른쪽 클릭한 후 **[Windows PowerShell(관리자)]** 선택해서 관리자 권한으로 실행
  2. **CMD**작성 후 엔터
  3. **SETX PATH "C:\Program Files\MariaDB 10.3\bin;%PATH%" /m** 띄어쓰기 및 글자가 틀리지 않도록 주의
  4. 지정한 값 저장 성공


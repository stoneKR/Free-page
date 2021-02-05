# Markdown 사용법


### 제목
-------------------------
+ 6단계로 사용이 가능합니다.
```
#
##
###
####
#####
######
```


### 강조(Emphasis)
-----------------------

각각 (<em>), (<strong>), (<del>) 태그로 변환됩니다.
  
  
밑줄을 입력하고 싶다면 <u></u> 태그를 사용하세요.
```
이텔릭체는 *별표(asterisks)* 혹은 _언더바(underscore)_를 사용하세요.
두껍게는 **별표(asterisks)** 혹은 __언더바(underscore)__를 사용하세요.
**_이텔릭체_와 두껍게**를 같이 사용할 수 있습니다.
취소선은 ~~물결표시(tilde)~~를 사용하세요.
<u>밑줄</u>은 `<u></u>`를 사용하세요.
```

이텔릭체는 별표(asterisks) 혹은 언더바(underscore)를 사용하세요.
두껍게는 별표(asterisks) 혹은 언더바(underscore)를 사용하세요.
이텔릭체와 두껍게를 같이 사용할 수 있습니다.
취소선은 물결표시(tilde)를 사용하세요.
밑줄은 <u></u>를 사용하세요.


### 목록
-----------------
+ <ol>, <ul> 목록 태그로 변환됩니다.
  
  ```
  1. 순서가 필요한 목록
  1. 순서가 필요한 목록
    - 순서가 필요하지 않은 목록(서브) 
    - 순서가 필요하지 않은 목록(서브) 
  1. 순서가 필요한 목록
    1. 순서가 필요한 목록(서브)
    1. 순서가 필요한 목록(서브)
  1. 순서가 필요한 목록

- 순서가 필요하지 않은 목록에 사용 가능한 기호
  - 대쉬(hyphen)
  * 별표(asterisks)
  + 더하기(plus sign)
  ```
  
1. 순서가 필요한 목록
2. 순서가 필요한 목록
    + 순서가 필요하지 않은 목록(서브)
    + 순서가 필요하지 않은 목록(서브)
3. 순서가 필요한 목록
    1. 순서가 필요한 목록(서브)
    2. 순서가 필요한 목록(서브)
4. 순서가 필요한 목록


+  순서가 필요하지 않은 목록에 사용 가능한 기호
+    대쉬(hyphen)
+    별표(asterisks)
+    더하기(plus sign)



### 링크 (links)
-------------------
<a> 로 변환 됩니다.
  ```
  [GOOGLE](https://google.com)

[NAVER](https://naver.com "링크 설명(title)을 작성하세요.")

[상대적 참조](../users/login)

[Dribbble][Dribbble link]

[GitHub][1]

문서 안에서 [참조 링크]를 그대로 사용할 수도 있습니다.

다음과 같이 문서 내 일반 URL이나 꺾쇠 괄호(`< >`, Angle Brackets)안의 URL은 자동으로 링크를 사용합니다.
구글 홈페이지: https://google.com
네이버 홈페이지: <https://naver.com>

[Dribbble link]: https://dribbble.com
[1]: https://github.com
[참조 링크]: https://naver.com "네이버로 이동합니다!"
  ```
  
  > 문서 안에서 참조 링크를 그대로 사용할 수도 있습니다.
  > 다음과 같이 문서 내 일반 URL이나 꺾쇠 괄호(< >, Angle Brackets)안의 URL은 자동으로 링크를 사용합니다.
  > 구글 홈페이지: https://google.com
  > 네이버 홈페이지: https://naver.com
  
  
  
### 이미지(images)
-------------------

> <img>로 변환됩니다.
> 링크과 비슷하지만 앞에 !가 붙습니다.


```
![대체 텍스트(alternative text)를 입력하세요!](http://www.gstatic.com/webp/gallery/5.jpg "링크 설명(title)을 작성하세요.")

![Kayak][logo]

[logo]: http://www.gstatic.com/webp/gallery/2.jpg "To go kayaking."
```

### 이미지에 링크
--------------------------

마크다운 이미지 코드를 링크 코드로 묶어 줍니다.

```
[![Vue](/images/vue.png)](https://kr.vuejs.org/)
```

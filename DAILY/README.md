# Here's my daily TIL

## [250116] TIL: Let's Being a Personal Github Page Owner
---
### CLI
* 절대 경로: Root 디렉토리부터 목적지점까지 거치는 모든 경로를 전부 작성한 것
* 상대 경로: 현재 작업 중인 디렉토리를 기준으로 계산된 상대적 위치를 작성한 것

---
### Git
* Git: 분산 버전 관리 시스템
* Git의 영역: Working Directory, Staging Area, Repository
* Git의 동작: git과 관련된 명령어이면 무조건 git으로 시작함
+   ```git init```
+   ```git add``` 
-    ```git add .```: 모든 파일
-    ```git add 파일명```: 특정 파일
+   ```git commit -m "커밋 메시지"``` 

---
---

## [250117] TIL: Create My Portpolio Using Github
---
## Revert&Reset
* Revert 
```git revert <commit id>```
특정 commit을 실행 취소하는 것
취소한 history가 기록되기 때문에 무결성을 보장하며 협업의 신뢰성을 ㄴㅍ임

* Reset
```git reset [옵션] <commit id>```
특정 commit으로 되돌아가는 것
돌아간 지점 다음에 만들어진 commit을 어떻게 처리할 지에 대해 3가지 옵션이 있음
   ```git reset --soft <commit id>``` : commit기록을 staging area에 남김
   ```git reset --mixed <commit id>``` : commit기록을 working directory에 남김
   ```git reset --hard <commit id>```: commit기록을 아예 삭제
   
---
## [250120] TIL: Basic Python Syntax

## Expressions&Values
* Expressions
표현식: 값으로 평가될 수 있는 코드 조각
   ex. 3+5

* Values
값: 표현식이 평가된 결과
   ex. 8

* 평가
표현식을 실행하여 값을 얻는 과정
표현식을 순차적으로 평가하여 프로그램의 동작을 결정
평가가 일어나야만 값이 반환됨 (평가가 없으면 값이 반환되지 않음)

* Statement 
문장: 실행가능한 동작을 기술하는 코드
   ex. 조건문, 반복문, 함수 정의 등

---
## Types
* Types
타입: 변수나 값이 가질 수 있는 데이터의 종류
2가지 요소로 이루어짐
   1. 값(피연산자)
      * Numeric
         a. int

            진법의 표현: 2진수(0b), 8진수(0o), 10진수(0x)

         b. float

            부동소수점 에러 발생에 유의

      * Sequence
         a. str

            문자열: 문자들의 순서가 있는 **변경 불가능한** 시퀀스 자료형

            단일 문자/여러 문자의 조합으로 구성됨

            작은따옴표 또는 큰따옴표로 감싸서 표현됨

            * Escape scquence 

               \n 줄 바꿈

               \t 탭

               \\ 백슬래시

               \' 작은 따옴표

               \" 큰 따옴표


            * String Interpolation

            문자열 내에 변수나 표현식을 삽입하는 방법

            **f-string**

            문자열에 f또는 F 접두어를 붙이고 표현식을 {expression} 으로 작성하는 문법

            문자열에 파이썬 표현식의 값을 삽입할 수 있음  

         b. index 
            시퀀스 내 값들에 대한 고유 번호

            각 값들의 위치를 식별하는데 사용되는 숫자

            양수/음수 인덱싱이 존재

            *  슬라이싱

            시퀀스의 일부분을 선택해 추출하는 작업업     

      * Text Sequence
      * Non-sequence
      * 기타
   
   2. 연산자
      * ``` - ``` : 뺄셈, 음수부호
      * ``` + ``` : 덧셈
      * ``` * ``` : 곱셈
      * ``` ** ``` : 지수(거듭제곱)
      * ``` / ``` : 나눗셈
      * ``` // ``` : 나눗셈의 몫
      * ``` % ``` : 나눗셈의 나머지

      2.1. 연산자의 우선순위
      * ``` ** ``` 
      * ``` - ``` 음수부호
      * ``` *. /, //, % ```
      * ``` +, - ```
---
## Variables
* 변수: 값을 저장하기 위한 이름
* 변수 할당: 표현식을 통해 변수에 값을 저장
* 할당문: ``` variable = expression ```

   할당 연산자 오른쪽에 있는 표현식을 평가해서 값(메모리 주소)을 생성

   값의 메모리 주소를 할당 연산자 왼쪽에 있는 변수에 저장 (경우에 따라 할당/재할당)




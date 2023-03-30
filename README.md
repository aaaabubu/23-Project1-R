# 안진홍 602377109

## [ 03월 30일 학습내용 ]
>오늘 배운 내용 정리

### r에서의 자료구조

    1차원 자료 벡터 리스트 팩터
    2차원 자료 매트릭스 데이터프라임

### 범주형 자료와 수치형 자료

    범주형 자료: 분류의 의미를 갖는 값들로 구성된 자료로 보통 문자로 표현되고 산술연산을 적용할수없음
    수치형 자료: 값들이 크기를 가지며 산술연산이 가능함
    
### 데이터 분석에 많이 사용 되는 함수
![image](https://user-images.githubusercontent.com/35441691/228815641-3a56f8fe-22c3-42a8-be4a-95019a20de7c.png)


## [ 03월 23일 학습내용 ]
>오늘 배운 내용 정리

### R 패키지란?
여러개의 함수를 가진 꾸러미라고 표현할 수 있으며, 하나의 패키지 안에는 다양한 함수들이 들어있음.

### R 패키지 설치

    install.packages("ggplot2")

### 변수
어떤 값을 보관하는 공간을 변수라고 함<br>
R에서 변수를 선언할 때는 할당 연산자인 "="와 "<-"을 활용함

### 벡터

    • 한 가지 데이터 타입으로 저장 가능
    • 기본적으로 열벡터 형태로 저장됨
    • 벡터 연산으로 빠르게 처리 가능

## [ 03월 16일 학습내용 ]
>오늘 배운 내용 정리

### R언어의 특징

    • 변수들이 저장되는 환경이라는 데이터 타입이 있다.
    • 변수를 선언 및 할당하면 해당 변수가 .GlobalEnv 라는 환경에 생성된다.
    • 기본적으로 함수의 매개변수로 받는 값은 함수 내부에서 값을 변경하더라도 외부에 반영되지 않는다. 이러한 이유로 일반적으로 함수를 정의하게 되면 순수함수가 되어 Side Effect 를 줄일수 있다.
    • 함수를 입력받거나 반환할 수 있어 함수형 프로그래밍을 하기에 용이하다.
    • assign() 함수를 이용하여 동적으로 원하는 환경에 변수를 생성해낼 수 있으며 이를 이용하여 객체지향 프로그래밍을 구현해낼 수도 있다.
    • Java, C, PHP 등 다른 프로그래밍 언어와 연결이 용이하고, 윈도우, 맥 OS, 리눅스 및 유닉스 등의 컴퓨터 운영체계를 지원한다.

### R을 배우는 이유

    • 4차 산업혁명 때문
    • 4차 산업혁명의 중심은 '데이터'
    • 시대적 흐름은 데이터를 잘 다룰 줄 아는 기업과 개인이 경쟁에서 우위를 점할 수 있음을 의미
    • 컴퓨팅 사고와 데이터 활용 능력은 전공을 불문하고 어떤 분야로 진출하든 점점 더 중요한 스펙이다
    
### R스튜디오 화면 구성

    • Script 창
    • Console 창
    • Environment/History 창
    • Files/Plot/Packages/Help/Viewer 창

## [ 03월 09일 학습내용 ]
>오늘 배운 내용 정리

### Git 사용자 설정

    • Global 사용자 정보 설정: 시스템 전체에서 사용
    • 스페이스가 없으면 “ ”(double quotes)은 사용하지 않아도 됨
#### 예시

    $ git config --global user.name “AHN JIN HONG”
    $ git config --global user.email “example@naver.com”
    
#### 설정 내용 확인

    $ git config user.name
    $ foo
    $ git config user.email
    $ foo@example.com
    
### 프로젝트 폴더 Git으로 초기화 하기

    • 명령은 원하는 폴더로 이동 후 git init 명령으로 초기화 할 수 있음
    • VSCode에서는 ‘source control > Initialize Repository’ 버튼 클릭
    • 폴더에는 .git 이라는 숨긴 폴더가 생성
    
![image](https://user-images.githubusercontent.com/35441691/224522969-6e4708a1-3473-4c6a-904c-14d5d4855524.png)
![image](https://user-images.githubusercontent.com/35441691/224522990-aacf52fe-28a3-4050-a372-12ed12c6989b.png)

### 커밋 하기

    • Git으로 초기화된 폴더에 파일이 생성되거나, 파일의 내용이 변경되면 Git이 추적을 시작
    • 변한 파일의 숫자 만큼 source control에 숫자가 표시 됨
    • source control 아이콘을 클릭하고, commit을 원하는 파일을 stage로 이동
    • Stage로 이동 할 때는 파일이름 오른쪽의 ‘+’ 버튼을 클릭
    • State로 올라온 파일을 취소하고 싶으면 ‘-’ 버튼을 클릭
    • 원하는 파일을 stage에 올린 다음, 위쪽의 ‘Message … ’ 라고 쓰여 있는 부분 commit 제목과 자세한 설명 쓰기
    • 제목은 50character 이내로 작성하고, enter키를 두 번 입력 후 자세한 설명 쓰기
    • 제목과 내용을 쓴 다음 ‘ctrl + enter’ 를 누르거나, 아래 쪽의 ‘✔commit’ 버튼이나, 위의✔체크 아이콘을 클릭
    • Commit이 끝나고 나면 source control의 숫자가 하나 줄어 든 것을 확인 가능
    • 이렇게 필요할 때 마다 commit을 해 주면서 프로젝트의 history를 저장하여 버전관리에 활용
 ![image](https://user-images.githubusercontent.com/35441691/224523135-1c76fd4a-448d-4e1d-916b-c9928552c942.png)
 
### 푸시 하기

    • 변경된 내용 모두 commit후 push하는 경우
    • 더 이상 커밋할 파일이 없으면 commit 버튼이 ‘Publish Branch’로 바뀜
    • 이 버튼을 클릭해도 Push 가능
    ★private인지 public인지만 선택하기(private는 자기자신만 볼수있음, public은 공유)★
![image](https://user-images.githubusercontent.com/35441691/224523458-9b41170d-0389-48ba-8760-59d19428c491.png)

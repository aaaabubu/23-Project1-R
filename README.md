# 안진홍 602377109

## [ 05월 25일 학습내용 ]
>오늘 배운 내용 정리

### 방사형 차트
방사형 차트(Radar Chart)는 어떤 측정 목표에 대한 평가항목이 여러 개일 때 항목 수에 따라 원을 같은 간격으로 나누고, 중심으로부터 일정 간격으로 동심으로 척도를 재는 칸을 나누어 각 평가항목의 정량화된 점수에 따라 그 위치에 점을 찍고 평가항목간 점을 이어 선으로 만들어 항목 간 균형을 한눈에 볼 수 있도록 해주는 차트입니다. 여러 측정 목표를 함께 겹쳐 놓아 비교하기에 편리하고 각 항목 간 비율뿐만 아니라 균형과 경향을 직관적으로 알 수 있어 편리함을 제공해주는 차트.

### 데이터 만들기

        > set.seed(99)
        > data <- as.data.frame(matrix( sample( 0:20 , 15 , replace=F) , ncol=5))
        > colnames(data) <- c("math" , "english" , "biology" , "music" , "R-coding" )
        > rownames(data) <- paste("mister" , letters[1:3] , sep="-")
        > data
         math english biology music R-coding
        mister-a   12      17      10    19        1
        mister-b    2       9       4     6       16
        mister-c   13      15      18     5       20


## [ 05월 18일 학습내용 ]
>오늘 배운 내용 정리

### 데이터 정령

#### sort( )
sort(x, decreasing = F) 를 이용해서 간단하게 가격을 오름차순 정렬

        > sort(v3)
        [1] 1000 1000 2000 2000 2000 3000 3000
        > sort(v3, decreasing = T)
        [1] 3000 3000 2000 2000 2000 1000 1000
       
#### order( )

        > order(v3)
        [1] 1 4 2 3 7 5 6
        > order(-v3)
        [1] 5 6 2 3 7 1 4

### 샘플링
많은 데이터 중 일부를 선택해야 할 때가 있음. 그 경우에 처리하는 기술을 샘플링이라고 함


## [ 05월 11일 학습내용 ]
>오늘 배운 내용 정리

### 겉측값 확인

        C1=c(1,2,NA,NA,5)
        C2=(1,2,3,4,5)
        C3=(NA,2,3,4,5)
        md=data.frame(C1,C2,C3)

        > is.na(md)
        C1    C2    C3
        [1,] FALSE FALSE  TRUE
        [2,] FALSE FALSE FALSE
        [3,]  TRUE FALSE FALSE
        [4,]  TRUE FALSE FALSE
        [5,] FALSE FALSE FALSE
   
### NA 제거

        C1=c(1,2,NA,NA,5)
        C2=(1,2,3,4,5)
        C3=(NA,2,3,4,5)
        md=data.frame(C1,C2,C3)
        
        > na.omit(md)
        C1 C2 C3
        2  2  2  2
        5  5  5  5

## [ 05월 04일 학습내용 ]
>오늘 배운 내용 정리

## 병결

## [ 04월 27일 학습내용 ]
>오늘 배운 내용 정리

## 막대그래프
### R에서 막대그리프를 그려주는 함수는 barplot()

        mydata=c(5,8,3)
        barplot(mydata,names=c("A","B","C"))

![image](https://user-images.githubusercontent.com/35441691/235650289-ed5a631e-925a-4cf4-8693-c7fb616361a2.png)


## [ 04월 20일 학습내용 ]
>오늘 배운 내용 정리

## 중간고사

## [ 04월 13일 학습내용 ]
>오늘 배운 내용 정리

read.table() : 텍스트 파일을 불러오고, 데이터 프레임 형식으로 저장 

### TXT 파일 가져오기
        ex_data <- read.table(“C:/Rstudy/data_ex.txt”, encoding = “EUC-KR”, fileEncoding = “UTF-8”)
        View(ex_data)
        
### CSV 파일 가져오기

        ex_data <-read.csv(“C:/Rstudy/data_ex.csv”)
        View(ex_data)
        
### 엑셀 파일 가져오기

        excel_data_ex <- read_excel("C:/Rstudy/data_ex.xlsx")
        View(excel_data_ex)

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

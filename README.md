# 안진홍 602377109

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

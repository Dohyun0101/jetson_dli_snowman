# jetson_dli_s

```bash```
# Jetson nano 장치 연결 및 준비
1. SD 카드 포멧터 다운 및 포멧팅
![1-3 필요도구 다운로드](https://github.com/user-attachments/assets/ade72f6c-d922-4bd4-80ad-e6ad813c2e12)
![1-3 설치 2](https://github.com/user-attachments/assets/cf5851d2-7e6c-4970-b679-ce271a02dbf3)
![1-3 설치사진3](https://github.com/user-attachments/assets/b18b7796-6f8c-4cf4-a750-6149a690cc95)
![1-3 설치사진 4](https://github.com/user-attachments/assets/1ee4fd79-a42f-4682-bae4-1c9da2e4dbe8)


2. jetack 링크로 다운로드
![1_2 jetack 설치 이미지](https://github.com/user-attachments/assets/915209fe-7cbe-4b54-b84b-d45abac22e76)

3. balanetcher 다운로드 및 이미지 굽기
![4번 사진](https://github.com/user-attachments/assets/50adc32a-db27-4ddd-839d-5ccf3d9a29e5)
![4번 사진 2](https://github.com/user-attachments/assets/a049155f-af38-429d-a637-6b647202a701)
![4번 사진 3](https://github.com/user-attachments/assets/9eece182-dae6-4eef-9394-3cd03d08953c)
![4번 4](https://github.com/user-attachments/assets/f0e8805f-6ca1-4be1-ad6e-ae0b0f26cb46)

4. jetsonnano 설명(introduction)
![introduction_jetson](https://github.com/user-attachments/assets/76397490-a768-4c8b-b19d-2cb48e1ebd49)

5. jetson nano에 sd 카드와 키보드 및 마우스 선, HDMI 선 연결

6. 와이파이 연결을 위한 안테나 2개 연결

# 한글 설치하기

1. 우분투 설치
   * 언어설정은 영어로
   * 와이파이 연결
   * 지역설정: seoul
   * name(dli), Password(dli) 설정
   * reboot 한 뒤 화면이 나타남.
2. 한글 설치
   * 시작 전 명령어 입력
     > 명령어
       ```bash
       sudo apt-get update
       dli@dli-desktop:~$ sudo apt-get install fcitx-hangul
       dli@dli-desktop:~$ im-config -n fcitx
       reboot
       ```
    * 우분투 setting
      1. Region & Language 수행
         <br>&rarr; Mange installed Language 버튼 실행<br>
         설치 완료 후 keyboard input method system 항목을 fcitx로 변경
      2. System rebooting
      3. 우측 상단의 키보드 아이콘 늘릭으러 configure 선택
         <img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FIdlr5%2FbtqwMLjQKJt%2FcVmuAK6Q9Mh86POcg5KYN0%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
      4. Input Method Configuration 에서 하단 "+" 버튼 클릭
         <img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FIdlr5%2FbtqwMLjQKJt%2FcVmuAK6Q9Mh86POcg5KYN0%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
      5. "Only Show Current Language"에 체크가 된 것을 해제 및 hangul 검색
          <img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FtX8Et%2FbtqwMJGj2Ku%2FTvy1C5hYGur9h6OTlH5dw1%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
      6. Input Method Configuration &rarr; Global Config &rarr; Trigger Input Method의 왼쪽 버튼 클릭 및 "한영키" 눌러서 언어 변경 
          <img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fk9mHo%2FbtqwKSdmDdI%2FSyxQUATWJdtf1bMFl62QdK%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
       7. "한영키" 눌러서 결과 확인
          <img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fo77V5%2FbtqwMJzxJkV%2Fr7mpuIQLjWnSDyXTjivzP0%2Fimg.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>


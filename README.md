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
         <br><img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FIdlr5%2FbtqwMLjQKJt%2FcVmuAK6Q9Mh86POcg5KYN0%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
         
      4. Input Method Configuration 에서 하단 "+" 버튼 클릭
         <br><img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FIdlr5%2FbtqwMLjQKJt%2FcVmuAK6Q9Mh86POcg5KYN0%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
         
      5. "Only Show Current Language"에 체크가 된 것을 해제 및 hangul 검색
          <img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FtX8Et%2FbtqwMJGj2Ku%2FTvy1C5hYGur9h6OTlH5dw1%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
          
      6. Input Method Configuration &rarr; Global Config &rarr; Trigger Input Method의 왼쪽 버튼 클릭 및 "한영키" 눌러서 언어 변경 
          <br><img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fk9mHo%2FbtqwKSdmDdI%2FSyxQUATWJdtf1bMFl62QdK%2Fimg.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
          
       7. "한영키" 눌러서 결과 확인
          <br><img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fo77V5%2FbtqwMJzxJkV%2Fr7mpuIQLjWnSDyXTjivzP0%2Fimg.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

  # 쿨링팬과 jtop
   <br> jtop: system monitoring tool <br>
   jetson nano의 온도체크
   ```bash
   sudo apt install python3-pip
   sudo -H pip3 install -U jetson-stats
   sudo apt-get upgrade
   reboot
   jtop
   ```
   <br>![스크린샷 2024-11-21 210653](https://github.com/user-attachments/assets/adca3433-e928-4890-b4bb-bff0d425fd3c)<br/>
   
   <br> jetson nano에 쿨링팬 장착 <br>
   <br>![image](https://github.com/user-attachments/assets/dec02a53-5949-496a-9c7b-07637a209e45)<br/>

   terminal을 열고 명령어 작성
   ```bash
    sudo sh -c 'echo 128 > /sys/devices/pwm-fan/target_pwm'
   ```

  # Camera
  1. jetson 의 카메라 인식 확인
     ```bash
     ls /dev/vi*
     ```
  2. gitclone cloning
     ```bash
      git clone https://github.com/jetsonhacks/USB-Camera.git
     ```
     [result]
     ```bash
     Cloning into 'USB-Camera'...
      remote: Enumerating objects: 27, done.
      remote: Counting objects: 100% (27/27), done.
      remote: Compressing objects: 100% (24/24), done.
      remote: Total 27 (delta 11), reused 8 (delta 2), pack-reused 0
      Unpacking objects: 100% (27/27), done.
     ```
  3. Camera 작동 확인
     [code]
     ```bash
     cd USB-Camera
     ```
     ```bash
     ~/USB-Camra$ ls
     ```
     [result]
     ```bash
     face-detect-usb.py  LICENSE  README.md  usb-camera-gst.py  usb-camera-simple.py
     ```
     
     [code]
     ```bash
     python3 usb-camera-gst.py
     ```

# Dockor 설치
  1. CODE
  ```bash
  ls
  ```
  ```bash
  Desktop    examples.desktop  Public
  Documents  Music             Templates
  Downloads  Pictures          Videos
  ```
  교육과정에 필요한 dir 추가
  ```bash
  mkdir -p ~/nvdli-data
  ls
  ```
  ```bash
  Desktop           Music       Templates
  Documents         nvdli-data  Videos
  Downloads         Pictures
  examples.desktop  Public
  ```

  ```bash
  sudo docker run --runtime nvidia -it --rm --network host \
    --memory=500M --memory-swap=4G \
    --volume ~/nvdli-data:/nvdli-nano/data \
    --volume /tmp/argus_socket:/tmp/argus_socket \
    --device /dev/video0 \
    nvcr.io/nvidia/dli/dli-nano-ai:v2.0.2-r32.7.1kr
  ```
  ```bash
  ls
  ```

  ```bash
  ./docker_dli_run.sh
  ```
  ```bash
  [sudo] password for dli:
  Unable to find image 'nvcr.io/nvidia/dli/dli-nano-ai:v2.0.2-r32.6.1kr' locally
  v2.0.2-r32.6.1kr: Pulling from nvidia/dli/dli-nano-ai
  b9bb7af7248f: Pulling fs layer
  2e163bfa50fc: Download complete
  c8bd4a89e71c: Pulling fs layer
  0a8ce4f08307: Waiting
  334a570c08f5: Downloading  5.855MB/165.2MB  ~~~~~~
  ```

  [result]
  ```bash
  0be277f6cdcf: Pull complete
  561a3bf4f244: Pull complete
  2a5d5ea0506f: Pull complete
  ed5b8317fa2e: Pull complete
  Digest: sha256:87d580feed4a9670dfe343cf352239065ff9c7789cfa3a3b36adf828b7e50ac0
  Status: Downloaded newer image for nvcr.io/nvidia/dli/dli-nano-ai:v2.0.2-r32.6.1kr     allow 10 sec for JupyterLab to start @ http://192.168.55.1:8888 (password           
  dlinano)c932e62bbab: Waiting
  JupterLab logging location:  /var/log/jupyter.log  (inside the container)
  root@dli-desktop:/nvdli-nano#
  ```

  2. Web browser 내의 주소창 입력
     ```bash
     192.168.55.1:8888
     ```



# Thumbs Project
1. image classification project

   주피터 노트북에 있는 모든 셀을 실행한다.
   
2. 데이터 셋 만들기
   <br>![image](https://github.com/user-attachments/assets/f91e81fd-8731-4daa-9e72-42975960e0a0)<br/>
   1) 위의 그림과 같이 A, B Dataset으로 나누어서 카메라로 직접 thumbs up/ down 직접 수집한다.
   2) 수집한 Dataset을 기반으로 모델을 훈련시킴
   3) 훈련시킨 모델의 성능을 확인해보기 위해 카메라에 thumbs up/ down 동작을 취해서 확인해본다.

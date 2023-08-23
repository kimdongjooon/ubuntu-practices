- sh -
1. java JDK 다운
  명령어 입력.
  wgt https://download.oracle.com/java/17/archive/jdk-17.0.7_linux-aarch64_bin.tar.gz

2. 압축 풀기.
  tar xvfz jdk-17.0.7_linux-aarch64_bin.tar.gz

3. poscodx 소프트웨어 설치 디렉토리 만들기.
  # mkdir /user/local/poscodx2023

4. 설치 
  sudo mv ./jdk-17.0.7 /usr/local/poscodx2023/java17

5. 링크파일 생성
  ln -s /usr/local/poscodx2023/java17 /usr/local/poscodx2023/java
  ls -l /usr/local/poscodx2023/

6. 설정(etc/profile)
  # java
  export JAVA_HOME=/usr/local/poscodx2023/java
  export CLASSPATH=$JAVA_HOME/lib/*
  export PATH=$PATH:$JAVA_HOME/bin

7. 현재 shell 환경에 적용
  source /etc/profile

8. 확인.
  java --version

9. 파일 실행
  javac hello.java
  java -cp . hello
  
   

## Maven 3.8.7
1. 작업 디렉토리
```sh
   /root
```
2. 다운로드
```sh
   # wget https://dlcdn.apache.org/maven/maven-3/3.8.8/binaries/apache-maven-3.8.8-bin.tar.gz
```

3. 압축 풀기
```sh
   # tar xvfz apache-maven-3.8.8-bin.tar.gz
```
4. 설치
```sh
   # mv apache-maven-3.8.8 /usr/local/poscodx2023/maven3.8
   # ln -s /usr/local/poscodx2023/maven3.8 /usr/local/poscodx2023/maven
```
5. 설정(/etc/profile)
```sh
# maven
export PATH=$PATH:/usr/local/poscodx2023/maven/bin
```

6. 확인
```sh
# mvn --version
Apache Maven 3.8.8 (4c87b05d9aedce574290d1acc98575ed5eb6cd39)
Maven home: /usr/local/poscodx2023/maven
Java version: 17.0.7, vendor: Oracle Corporation, runtime: /usr/local/poscodx2023/java17
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "6.2.0-27-generic", arch: "aarch64", family: "unix"
```

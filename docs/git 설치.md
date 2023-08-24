git 2.9.5 설치

1. 의존성 라이브러리
```sh
   # yum install curl-devel
   # yum install expat-devel
   # yum install gettext-devel
   # yum install openssl-devel
   # yum install zlib-devel
   # yum install perl-devel
```
3. 다운로드
```sh
   # wget https://mirrors.edge.kernel.org/pub/software/scm/git/git-2.9.5.tar.gz
```
5. 압축 풀기
```sh
  # tar xvfz git-2.9.5.tar.gz
```
4.소스 디렉토리
```sh
  # cd git-2.9.5
  # pwd
```
5. configure
```sh
  # ./configure --prefix=/usr/local/poscodx2023/git
```
6. 빌드
```sh
  # make all
```
7. 설치
```sh
  # make install
```
8. 설정(/etc/profile)
```sh
# git
export PATH=$PATH:/usr/local/poscodx2023/git/bin
```
8-1/
```sh
mv /usr/bin/git /usr/bin/git_old
ln -s /usr/local/poscodx2023/git/bin/git /usr/bin/git
```

9. git 확인
```sh
# git --version
```
10. git 사용하기
```sh
# mkdir my-workspace
# cd my-workspace
# mkdir centos-practices
# cd centos-practices
# git init
# git add -A
# git commit -m "first commit"
# git branch -M main
# git remote add origin https://github.com/douzone-bipa/centos-practices.git
# git push -u origin main

================
# git add -A
# git commit -m "...."
# git push 


=========================================================


# git clone https://github.com/douzone-bipa/javastudy.git
# cd javastudy
# mvn clean package
```









  








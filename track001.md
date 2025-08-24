
[ 실습1 ]    
1.  회원가입(https://github.com/) 후 로그인
2.  원격저장소 만들기  
https://github.com/sally03915/git0.git

[ 실습2 ]   
1.  https://git-scm.com/
2.  설치

[ 실습3 ]   git
1.  유저이름
$ git  config  --global   user.name "sally An"

2.  github 가입시 사용한 이메일
$ git  config  --global   user.email  "sally03915@gmail.com"

3.  github  설정확인
$  git  config --list

>>>>>> CODE
Administrator@User -2023CNVKK MINGW64 ~
$ git  config  --global   user.name "sally An"

Administrator@User -2023CNVKK MINGW64 ~
$ git  config  --global   user.email  "sally03915@gmail.com"

Administrator@User -2023CNVKK MINGW64 ~
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=sally An
user.email=sally03915@gmail.com


[ 실습4 ]   폴더만들고  visual studio 로 열기
1.  폴더만들기 - mkdir   git0
C:\Users\Administrator.User -2023CNVKK>cd C:\
C:\>dir
C:\>mkdir  git0
C:\>dir
C:\>cd  git0
C:\git0>code .


2.  터미널 열기 - 
[Terminal]  - [New Terminal]

3. basic001.html   파일만들기

4. git
PS C:\git0> git init               설명)   저장소 초기화
Initialized empty Git repository in C:/git0/.git/
PS C:\git0>   ※ backup 하고
PS C:\git0> git  add  .           설명) 추가할 파일 확인     . 모든파일
		               설명) git   add  basic001.html
PS C:\git0> 
PS C:\git0> git  status          설명)   상태확인
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   basic001.html

PS C:\git0> git  commit  -m  "first  commit"       설명)기록남기기 
[master (root-commit) 1b33931] first commit
 1 file changed, 11 insertions(+)
 create mode 100644 basic001.html
PS C:\git0>  
PS C:\git0>  설명)     내 로컬저장소와   원격저장소 연결
PS C:\git0> git  remote  add   origin  https://github.com/sally03915/git0.git
PS C:\git0> 
PS C:\git0>  설명)    연결확인
PS C:\git0> git  remote  -v
origin  https://github.com/sally03915/git0.git (fetch)
origin  https://github.com/sally03915/git0.git (push)
PS C:\git0> 
PS C:\git0> 설명) 원격저장소로 올리기
PS C:\git0> git  push  origin  master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 379 bytes | 379.00 KiB/s, done.      
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/sally03915/git0.git
 * [new branch]      master -> master
PS C:\git0>


5. github에가서 원격저장소에 올라간것 확인


※ error 시
 remote: Permission to newaccount/projectname.git denied to oldaccount.
fatal: unable to access 'https://github.com/newaccount/projectname.git/': The requested URL returned error: 403 

1. 제어판
다음 Windows 자격 증명에 들어가면
일반 자격 증명 탭에 기존에 사용하던 토큰들이 있을 것입니다.
 
step1) git:https://githubs.com 없다면 .....  사용자계정 추가
git:https://githubs.com
사용자이름 : sally03915
암호: github접속시 홈페이지 접속암호

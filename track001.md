## 🧪 실습 1: GitHub 회원가입 및 원격 저장소 생성

1. [GitHub](https://github.com/)에 회원가입 후 로그인  
2. 원격 저장소 생성  
   - 저장소 주소: `https://github.com/sally03915/git0.git`

---

## 🧪 실습 2: Git 설치

1. [Git 공식 사이트](https://git-scm.com/) 접속  
2. Git 다운로드 및 설치

---

## 🧪 실습 3: Git 사용자 정보 설정

### 🔧 사용자 정보 등록
```bash
$ git config --global user.name "sally An"
$ git config --global user.email "sally03915@gmail.com"
```

### 🔍 설정 확인
```bash
$ git config --list
```

📋 예시 출력:
```bash
user.name=sally An
user.email=sally03915@gmail.com
...
```

---

## 🧪 실습 4: 프로젝트 폴더 생성 및 Git 초기화

### 📁 폴더 생성 및 VS Code로 열기
```bash
C:\> mkdir git0
C:\> cd git0
C:\git0> code .
```

### 🖥️ VS Code에서 터미널 열기
- 메뉴: [Terminal] → [New Terminal]

### 📄 파일 생성
- `basic001.html` 파일 생성

### 🧵 Git 저장소 초기화 및 커밋
```bash
PS C:\git0> git init                     # 저장소 초기화
PS C:\git0> git add .                   # 모든 파일 추가
PS C:\git0> git status                  # 상태 확인
PS C:\git0> git commit -m "first commit"  # 첫 커밋
```

### 🌐 원격 저장소 연결 및 푸시
```bash
PS C:\git0> git remote add origin https://github.com/sally03915/git0.git
PS C:\git0> git remote -v               # 연결 확인
PS C:\git0> git push origin master      # 원격 저장소로 푸시
```

### ✅ GitHub에서 업로드 확인

---

## ⚠️ 오류 발생 시 대처 방법

### ❌ 오류 메시지 예시
```bash
remote: Permission to newaccount/projectname.git denied to oldaccount.
fatal: unable to access 'https://github.com/newaccount/projectname.git/': The requested URL returned error: 403
```

### 🛠️ 해결 방법
1. 제어판 → Windows 자격 증명 → 일반 자격 증명 탭 확인  
2. 기존 GitHub 토큰 삭제 또는 새 사용자 계정 추가

#### 🔐 사용자 계정 추가 예시
- 항목: `git:https://github.com`
- 사용자 이름: `sally03915`
- 암호: GitHub 로그인 시 사용하는 비밀번호

<<<<<<< HEAD

---

## 🧪 실습 5: pull & push  [chapter002]

### 실습 시나리오
1. GitHub에서 track001.md 파일을 수정
2. 로컬에서도 같은 파일을 수정 후 커밋
```bash
git  add  track001.md
git commit -m "chapter2-1.  track001.md"
git pull origin master 
```

3. 실행 시 충돌 발생
```bash
PS C:\◎stackventure_250825◎\test-local> git pull  origin master
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 976 bytes | 19.00 KiB/s, done.
From https://github.com/sally03915/stackventure_test_250825
 * branch            master     -> FETCH_HEAD
   d14869c..10d4b45  master     -> origin/master
error: Your local changes to the following files would be overwritten by merge:
        track001.md
Please commit your changes or stash them before you merge.
Aborting
Merge with strategy ort failed.
PS C:\◎stackventure_250825◎\test-local>
```
=======
---

## 🧪 실습 5: pull & push
### 🛠️  pull
```bash
git pull origin master
```

>>>>>>> 10d4b45faf7f8dc50e8864845bc398e4b1da1c1a


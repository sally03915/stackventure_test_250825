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

---

## 🧪 실습 5: pull & push
### 🛠️  pull
```bash
git pull origin master
```



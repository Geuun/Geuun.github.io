---
title: "[Git] gitignore 설정법"
categories:
  - Git
tags:
  - Git
toc: false
toc_sticky: false
toc_label:
published: true
---

# 목차

1. .gitignore 이란?
2. .gitignore 를 사용해야하는 이유는 무엇일까?
3. .gitignore File 생성 / 적용
4. 간단하게 .gitignore File 생성하는 방법

### 1. .gitignore이란?

`.gitignore 의 개념`

- 프로젝트 작업시 로컬 환경의 정보나 빌드 정보등 원격 저장소에서 추적(Tracking) 하지 말아야되는 파일에 대해서 미리 List를 작성하고, Git이 List를 참고해서 추적하지 않도록 관리하는 파일
- git이 파일을 추적할 때, 어떤 파일이나 폴더 등을 추적하지 않도록 명시하기위해 작성하며, 해당 문서에 작성된 List는 수정사항이 발생해도 git이 무시하게된다.
- 특정 파일 확장자를 무시하거나 이름에 패턴이 존재하는 경우, 또는 특정 디렉토리 아래의 모든 파일을 무시할 수 있다.

### 2. .gitignore 를 사용해야하는 이유는 무엇일까?

- git을 활용해 여러사람과 협업을 진행하게되면 원격저장소에 관리하지 않아도 될 파일들이 올라가는 경우  
  (예로들면 jupyter notebook을 사용하면 자동으로 생성되는 .ipycheckpoint_checkpoints 등)
- git을 활용해 여러사람과 협업을 진행 중 원격저장소에 올라가면 충돌이 일어날 수 있는 여지가 있는 파일들이 있는 경우
- 원격저장소에 업로드하면 안되는 파일이 있을 때  
   (예로들면 django의 SECRETKEY가 포함된 settings.py File)

즉, 간단하게 말하면 원격저장소에 올라가는 안되는 파일을 선택적으로 미리 List를 만들어 놓는것이다.

### 3. .gitignore File 생성

📝 작성방법

- '#'로 시작하는 라인은 무시한다.
- 표준 Glob 패턴을 사용한다.
- 슬래시(/)로 시작하면 하위 디렉터리에 적용되지(recursivity) 않는다.
- 디렉터리는 슬래시(/)를 끝에 사용하는 것으로 표현한다.
- 느낌표(!)로 시작하는 패턴의 파일은 무시하지 않는다.

참고문헌 : [Git 공식 github](https://github.com/github/gitignore)

✏️ Example

```markdown
# ignore all .class files

\*.class

# exclude lib.class from "\*.class", meaning all lib.class are still tracked

!lib.class

# ignore all json files whose name begin with 'temp-'

temp-\*.json

# only ignore the build.log file in current directory, not those in its subdirectories

/build.log

# specify a folder with slash in the end

# ignore all files in any directory named temp

temp/

# ignore doc/notes.txt, but not doc/server/arch.txt

bin/\*.txt

# ignore all .pdf files in the doc/ directory and any of its subdirectories

# /\*\* matches 0 or more directories

doc/\*_/_.pdf
```

**기본적인 .gitignore 파일을 작성했다면 Github 원격저장소에 적용해보도록하자.**

### 3-1. .gitignore 파일 적용

이미 원격저장소에 올라가있는 파일은 git 시스템에 의해 추적(Tracking) 당하고(🤔?) 있는 중이다.
이때는 아래의 코드를 입력해서 추적을 끊고 앞으로 추적 되지않도록 하자.

```markdown
$git rm -r --cached .
$git add.
$git commit -m "커밋메세지"
$git push origin {브랜치명}
```

## 위 코드를 적용하면 원격저장소에서 .gitignore File List에 등록해둔 파일 또는 디렉토리가 사라진 것을 확인할 수 있을것이다.

### 4. 간단하게 .gitignore File 생성하는 방법

일일히 .gitignore 파일을 작성하는 방법도 있겠지만 개발자들은 귀찮은걸 싫어한다.
따라서 당연히 자신의 개발환경을 입력하면 거기에 알맞는 .gitignore 파일을 생성해주는 사이트가 있다.

[https://www.gitignore.io/](https://www.gitignore.io/) 에 접속해보자!
접속했다면 자신의 현재 개발환경에 알맞는 키워드를 입력하고 생성버튼을 눌러주면 알맞는 .gitignore 파일을 생성해준다!

---

{: .notice--success}

✏️**마무리하며**  
원격저장소를 혼자 사용한다면 .gitignore 파일을 사용하지 않아도 되지만,  
자신이 여러사람과 협업하는 상황이라면 프로젝트 초반단계에 간단하게라도
.gitignore 파일을 생성해두면 불필요한 충돌상황을 피할 수 있을것 같다.

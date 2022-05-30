---
title: "[Python] File “<stdin>”, line 1 SyntaxError: invaild syntax"
categories:
  - Python
tags:
  - Error
toc: false
toc_sticky: false
toc_label:
published: true
---

```shell
[Python] File “<stdin>”, line 1 SyntaxError: invaild syntax
```

이번 포스트는 개인 미니 프로젝트 진행 중 발생한 에러에 대해 기록해보려한다.

SyntaxError라고 해서 내 코드에 이상이 있는 줄 알았지만
아무리 눈씻고 디버깅을 해봐도 SyntaxError가 나왔다.

바로 만인의 선생님 구글선생님께 물어보았더니 손 쉽게 찾을 수 있었다.

### 오류 발생이유

> 이미 실행되어있는 파이썬 인터프리터 내부에서 파이썬을 다시 실행시켜서 발생하는 오류이다.

파이썬이 실행 중인 인터프리터에서는 입력 커서 앞부분이

`>>>` 모양으로 바뀌니 참고하자.

### 해결방법

1. code-runner 실행 설정에서 파이썬 항목을 아래와 같이 바꿔준다

```python
"code-runner.executorMap": {

        "python": "set PYTHONIOENCODING=utf8 | py"
        }
```

2. `exit()` 혹은 Ctrl+Z 를 입력해주자.

[참고 문헌]

- [https://stackoverflow.com/questions/13961140/syntax-error-when-using-command-line-in-python](https://stackoverflow.com/questions/13961140/syntax-error-when-using-command-line-in-python)

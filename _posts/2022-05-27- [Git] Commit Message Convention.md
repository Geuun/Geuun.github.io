---
title: "[Git] Commit Message Convention"
categories:
  - Git
tags:
  - Git
toc: false
toc_sticky: false
toc_label:
published: true
---

# [git] Commit Message Convention이란?

> 프로젝트를 진행하면서 버전관리와 협업의 목적으로 Git을 사용하는 것이 일반적 일텐데 누군가 알아볼 수 없는 메세지로 Commit 을 한다면 무엇이 어떻게 바뀌었는지 한 눈에 알아보기가 힘들 것이다.
> 따라서 Commit Message를 일관성있게 써서 누구나 알아볼 수 있도록 하는것이 Git Commit Message Convention의 목표이다.

---

그렇다면 일관성있는 Commit Message는 어떻게 작성할까?
이것은 팀 / 회사마다 다르고 구성원이 정한 약속하에 누구나 알아볼 수 있게 쓰면 된다.
하지만 개인이 혼자 사용하는 레포의 Commit Message를 작성할 때에도 일관성 있게 작성하는 것이 기본적으로 좋다.
따라서 앞으로 나는 굉장히 많은 사람들이 참고로 하는 Udacity의 Commit Message Convention 을 참고해서 Commit Message 를 작성하려고 한다.

<[Udacity Nanodegree Style Guide](https://udacity.github.io/git-styleguide/)>

공식문서를 살펴보자.

- 기본 Message Structure

```bash
type: Subject

body

footer
```

모든 내용은 전세계 누가봐도 알아볼 수 있게 영어로 작성하는 것을 원칙으로 한다.

1. Commit type

- feat : 새로운 기능 추가
- fix : 버그 수정
- docs : 문서 수정
- style : 코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우
- refactor : 코드 리펙토링
- test : 테스트 코드 및 리펙토링 테스트 코드 추가
- chore : 빌드 업무 수정 및 패키지 매니저 수정

위의 type 중 혼자 작업하며 가장 많이 쓰게될 것은 아마 feat, fix, docs, refactor 정도가 아닐까 싶다.

1. Commit Subject

- Commit 의 제목이라고 생각하면 된다.
- 제목은 간결하게 50자 이내로 작성하고 추가로 설명이 필요한 내용은 Body에 적는다.
- 과거시제를 사용하지 않고 명령어로 작성한다.
  - Fixed → Fix
  - Added → Add

1. Body

- Subject에서 추가로 설명이 필요하면 Body에 작성한다.
- 선택사항이므로 모든 Commit에 작성할 필요는 없다.
- 72자를 넘기지 않고 제목과 구분되기 위해 한칸을 띄워서 작성한다.

1. Footer

- Commit의 꼬리말이라고 생각하면 된다.
- issue tracker id를 작성할 때에는 footer에 작성하면 된다.
- 선택사항이며 마찬가지로 모든 Commit에 작성할 필요는 없다.

1. Example : 참고 문헌 인용

```bash
feat: Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```

정리 및 요약

> 여러 사람과 협업할 때에 Commit Message Convention은 필수적으로 정해야 할 것 같다.
> 여러사람이 Commit Message를 작성하는 방식이 다 다를 것이기 때문에 모든 팀원 과 팀원이외에 사람도 Commit Message를 통해 변경사항을 알아볼 수 있도록 간결하게 알아 볼 수 있도록 작성하는 것이 중요하다.

---
layout: post
title: ".gitignore가 일해주지 않을 때"
author: "Ahreum Han"
---

git repository를 옮기는 상황이 생겼다.
아차 싶어서 나중에야 .gitignore 를 부랴부랴 추가했는데
아무리 새로 작성하고 generator 서비스의 도움까지 받아봐도 무시해주길 바라는 파일들 대신에 내 부탁을 무시했다.

***

이럴때 터미널에서
```
git rm -r --cached .
git add .
git commit -m "fixed untracked files"
```
라고 명령해주면 .gitignore가 제대로 적용된다.

간단한 것들 기록 해둬야지.

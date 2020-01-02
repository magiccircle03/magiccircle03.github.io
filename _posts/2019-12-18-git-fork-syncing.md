---
title: "원본 저장소의 변경 내역을 포크한 저장소로 가져오기"
date: 2019-12-18
categories: git
---

```bash
// 포크 저장소를 로컬로 클론
$ git clone https://github.com/magiccircle03/myrepository.git


// 로컬 저장소로 이동
$ cd myrepository


// 현재 설정된 리모트 저장소 조회
$ git remote -v
origin	https://github.com/magiccircle03/myrepository.git (fetch)
origin	https://github.com/magiccircle03/myrepository.git (push)


// 리모트 저장소 추가
$ git remote add upstream https://github.com/원본id/myrepository


// 리모트 저장소 확인
$ git remote -v
origin	https://github.com/magiccircle03/myrepository.git (fetch)
origin	https://github.com/magiccircle03/myrepository.git (push)
upstream	https://github.com/원본id/myrepository (fetch)
upstream	https://github.com/원본id/myrepository (push)


// 리모트 저장소 fetch
$ git fetch upstream


// 리모트 저장소 merge
$ git merge upstream/master


// 포크 저장소로 push
$ git push

```

[참고 링크](https://hyunjun19.github.io/2018/03/09/github-fork-syncing/)

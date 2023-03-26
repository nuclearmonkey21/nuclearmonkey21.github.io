---
title: "[Git]#1 Git 기본 명령어 모음"
excerpt: "Git 기본 명령어를 알아보자!"

categories:
  - Git
tags:
  - Git

toc: true
toc_sticky: true

date: 2023-03-26
last_modified_at: 2023-03-26
---

# 0. Git 기본 용어
---
`저장소(Repository)`: 개발자의 작업 폴더들과 Git의 주요 정보등을 담고 있는 저장 공간  
<br>
`원격 저장소(Remote Repository)`: 로컬 저장소를 업로드하는 서버의 저장 공간`git push`  
<br>
`로컬 저장소(Local Repository)`: 사용자의 PC에서 관리하는 Git의 저장 공간`git commit`  
<br>
`스테이징 영역(Staging Area)`: 작업 폴더(Working Directory)에서 변경된 사항을 로컬 저장소(Local Repository)에 전달하기 위해 기록되는 공간 Git에서는 `Index`라고 명명됨 `git add`  
<br>
`작업 폴더(Working Directory)`: 개발자의 실제 작업 공간 Git에서 관리는 하지만 추적은 하지 않는다. 
<br>
`Head`: 현재 작업중인 브랜치의 최근 커밋된 위치
<br>
![image](/assets/images/git/1/0.webp) 
<br><br>


# 1. Git 기본 명령어
---
<br>

| 명령어 | 옵션 | 설명 ex) ... |
|---|---|---|
| git init || Local Repository `생성` 및 기존 Local Repository `초기화` <br> ex) git init |
| git clone \<repo\> || Remote Repository를 Directory에 복제 <br> ex) git clone http://... |
| git status || 작업 트리 상태 표시 <br> ex) git status |
| git add || 인덱스(Staging Area)에 파일 내용 추가 |
|| ., -A, --all | 모든 추적 및 추적되지 않은 파일에서 변경 사항을 추가 <br> ex) git add --all |
|| \<pathspec\> | 단일 파일에서 변경 사항을 추가 <br> ex) git add --all  |
| git commit || Local Repository에 변경 사항 기록 |
|| -m, --message \<message\> | 짧은 변경 사항 기록 <br> ex) git commit -m "First Commit" |
| git push \<remote\> \<branch\> || Remote Repository에 변경 사항을 업데이트 <br> ex) git push origin master |
| git branch || Branch  목록 출력 <br> ex) git branch |
|| \<branch-name\> | Branch 생성 <br> ex) git branch newbranch |
|| -d, --delete \<branch-name\> | Branch 삭제 <br> ex) git branch -d newbranch |
| git checkout \<branch-name\> || Branch 이동 <br> ex) git checkout newbranch |
| git remote || Remote Repository 연결 목록 출력 <br> ex) git remote|
|| add \<name\> \<url\> | Remote Repository 연결 추가 <br> ex) git remote add origin http://... |
|| remove \<name\> | Remote Repository 연결 해제 <br> ex) git remote remove origin |
| git merge \<branch-name\> || Branch 병합 <br> ex) git merge newbranch |
| git pull \<url\> | Repository 또는 Local Branch에서 작업 데이터를 가져와서 통합 <br> ex) git pull http://... |

<br><br>






<br><br>

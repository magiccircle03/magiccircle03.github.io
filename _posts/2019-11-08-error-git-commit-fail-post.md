---
title: "[git] commit failed - exit code 128 received, with output"
date: 2019-11-08
categories: error
---
## 발생 문제
깃허브 데스크탑에서 커밋하다 다음과 같은 에러가 발생했다.
![commit_error_img](https://user-images.githubusercontent.com/51072198/68484673-15eb4b80-0281-11ea-8372-9d60808f7b5f.png)

## 해결법
1. 옵션-git 에 들어가 이메일을 다시 입력하고 save -> 실패
![email_save](https://user-images.githubusercontent.com/51072198/68484817-62cf2200-0281-11ea-8402-ac602dd91eca.png)

2. 위와 같지만 직접 명령 -> 실패
[https://stackoverflow.com/questions/47461612/commit-failed-exit-code-128-received](https://stackoverflow.com/questions/47461612/commit-failed-exit-code-128-received)

**3. `git config --global commit.gpgsign false` -> 성공**
[https://stackoverflow.com/questions/47461612/commit-failed-exit-code-128-received](https://stackoverflow.com/questions/47461612/commit-failed-exit-code-128-received)


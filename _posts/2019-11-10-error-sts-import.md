---
title: "[STS] Spring maven project import 후 에러가 날 때"
date: 2019-11-10
categories: error
---

## 1. 발생 문제

GitHub Desktop을 이용하여 프로젝트를 Clone 한 뒤, STS에서 import했을 때 실행하면 에러가 나는 경우가 있다.<br>
자바 버전을 맞춰주고, Dependencies 설정을 해주면 해결된다.

## 2. 문제 해결 

0. 프로젝트 오른쪽 클릭 - Properties 

1. Java Build Path - Libraries - JRE System Library - Edit 
![import3](https://user-images.githubusercontent.com/51072198/68544173-c84b1c00-0403-11ea-91d2-a645c0972277.png)
  
2. Java Compiler - Compiler compliance level 도 맞춰준다.
![import4](https://user-images.githubusercontent.com/51072198/68544190-eb75cb80-0403-11ea-9941-74684f10a606.png)
  
3. DeployAssembly - Add - Java Build Path Entries - Maven Dependencies - Finish
![import1](https://user-images.githubusercontent.com/51072198/68544290-fbda7600-0404-11ea-8c0a-e6cc553a0ac6.png)

4. Spring - Dependency Management - Automatically update dependencies from Maven pom.xml
![import2](https://user-images.githubusercontent.com/51072198/68544323-4cea6a00-0405-11ea-9a9c-69fc7aa520ad.png)


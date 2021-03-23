---
layout: single
title: "MVC, MVP, MVVM 디자인 패턴 비교"
read_time: true

categories: 
 - etc
tags: 
 - android	
 - mvc
 - mvp
 - mvvm
last_modified_at: '2021-03-23 23:36:00 +0800'
toc: true
toc_sticky: true
toc_label: 목차

---
## MVC, MVP, MVVM 디자인 패턴은 왜 필요한가?
프로그램의 크기가 점점 커짐에 따라 코드의 관리가 어렵고 유지보수와 개발효율이 떨어지게 되는데, 
이를 개선하기 위해 역할에 따라 코드를 분리시켜 관리하는 프레임워크 패턴이 사용되게 됩니다.

### MVC 패턴 :  Model + View + Controller
> Model 
> 프로그램에서 사용되는 데이터와 데이터를 처리하는 부분. 
> View
> 사용자에게 보여지는 UI 부분. 웹페이지나 모바일어플의 화면.
> Controller
> 사용자의 입력을 받고 처리하는 부분.
![image](https://user-images.githubusercontent.com/66898243/112164023-e8623080-8c30-11eb-9ec3-28e69e8cdebd.png)
> 1. 사용자가 입력 
> 2. Controller에서 사용자의 입력을 확인하고 Model 업데이트
> 3. Controller에서 Model을 나타낼 View를 선택
> 4. View는 Model을 이용하여 화면 출력

-----
### MVP 패턴 :  Model + View + Presenter
> Model 
> 프로그램에서 사용되는 데이터와 데이터를 처리하는 부분. 
> View
> 사용자에게 보여지는 UI 부분. 웹페이지나 모바일어플의 화면.
> Presenter 
> View에서 요청한 정보를 Model로부터 가공해서 View로 전달하는 부분
![image](https://user-images.githubusercontent.com/66898243/112163971-db454180-8c30-11eb-82d1-1f5cbabdd165.png)
> 1. 사용자가 입력
> 2. View에서 Presenter에게 데이터를 요청
> 3. Presenter에서 Model에게 데이터를 요청
> 4. Model은 Presenter에게 데이터를 응답
> 5. Presenter는 View에게 데이터를 응답
> 6. View는 응답받은 데이터를 이용하여 화면 출력

-----
### MVVM 패턴 :  Model + View + ViewModel




## 참고
https://magi82.github.io/android-mvc-mvp-mvvm/
https://velog.io/@jojo_devstory/%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C-%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98-%ED%8C%A8%ED%84%B4-MVVM%EC%9D%B4-%EB%AD%98%EA%B9%8C
https://beomy.tistory.com/43
https://jcchu.medium.com/%EB%94%94%EC%9E%90%EC%9D%B8-%ED%8C%A8%ED%84%B4-mvc-mvp-mvvm-965e324742df
https://www.thekpop.net/2020/03/design-pattern-04-mvc-mvp-mvvm-3.html

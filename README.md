# 항해 99 주특기 2주차 개인 과제 - 로그인 사용자용 매거진 웹 사이트 만들기  :diamond_shape_with_a_dot_inside:
***

## 개발자 :bust_in_silhouette:
### 이름 : 김윤민   :rose:  
### Email : dbsalszz@naver.com :email: :love_letter:
***
## 사용 기술 :computer:
<img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white"> -version : Java 8, JDK 11.0.13 </br>
          - Java 11이 아닌 Java 8을 사용한 이유</br>
          - 외부 개발 툴과의 연동성에서 더 안정적이다.</br>
          - Maven이나 Gradle같은 내부 빌드 툴이 가장 안정적인 버전</br>
</br>
<img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"></br>
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"></br>
<img src="https://img.shields.io/badge/jquery-0769AD?style=for-the-badge&logo=jquery&logoColor=white"></br>
<img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white"> -version : 8.0.27.</br>
<img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white"></br>

***
## 주요 기능 :cherry_blossom:
### :seedling: 로그인, 회원가입
### :seedling: 게시글 전체 조회, 검색 조회, 등록, 수정, 삭제
### :blossom: 좋아요, 좋아요 취소
          
***
## API  :barber:
|분류|기능|URL|Method|Request|Response|
|:-----|:-----|:-----|:-----|:-----|:-----|
|회원관리|:white_check_mark:회원가입|/api/register|POST|{“username” : 이메일, </br> password” : 비밀번호, </br> “passwordCheck”:비밀번호확인, </br> “nickName”: 별칭}|{“result” : True, False, </br> ”msg” : “msg”}|
| |:white_check_mark:로그인|/api/register|POST|{“username” : 이메일, </br> “password”: 비밀번호}|{“result” : True, False, </br> ”msg” : “msg”,  </br> “username”: username, </br> ”nickName”:nickname,}|
|게시글|:white_check_mark:등록|/api/post|POST|{“nickName” : 사용자이름,  </br> “contents” : 내용, </br> ”image”:이미지경로, </br> “type”: “full”, ”right”, ”left”}|{“result” : True, False, </br> ”msg” : “msg”}|
||:white_check_mark:조회|/api/post|GET|{”username”:회원아이디 (이메일형식)}| {"total":[전체 게시글 목록],  </br> "myLike":[내가 좋아요한 게시글 목록]} |
||:white_check_mark:수정|/api/post|PUT|{수정된 게시글 정보}|{“result” : True, False, </br> ”msg” : “msg”}|
||:white_check_mark:삭제|/api/post|DELETE|{”postId”:게시글 번호}|{“result” : True, False,  </br> ”msg” : “msg”}|
|좋아요|:white_check_mark:게시글 좋아요|/api/like|POST|{”postId”:게시글 번호, </br> ”userId”:사용자 ID} |{“result” : True, False, </br> ”msg” : “msg”}|
||:white_check_mark:게시글 좋아요 취소|/api/like|POST|{”postId”:게시글 번호, </br> ”userId”:사용자 ID} |{“result” : True, False, </br> ”msg” : “msg”}|


      
      


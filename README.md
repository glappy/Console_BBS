# 오라클 활용 콘솔 게시판 만들기

## 순수 자바를 활용하고 JDBC를 통해서 오라클 DB와 연동하는 콘솔형 게시판 생성

## 1. 목표
글쓰기, 내용보기, 수정, 삭제 기능 구현
댓글쓰기, 답글쓰기는 다음에 구현한다

## JAVA에서 DB 어플리케이션 구현 순서
1. VO생성
table과 같은 구조로 생성하고 member변수 이름도 table칼럼과 일치시킨다.

2. DAO 생성
dao는 db로부터 데이터를 읽고 쓰고 수정하고 삭제할 때 사용할 class
실제적으로 db에 연결하고 crud를 구현하는 부분
class를 생성하기 앞서 interface를 작성하고 interface를 implement해서 클래스를 구현한다

3. Service생성
dao와 사용자 ui 사이에서 데이터를 선가공하는 여러 method를 구현한다

#### (틀렸을 때는 파일 수정하고 git add . → git commit -m "README 파일 수정" → git push)
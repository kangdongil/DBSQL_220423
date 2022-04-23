# DB SQL 개요

## DB
- 행과 열의 관계로 데이터를 저장하는 시스템

## SQL
- 데이터정의어(DDL): Table 관리
- 데이터제어어(DCL): 사용자 관리/보안설정
- 데이터조작어(DML): 데이터 조작
  - Select / Update / Insert / Delete 4가지가 있다(=CRUD)
  - Update / Insert / Delete는 구문형태가 한 가지밖에 없다
  - Insert문을 어떻게 잘 짜는가가 SQL을 다루는데 있어 관건이다

* DDL과 DCL은 DBMS에서 기본적으로 지원한다
* DML는 `DB안 data를 어떻게 다룰 것인가?`에 대한 내용이다
* SQL 데이터 형식은 크게 `'문자'`와 `숫자`가 있다

## INSERT INTO 문: 데이터 추가하기
- `INSERT INTO TABLE(FIELD1, FIELD2, ...) VALUES (VALUE1, VALUE2, ...)`
- `FIELD`와 `VALUE`의 개수가 일치해야 한다

### INSERT문 실습하기: 
```
USE [DB명]

SELECT * FROM [TABLE명]
INSERT INTO [TABLE명]([필드명1], [필드명2], ...) VALUES([값1], [값2], ...)
```

## UPDATE SET 문: 데이터 수정하기
- `UPDATE TABLE SET FIELD1=VALUE1, FIELD2=VALUE2, ...`
- `WHERE`절과 같이 조건 설정이 반드시 필요하다

### UPDATE문 실습하기:
```
 USE [DB명]
 
 SELECT * FROM [TABLE명]
 UPDATE [TABLE명] SET [필드명]=[값] WHERE [필드명]=[값]
```

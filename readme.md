## 1.데이터베이스(DataBase)

### 1) 데이터베이스란?

- 데이터를 저장하는 구조

### 2) 데이터베이스 관리시스템(DBMS)

- 데이터베이스를 단위로 C(insert)R(select)U(update)D(update)
- 별도의 SQL을 문법으로 하여 실행됨

## 2.mySQL 데이터베이스

### 데이터베이스

- 관련성이 있는 데이터를 중복없이 저장하는 구조

### 관계형 데이터베이스(RDBMS) Relationship Database Managaement System

- 테이블 단위로 데이터를 저장
- 관련성 있는 테이블은 참조관계(부pk-자식fk)를 통해 연결
- 서버가 종료된 후에도 별도의 시스템에서 유지
- 여러 사람이 한꺼번에 접속하여 공유하는 형태
- 실시간(realtime) 서비스로 운영

## 3. MySQL, Workbench 설치

- 다운로드 : https://dev.mysql.com/downloads/installer

## SQL(structured Query Language) / ANSI SQL

- -DBMS에 저장된 데이터를 CRUD 작업을 통해 작업을 수행하는 언어
- 1.DDL(Data Definition Language 데이터정의어)
- - 데이터베이스 관리자가 논리적인 저장공간을 정의하는 언어
- create, alter, drop, truncate
- 2.DML(Data Manipulation Language 데이터 조작어)
- - 저장된 논ㄴ리적인 공간에 저장할 데이터를 CRUD를 수행하는 언어
- insert-c select-r update-u delete-d(
- 3.DCL(Data Control Language 데이터 제어어)
- - 데이터베이스에 접근할 수 있는 권한을 제어하는 언어
- grant(권한부여) revoke(권한해지)
- 4.TCL(Transcation Control language 트랜젝션 제어어)
- - 데이터베이스 작업의 단위를 트랜젝션이라 하며, 작업을 데이터베이스에 영구히 적용하는 경우하거나 취소하는 언어
- commit(작업완료), rollback(작업취소),savepoint(작업저장)

### 테이블의 구조 확인 : DESC

- 형식 : DESC : 테이블명

### 단순조회 (R:select)

- 형식 : select 컬럼 from 테이블명

### null 값을 다른 값으로 대체하는 함수 : ifnull()

- 형식 : ifnull(null포함 컬럼명,변경하는값

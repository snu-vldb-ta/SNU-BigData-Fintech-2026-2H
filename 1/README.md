### 1차시 실습

수업에서 배운 SQL 문을 직접 작성하고 실행해 봅니다.
실습 환경인 FreeSQL 사용법을 익히고, 앞으로 계속 사용할 SCOTT 스키마를 만듭니다.

#### 준비물
- Oracle 계정 (테이블을 만들려면 로그인이 필요합니다)
- 웹 브라우저 (별도 설치 없음)

#### 실습 순서 [참고](./getting_started_with_freesql.pdf)
1. [FreeSQL](https://freesql.com)에 접속해 로그인합니다.
2. [scott.md](scott.md)를 따라 SCOTT 스키마를 만듭니다.
3. `SELECT * FROM DEPT;`로 테이블이 만들어졌는지 확인합니다.
4. 아래 실습 자료의 SQL 문을 따라 실행합니다.

#### 실습 자료
교수님께서 수업 시간에 사용하시는 SQL 문은 Oracle 환경을 기준으로 작성되어 있습니다.
FreeSQL에서 그대로 실행할 수 있도록 변환한 파일을 제공합니다.

| 단원 | SQL 문 | 실행 결과 포함 |
|---|---|---|
| 1.1 Introduction to DB | [보기](./1.1%20Introduction%20to%20DB%20(FreeSQL).md) | [보기](./1.1%20Introduction%20to%20DB%20(FreeSQL)_with_results.md) |
| 1.2 Relational Model | [보기](./1.2%20relational%20model%20(FreeSQL).md) | [보기](./1.2%20relational%20model%20(FreeSQL)_with_results.md) |

- 모든 실습 자료는 SCOTT 스키마가 만들어져 있다고 가정합니다. 먼저 scott.md를 실행한 뒤 따라 하세요.


#### 유의사항
- 실습을 시작할 때마다 테이블이 있는지 먼저 확인합니다. 없으면 scott.md를 다시 실행합니다.
- 데이터를 처음 상태로 되돌리려면 테이블을 삭제한 뒤 scott.md를 다시 실행합니다.
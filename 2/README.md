### 2차시 실습

수업에서 배운 관계대수 연산과 SQL 문을 직접 실행해 봅니다.
1차시에 만든 SCOTT 스키마를 그대로 사용합니다.

#### 준비물
- Oracle 계정 (테이블을 만들려면 로그인이 필요합니다)
- 웹 브라우저 (별도 설치 없음)
- 1차시에 만든 SCOTT 스키마

#### 실습 순서
1. [FreeSQL](https://freesql.com)에 접속해 로그인합니다.
2. `SELECT * FROM EMP;`로 테이블이 있는지 확인합니다. 없으면 [scott.md](../1/scott.md)를 다시 실행합니다.
3. 아래 실습 자료의 SQL 문을 따라 실행합니다.

#### 실습 자료
교수님께서 수업 시간에 사용하시는 SQL 문은 Oracle 환경을 기준으로 작성되어 있습니다.
FreeSQL에서 그대로 실행할 수 있도록 변환한 파일을 제공합니다.

| 단원 | SQL 문 | 실행 결과 포함 |
|---|---|---|
| 2.1 Relational Algebra | [보기](./2.1%20relational%20algebra%20(FreeSQL).md) | [보기](./2.1%20relational%20algebra%20(FreeSQL)_with_results.md) |
| 2.2 Basic SQL | [보기](./2.2%20basic%20sql%20(FreeSQL).md) | [보기](./2.2%20basic%20sql%20(FreeSQL)_with_results.md) |
| 3.1 (Advanced SQL) Cube | [보기](./3.1%20(Advanced%20SQL)%20Cube%20(FreeSQL).md) | [보기](./3.1%20(Advanced%20SQL)%20Cube%20(FreeSQL)_with_results.md) |
| 3.3 (Advanced SQL) With Recursive Subquery Factoring in Oracle | [보기](./3.3%20(Advanced%20SQL)%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20(FreeSQL).md) | [보기](./3.3%20(Advanced%20SQL)%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20(FreeSQL)_with_results.md) |

- 모든 실습 자료는 SCOTT 스키마가 만들어져 있다고 가정합니다. 먼저 [scott.md](../1/scott.md)를 실행한 뒤 따라 하세요.


#### 유의사항
- 실습을 시작할 때마다 테이블이 있는지 먼저 확인합니다. 없으면 scott.md를 다시 실행합니다.
- 데이터를 처음 상태로 되돌리려면 테이블을 삭제한 뒤 scott.md를 다시 실행합니다.
- "(에러가 나는 것이 정상입니다)"라고 표시된 문장은 일부러 에러를 내는 예제입니다. 왜 에러가 나는지 생각해 보세요.
- 2.2와 3.3에는 EMP 테이블의 KING 행을 잠시 바꾸는 블록이 있습니다. 주의사항이 붙은 블록은 마지막 문장까지 실행해 원래대로 되돌리세요.
- 실습 중에 만든 테이블(TEST, SALES, PARENT)은 각 자료 끝의 "실습을 마친 뒤"에 있는 문장으로 삭제합니다.
- ORDER BY가 없는 질의는 실행 결과의 행 순서가 "실행 결과 포함" 파일과 다를 수 있습니다.
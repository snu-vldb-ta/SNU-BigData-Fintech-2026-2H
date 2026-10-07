# 2차시 실습

## SQL

Oracle FreeSQL에서 [SCOTT 스키마](../1/scott.md)를 사용한다.

| 단원 | SQL 문 | 실행 결과 포함 |
|---|---|---|
| 2.1 Relational Algebra | [보기](./2.1%20relational%20algebra%20%28FreeSQL%29.md) | [보기](./2.1%20relational%20algebra%20%28FreeSQL%29_with_results.md) |
| 2.2 Basic SQL | [보기](./2.2%20basic%20sql%20%28FreeSQL%29.md) | [보기](./2.2%20basic%20sql%20%28FreeSQL%29_with_results.md) |
| 3.1 ROLLUP과 CUBE | [보기](./3.1%20%28Advanced%20SQL%29%20Cube%20%28FreeSQL%29.md) | [보기](./3.1%20%28Advanced%20SQL%29%20Cube%20%28FreeSQL%29_with_results.md) |
| 3.3 재귀 서브쿼리 | [보기](./3.3%20%28Advanced%20SQL%29%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20%28FreeSQL%29.md) | [보기](./3.3%20%28Advanced%20SQL%29%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20%28FreeSQL%29_with_results.md) |

- 데이터 변경 예제는 복원 문장까지 실행
- `ORDER BY`가 없는 질의는 결과의 행 순서가 다를 수 있음

## NL2SQL·RAG

| 실습 | 자료 | 데이터 | DB |
|---|---|---|---|
| NL2SQL | [강의자료](./nl2sql.pdf) · [노트북](./NL2SQL.ipynb) | SCOTT의 EMP·DEPT 테이블 | DuckDB (관계형 DB) |
| RAG | [노트북](./RAG.ipynb) | GSDS 이수규정·입시 FAQ 요약 문서 6개 | Chroma DB (벡터 DB) |

[전체 실습 자료](../README.md)

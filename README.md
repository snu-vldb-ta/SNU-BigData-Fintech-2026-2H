# SNU BigData Fintech 2026-2H

- **Instructor**: Prof. Sang-Won Lee
- **TA**: Kyong-Shik Lee (kyongshikl@snu.ac.kr)

데이터베이스·SQL 수업의 실습 자료와 NL2SQL·RAG 노트북을 제공한다.

## 1차시 · 2026.09.30

[1차시 실습 안내](./1/README.md)

- [FreeSQL 사용법](./1/getting_started_with_freesql.pdf)
- [SCOTT 스키마 및 데이터](./1/scott.md)

| 단원 | SQL 문 | 실행 결과 포함 |
|---|---|---|
| 1.1 Introduction to DB | [보기](./1/1.1%20Introduction%20to%20DB%20%28FreeSQL%29.md) | [보기](./1/1.1%20Introduction%20to%20DB%20%28FreeSQL%29_with_results.md) |
| 1.2 Relational Model | [보기](./1/1.2%20relational%20model%20%28FreeSQL%29.md) | [보기](./1/1.2%20relational%20model%20%28FreeSQL%29_with_results.md) |

## 2차시 · 2026.10.07

[2차시 실습 안내](./2/README.md)

### SQL 실습 자료

관계대수, 기본 SQL, 고급 SQL의 질의와 실행 결과를 비교한다.

| 단원 | SQL 문 | 실행 결과 포함 |
|---|---|---|
| 2.1 Relational Algebra | [보기](./2/2.1%20relational%20algebra%20%28FreeSQL%29.md) | [보기](./2/2.1%20relational%20algebra%20%28FreeSQL%29_with_results.md) |
| 2.2 Basic SQL | [보기](./2/2.2%20basic%20sql%20%28FreeSQL%29.md) | [보기](./2/2.2%20basic%20sql%20%28FreeSQL%29_with_results.md) |
| 3.1 ROLLUP과 CUBE | [보기](./2/3.1%20%28Advanced%20SQL%29%20Cube%20%28FreeSQL%29.md) | [보기](./2/3.1%20%28Advanced%20SQL%29%20Cube%20%28FreeSQL%29_with_results.md) |
| 3.3 재귀 서브쿼리 | [보기](./2/3.3%20%28Advanced%20SQL%29%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20%28FreeSQL%29.md) | [보기](./2/3.3%20%28Advanced%20SQL%29%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20%28FreeSQL%29_with_results.md) |

### NL2SQL·RAG 실습

| 자료 | 내용 |
|---|---|
| [NL2SQL 강의자료](./2/nl2sql.pdf) | 자연어 질의, 스키마 연결, 생성 SQL과 결과 검증 |
| [NL2SQL 실습 노트북](./2/NL2SQL.ipynb) | DuckDB의 SCOTT 데이터로 자연어 질문과 생성 SQL·기준 결과 비교 |
| [RAG 실습 노트북](./2/RAG.ipynb) | GSDS FAQ를 Chroma DB에서 검색하고, 근거를 바탕으로 답변 생성·평가 |

- FreeSQL 자료: Oracle 환경의 SQL 실습
- NL2SQL·RAG 노트북: Python 환경과 OpenAI API 키 사용
- `_with_results.md`: SQL 문과 실행 결과를 함께 수록한 자료

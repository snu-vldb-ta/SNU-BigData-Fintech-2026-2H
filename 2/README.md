# 2차시 실습

관계대수와 SQL 질의를 확인하고, 자연어 질문으로 데이터를 조회하는 NL2SQL과 문서에서 근거를 찾아 답하는 RAG를 실습한다.

## 자료 구성

| 구분 | 자료 | 내용 |
|---|---|---|
| SQL | 아래 단원별 Markdown 자료 | 관계대수, 기본 SQL, ROLLUP·CUBE, 재귀 서브쿼리 |
| NL2SQL | [강의자료](./nl2sql.pdf) · [실습 노트북](./NL2SQL.ipynb) | 자연어 질문을 SQL로 변환하고 실행 결과 비교 |
| RAG | [실습 노트북](./RAG.ipynb) | FAQ 검색, 근거 기반 답변 생성, 검색·답변 평가 |

## 1. SQL 실습

- 환경: Oracle FreeSQL
- 데이터: 1차시의 [SCOTT 스키마](../1/scott.md)
- SQL 문과 실행 결과를 나란히 비교

| 단원 | SQL 문 | 실행 결과 포함 |
|---|---|---|
| 2.1 Relational Algebra | [보기](./2.1%20relational%20algebra%20%28FreeSQL%29.md) | [보기](./2.1%20relational%20algebra%20%28FreeSQL%29_with_results.md) |
| 2.2 Basic SQL | [보기](./2.2%20basic%20sql%20%28FreeSQL%29.md) | [보기](./2.2%20basic%20sql%20%28FreeSQL%29_with_results.md) |
| 3.1 ROLLUP과 CUBE | [보기](./3.1%20%28Advanced%20SQL%29%20Cube%20%28FreeSQL%29.md) | [보기](./3.1%20%28Advanced%20SQL%29%20Cube%20%28FreeSQL%29_with_results.md) |
| 3.3 재귀 서브쿼리 | [보기](./3.3%20%28Advanced%20SQL%29%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20%28FreeSQL%29.md) | [보기](./3.3%20%28Advanced%20SQL%29%20With%20Recursive%20Subquery%20Factoring%20in%20Oracle%20%28FreeSQL%29_with_results.md) |

### 결과 확인 시 참고

- 오류가 정상이라고 표시된 질의는 오류 원인을 살펴보는 예제
- 2.2와 3.3에서 KING 행을 변경하는 블록은 복원 문장까지 포함
- TEST·SALES·PARENT 등 실습용 테이블의 정리 문장은 각 자료 끝에 수록
- `ORDER BY`가 없는 질의는 결과 행의 순서가 다를 수 있음

## 2. NL2SQL 실습

[강의자료](./nl2sql.pdf) · [NL2SQL.ipynb](./NL2SQL.ipynb)

- DuckDB: Python 프로그램 안에서 동작하는 관계형 DB
- 노트북에서 EMP·DEPT 데이터를 메모리에 구성
- LLM은 스키마와 질문을 바탕으로 SQL을 생성하고, DuckDB가 실행
- 생성 SQL과 기준 SQL의 결과를 비교하고 질문·힌트를 구체화

| 구분 | 실습 내용 |
|---|---|
| Practice I | 기본 질의, 스키마 연결, Join, Subquery, 중복 행 |
| Practice II | GROUP BY·HAVING, NULL, ROLLUP·CUBE, 분석 함수 |
| 추가 실습 | 직원·상사·부서 연결, 모호한 질문, NOT IN·NOT EXISTS, 분석 함수 응용, 업무 용어, 재귀 CTE |

- 실행 성공 여부와 질문에 맞는 결과인지를 구분
- 결과가 같아도 사용한 SQL 문법과 구조는 다를 수 있음
- 결과 불일치는 질문의 모호함, 생성 오류, 출력 형태 차이 등을 살펴보는 비교 지점

## 3. RAG 실습

[RAG.ipynb](./RAG.ipynb)

- 자료: GSDS 이수규정·입시 FAQ를 요약한 카드 6개
- Chroma DB: 문서·임베딩·출처를 저장하고 관련 자료를 찾는 벡터 DB
- 검색한 근거를 LLM에 전달해 답변과 근거 번호 생성

| 단계 | 실습 내용 |
|---|---|
| 자료 준비 | FAQ 확인, 청크 크기별 분할 비교, 임베딩 생성·저장 |
| 검색 | 검색 개수와 질문 표현에 따른 근거 비교 |
| 답변 생성 | 검색 개수·근거의 적절성에 따른 답변 비교 |
| 평가 | RAG 사용 여부 비교, 필요한 근거와 답변·인용 점검 |

- 유사도가 높은 자료라도 질문의 학번·과정과 다를 수 있음
- 검색 결과에 자료가 있어도 답변에 필요한 근거가 없을 수 있음
- 청킹 예제는 분할 방식 비교용이며, 이후 검색에는 카드 6개를 사용

## 실습 환경

| 자료 | 환경·준비 사항 |
|---|---|
| FreeSQL 자료 | Oracle 계정, 웹 브라우저, SCOTT 스키마 |
| NL2SQL 노트북 | Colab 또는 Jupyter, OpenAI API 키, DuckDB |
| RAG 노트북 | Colab 또는 Jupyter, OpenAI API 키, Chroma DB |

노트북의 데이터는 각 노트북에서 준비하며, FreeSQL의 테이블과 연결하지 않는다.

[전체 실습 자료로 돌아가기](../README.md)

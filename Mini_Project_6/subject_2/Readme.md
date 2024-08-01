# LLM을 활용한 QA 챗봇 구현

## Project Abstract

- 주제: LLM을 활용한 QA 챗봇 구현
- 사전학습과목: 언어 지능
- 데이터 출처: 네이버 감정분류 데이터 및 한국어 위키
- 데이터 구분: Text
- 문제 유형: Retrieval Augmented Generation(RAG)
- 중점사항:
    - LLM fine-tuning
    - 문서 검색
    - 검색 기반 QA 챗봇

## 데이터 소개(NSMC)

- https://github.com/e9t/nsmc

## 수행 절차 및 조건(SLLM SFT)

- Hugging Face
    - Access Token 발행
        - 일부 라이센스가 있는 모델을 사용하거나 API 레벨의 권한이 필요할 때 사용
    - Transformers
        - 공개된 유명 아키텍처 코드 지원(ex. Llama, Gemma 등)
        - 소스코드와 함께 학습된 모델 파라미터 다운로드 및 활용 가능
        - 다양한 외부 유명 라이브러리와 쉽게 연동 가능

## RAG(Retrieval-Augmented Generation)

- 문서 DB 구축
    - chunk_db.json 생성

- 문서 검색
    - BM25 문서 검색
    - Sentence Transformer 문서 검색

- RAG 시스템 구축

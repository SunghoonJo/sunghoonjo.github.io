# Sunghoon Jo  
**Search Backend / AI Search Engineer**

대규모 상용 서비스 환경에서 검색 시스템을 설계·운영하며,  
**사용자 경험의 변화를 기술로 선제적으로 반영하는 검색 엔지니어**입니다.

---

## About Me

저는 삼성전자에서 3년간 TV내 미들웨어 개발을 진행하며 디바이스 개발에 대한 경험을 쌓았고 약 9년간 Smart TV 환경에서 콘텐츠 검색 서비스 서버 개발과 검색 품질 고도화를 담당해 왔습니다.

검색 시스템을 단순한 기능이 아닌 **사용자 경험을 결정하는 핵심 인터페이스**로 바라보며, 기술 도입 자체보다 “왜 필요한가, 실제 서비스에 어떻게 안착시킬 것인가”를 중요하게 생각합니다.

최근에는 LLM과 Vector 기반 검색 기술을 실험적 적용에 그치지 않고, **법무·운영·성능 제약을 고려한 상용 검색 구조로 설계·확장**하는 데 집중하고 있습니다.

---

## Core Skills

### Search / Data
- Elasticsearch, Solr, Lucene
- OpenSearch 구조 이해 및 인덱스 설계
- 대규모 데이터 파이프라인 / 인덱싱 최적화

### AI / ML
- Semantic Search, Vector Embedding
- LLM 기반 메타데이터 증강
- NER / Classification
- RAG 기반 검색·추천 구조

### Infra / Operation
- Docker, Kubernetes
- Batch Processing Pipeline
- 대규모 트래픽 환경의 검색 안정화
- 검색 KPI 기반 품질 모니터링

---

## Career

### Samsung Electronics  
**Tizen middleware Engineer**
2013 - 2015
- Smart TV내 외부 파트너사의 콘텐츠 추천 제공을 위한 플랫폼 설계 및 개발
- 
**Search Backend Engineer**  
2016 – Present

- Smart TV 콘텐츠 검색 서비스 서버 개발
- 글로벌 TV 플랫폼 검색 인프라 설계·운영
- 음성/텍스트 검색 품질 개선 및 AI 검색 도입

---

## Featured Projects  
## Smart TV Search Evolution  
**Keyword Search → Semantic Search → LLM-based Search (2016–2024)**

Smart TV 검색 서비스는 사용자 입력 방식과 기대 수준의 변화에 따라 **단계적으로 진화해 온 검색 시스템**입니다.  
저는 이 검색 서비스의 초기 구조 설계부터 AI 기반 고도화까지 전 과정을 경험했습니다.

---

## 1. 검색 서비스 초기 구축 및 인프라 설계 (2016–2018)

### Background
Smart TV 플랫폼에서 다양한 콘텐츠를 안정적으로 검색·제공하기 위해 확장 가능하고 운영 가능한 검색 인프라가 필요했습니다.

### Work
- Lucene 기반 Solr Indexer 구성
- 콘텐츠 메타데이터 수집·정제·인덱싱 파이프라인 설계
- 파트너 데이터 유입을 고려한 검색 스키마 설계
- 대규모 콘텐츠 업데이트 환경에서의 인덱싱 안정성 확보

### Contribution
- 검색 인덱스 구조 및 필드 설계 주도
- 초기 검색 파이프라인 아키텍처 정의
- 운영 환경 인덱싱 이슈 대응

---

## 2. 검색 품질 개선 및 추천 고도화 (2019–2021)

### Background
콘텐츠 수 증가로 인해 단순 키워드 매칭만으로는 사용자가 기대하는 검색 품질을 유지하기 어려운 단계에 도달했습니다.

### Work
- Elasticsearch 기반 검색 인덱스 전환 및 최적화
- 검색 KPI 기반 품질 분석 체계 구축
- TF-IDF를 응용한 Trending 콘텐츠 추천 로직 설계
- Tokenizing, Stemmer 등 검색 솔루션 도입

### Result
- 인기 콘텐츠 노출 정확도 향상
- 검색 결과 일관성 개선
- 검색 품질 지표 안정화

---

## 3. 음성 검색 및 NER 기반 질의 이해 고도화 (2021–2023)

### Background
Bixby 음성 검색 도입으로 사용자 발화에서 의미 단위(Entity)를 정확히 분리하는 것이 핵심 과제가 되었습니다.

### Work
- ML 기반 classification을 활용한 NER 구조 설계
- 제목, 장르, 배우 등 엔티티 단위 분류
- 음성 발화 특성을 고려한 질의 전처리 개선

### Result
- 음성 검색 오탐 감소
- 엔티티 기반 검색 정확도 향상

---

## 4. LLM 기반 메타데이터 증강 및 Semantic Search 고도화 (2024)

### Background
기존에는 단문 발화가 주를 이루었지만, 사용자는 점차 자연어에 가까운 표현으로 검색 의도를 전달하기 시작했습니다.

기존 키워드·엔티티 중심 검색만으로는 이러한 변화에 대응하기 어렵다고 판단했습니다.

---

### Challenge
- 콘텐츠 메타데이터의 의미 정보 한계
- 메타데이터 제공 업체의 AI 활용 거부
- 법무 이슈 없이 의미 확장이 가능한 구조 필요

---

### Approach
- LLM을 활용한 콘텐츠 메타데이터 의미 증강
- 외부 오픈데이터 기반 간접 매칭 구조 설계로 법무 리스크 회피
- Batch 기반 프로세서로 증강 파이프라인 구성
- Vector embedding 기반 semantic search 구축
- 키워드 검색과 의미 검색 병렬 처리 후 re-rank 적용

---

### Result
- 확장·비정형 발화에서 검색 실패 비율 감소
- 검색 KPI 기준 의미 있는 품질 개선
- 대규모 상용 TV 서비스 환경에서 안정적 운영
- 검색 품질 고도화 기술로 특허 출원

---

### Contribution
- 프로젝트 문제 정의 및 기술 방향 설정
- 데이터 전략 및 법무 이슈 회피 구조 설계
- Batch 기반 메타데이터 증강 파이프라인 구현
- Semantic search 및 re-rank 구조 설계 주도

---

## Summary

본 프로젝트들은 서로 독립적인 시도가 아니라,  
검색 시스템이 사용자 경험 변화에 맞춰 진화해 온 연속적인 과정입니다.

저는 키워드 검색 인프라 구축부터 AI·LLM 기반 검색 고도화까지 검색 서비스의 전체 생애주기를 직접 설계·운영해 왔습니다.

---

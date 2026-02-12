# [PORTFOLIO] 검색 & AI 서비스 아키텍트

> **"10년의 데이터 검색 엔지니어링 경험을 바탕으로, 검색의 본질과 AI의 미래를 연결합니다."**

## 📂 업무 이력 요약

### 1. 콘텐츠 통합 및 데이터 수집 데몬 개발 (2013 ~ 2015)

**[Smart TV First Screen 지원용 백엔드 구축]**

- **역할:** 파트너사(CP) 데이터 수집/저장 데몬 프로세서 설계 및 개발
    
- **주요 성과:**
    
    - Smart TV 홈 화면(First Screen)에 노출될 추천 콘텐츠를 위해 다수의 외부 CP(Content Provider)와 TV 시스템 간의 주기적 데이터 동기화 구현.

    - 외부 파트너사 제공용 **Web API Spec 설계** 및 표준화 주도.
        
    - 대량의 콘텐츠 메타데이터를 안정적으로 수집하고 저장하기 위한 주기적 배치/데몬 로직 최적화.
    

---

### 2. Smart TV 통합 검색 서비스 서버 개발 (2016 ~ 현재)

**[검색 엔진 고도화 및 Cloud 인프라 운영]** Smart TV의 핵심 기능인 통합 검색 서비스의 백엔드 아키텍처를 설계하고 지속적으로 고도화해 오고 있습니다.

#### ① 검색 엔진 인프라 및 데이터 파이프라인 (Data & Infra)

- **AWS EKS 기반 MSA 전환:** Java 기반의 Monolitic 레거시 서버를 EKS 기반의 MSA로 전환하여 서비스 가용성과 배포 유연성 확보.
    
- **엔진 고도화:** Solr에서 Elasticsearch로 검색 엔진 전환 및 인덱스 설계 주도.
    
- **PostgreSQL 기반 데이터 파이프라인:**
    
    - PostgreSQL에서 데이터 1차 정제 및 무결성 검증.
        
    - **Batch Processor를 통한 비정규화(Denormalization):** 검색 성능 극대화를 위해 분산된 데이터를 단일 문서 모델로 변환하여 ES 인덱싱 수행.
        
- **성과:** 대규모 트래픽 하에서도 검색 응답 속도 최적화 및 데이터 정합성 유지.
    

#### ② 검색 품질 고도화 (Search Quality)

- **Progressive 검색:** Tokenizing, Stemmer 커스터마이징을 통해 한국어/영어 및 EU 주요 언어 검색 품질 개선.
    
- **Trending 추천:** 검색 KPI 데이터를 기반으로 **TF-IDF 알고리즘을 응용**한 실시간 트렌딩 콘텐츠 로직 구현.
    
- **Bixby 음성 검색:** 사용자 발화 의도를 분석하기 위한 **ML 기반 NER(Named Entity Recognition)** 도입 (제목, 장르, 배우 등 개체명 구분).
    

#### ③ AI & LLM 서비스 혁신 (AI Agent & Semantic Search)

- **Semantic Search 설계:** 키워드를 넘어선 의도 파악을 위해 **Vector 기반 의미 검색** 기능 개발.
    
- **Re-rank 알고리즘 (특허 출원):** Vector 검색 결과의 정밀도를 높이기 위해 검색 품질을 재정렬하는 알고리즘을 독자적으로 설계하고 **특허 출원**.
    
- **LLM 활용 메타데이터 증강:** 부족한 콘텐츠 정보를 LLM으로 생성/보충하여 검색 가능 범위(Coverage) 대폭 확대.
    
- **AI Agent 구현:** **RAG(검색 증강 생성)** 기술을 접목하여 단순 결과 나열이 아닌, 사용자의 질문에 직접 해답을 제공하는 콘텐츠 추천 에이전트 구축.
    

---

## 🛠 주요 기술 스택 (Tech Stack)

- **Languages:** Node.js, Python, C#
    
- **Search/AI:** Elasticsearch, Solr, Vector Search, RAG, ML-based NER
    
- **Database:** **PostgreSQL**, Redis, DynamoDB
    
- **Cloud/Infra:** **AWS EKS**, Docker, CI/CD(Jenkins), Batch Processing

---

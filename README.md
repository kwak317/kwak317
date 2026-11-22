# Kwak Hojun — AI Service Developer

근거를 찾고, 검증하고, 측정해서 **실제로 배포되는 LLM 서비스**를 만드는 신입 AI 서비스 개발자 곽호준입니다.

RAG 검색 품질을 숫자로 끌어올리고(Recall@5 0.777 → 0.877, MRR 0.735 → 0.903), LangGraph 멀티에이전트에 사람 승인 단계를 넣고, 개선이 없으면 "차이 없음"이라고 그대로 보고합니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-2563EB?style=flat-square&logo=vercel&logoColor=white)](https://kwak-hojun-ai-portfolio.vercel.app)
[![말해봄](https://img.shields.io/badge/Live-malhaebom.xyz-10B981?style=flat-square)](https://malhaebom.xyz/)
[![Email](https://img.shields.io/badge/Email-hojun6901%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:hojun6901@gmail.com)

> 🔎 **구직 중** · AI 서비스 개발 / LLM·AI 에이전트 엔지니어 / RAG 엔지니어 / Python(FastAPI) AI 백엔드 / LLMOps(평가·관측) 신입·주니어

---

## 🧰 Tech Stack

| Area | Technologies |
| --- | --- |
| LLM & Agent | `LangGraph` `LangChain` `Deep Agents` `FastMCP` `OpenRouter` `OpenAI API` `Prompt Engineering` |
| RAG & Search | `Hybrid Search (BM25 + Dense)` `RRF` `Cohere Rerank` `voyage-4` `KURE-v1` `pgvector` |
| Evaluation & Observability | `Langfuse` `Recall@k / MRR` `LLM-as-a-Judge` `JSON Schema` `Pydantic` |
| Backend | `Python` `FastAPI` `PostgreSQL` `Supabase` `Java` `Spring Boot` |
| Frontend | `React` `TypeScript` `Vite` `Next.js` `Streamlit` |
| DevOps | `Docker` `GCP Cloud Run` `Vercel` `GitHub Actions` `pytest` |
| ML | `PyTorch` `Transformers` `scikit-learn` `librosa` `pandas` |

---

## 📦 Featured Projects

### 1. SecuBridge (시큐브릿지) — 보안 조치 가이드 멀티에이전트 RAG

공공 SI 개발자가 SW 개발보안 기준(행안부 지침·KISA 자료)에 맞춰 Java 취약점 조치안을 찾을 수 있도록, **원문 근거 인용 → 검증 → 사람 승인**을 거치는 LangGraph 멀티에이전트 RAG 서비스입니다.
`3인 팀 프로젝트 · 2026.10–11 · 팀 PR 183건 작성(180건 병합)`

**My Role**: 코퍼스·청킹, 검색(RAG), 평가셋·평가 리포트, CI 게이트, 배포 운영 점검

**Results**

- 문서 754건 → 청크 13,234개 코퍼스 구축
- BM25 + voyage-4 하이브리드(RRF)로 **Recall@5 0.777 → 0.877**
- Cohere 2단계 재정렬로 **MRR 0.735 → 0.903** (Recall@5 0.897 유지)
- 검색 p50 1.486초, 문항당 약 $0.0025
- 단일 vs 멀티에이전트 비교: "품질 차이 없음, 비용 1.6배"로 정직하게 보고
- 간접 프롬프트 인젝션 시험: 단순 RAG 5/5 노출 vs 서비스 0/5
- GitHub Actions에 검색 점수 게이트 + 변이 테스트, 로컬 686개 테스트 통과

```text
User ─▶ React (Vercel) ─▶ FastAPI (Cloud Run)
                             │
                             ▼
                   LangGraph Supervisor
                             │
       근거 검색 ─▶ 조치안 작성 ─▶ 검증 ─▶ 사람 승인 (HITL interrupt)
          │
   BM25 + voyage-4 ─▶ RRF ─▶ Cohere Rerank ─▶ 원문 근거 인용

   PostgreSQL/pgvector (Supabase) · Postgres checkpointer · Langfuse
```

`Python` `FastAPI` `LangGraph` `Deep Agents` `Cohere Rerank` `pgvector` `Supabase` `Langfuse` `Docker` `Cloud Run` `GitHub Actions`

팀 저장소는 비공개입니다 · 구조와 평가 결과는 [포트폴리오](https://kwak-hojun-ai-portfolio.vercel.app)에서 볼 수 있어요

---

### 2. 말해봄 Mk.2 — AI 면접 코칭 에이전트 (팀장)

면접 답변을 녹음하면 **답변 속 근거로 코칭**하는 AI 면접 코칭 서비스입니다. NCS 자가진단, README·이력서 분석, 공고 추천, STT, 재답변 비교, 이력서 초안 생성까지 제공합니다.
`3인 팀 프로젝트 · 팀장`

**Results**

- 출력 계약 준수율 **10% → 100%** (30/30, 3회 반복 90/90) — 모델 교체 + JSON Schema·Pydantic 검증·재시도
- 응답 p95 4.20초
- FastMCP 도구에 인증·접근 제한 적용

`Python` `FastAPI` `RAG` `FastMCP` `React` `Langfuse` `Docker` `Supabase`

[Live Service](https://malhaebom.xyz/) · [Demo](https://kwak-hojun-ai-portfolio.vercel.app/demo/malhaebom)

---

### 3. Mini Projects

| Project | Summary | Links |
| --- | --- | --- |
| 컴퓨터 주변기기 매장 대시보드 | 상품 200개 판매·재고·견적 대시보드 + 검색 도구를 호출하는 에이전트 | [Repo](https://github.com/kwak317/streamline) |
| Music Lens | librosa 57개 특징 + RandomForest로 10개 장르 분류 | [Repo](https://github.com/kwak317/ai_music) |
| 딥러닝 모델 랩 | PyTorch CNN 손글씨 분류 + 서울 따릉이 수요 회귀 | [Repo](https://github.com/kwak317/mini_project) |
| CLIP 패션 검색 · 이미지 캡셔닝 | CLIP ViT-B/16 텍스트·이미지 검색, BLIP 캡셔닝 + NLLB 번역 | [Repo](https://github.com/kwak317/transformer4-assignment) |
| GPT 맞춤형 PC 견적 서비스 | React + Spring Boot 팀 프로젝트. GPT 응답 JSON 파싱, JWT 인증, 네이버·카카오 API 연동 담당 | [FE](https://github.com/5Headers/team_project_frontend) · [BE](https://github.com/5Headers/team_project_backend) |

---

## ⚙️ How I Work

1. **측정 먼저**: 동결된 평가셋과 사전 등록한 지표로 시작하고, 한 번에 하나만 바꿉니다.
2. **근거 있는 출력**: LLM 답변은 원문 인용과 스키마 검증을 거쳐야 화면에 나갑니다.
3. **끝까지 배포**: Docker, Cloud Run, Vercel로 다른 사람이 직접 써볼 수 있게 만듭니다.
4. **테스트로 지키기**: CI 점수 게이트, 회귀·변이 테스트로 품질이 떨어지는 변경을 막습니다.
5. **AI 도구 활용**: Claude Code·Codex로 빠르게 만들고, 테스트로 검증합니다.

---

## 🎓 Education

- **K-디지털 트레이닝 [이스트캠프] AI휴먼 과정 수료** — 멀티모달, TTS, STT, 프롬프트 엔지니어링, RAG
- Java·Spring Boot·React·SQL 웹 개발 과정 학습 ([Java](https://github.com/kwak317/Korea_it_web_java_study) · [Spring Boot](https://github.com/kwak317/Korea_it_web_spring_boot_study) · [Spring Security](https://github.com/kwak317/korea_web_springboot_security) · [React](https://github.com/kwak317/korea_it_web_react_study) · [DBMS](https://github.com/kwak317/korea_it_web_dbms_study))

---

## 📬 Contact

- Portfolio: [kwak-hojun-ai-portfolio.vercel.app](https://kwak-hojun-ai-portfolio.vercel.app)
- Email: [hojun6901@gmail.com](mailto:hojun6901@gmail.com)

채용, 협업, 피드백 제안 모두 환영합니다.

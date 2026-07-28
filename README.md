# Kwak Hojun — AI Service Builder

AI와 웹 개발을 연결해 **실제로 사용할 수 있는 서비스**를 만드는 개발자 곽호준입니다.

사용자의 불편함을 먼저 정의하고, Java/Spring 기반 백엔드부터 React/Next.js 프론트엔드, Python AI 모델과 데이터 시각화까지 제품의 전체 흐름을 구현합니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-2563EB?style=flat-square&logo=vercel&logoColor=white)](https://kwak-hojun-ai-portfolio.vercel.app)
[![GitHub](https://img.shields.io/badge/GitHub-kwak317-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/kwak317)
[![Email](https://img.shields.io/badge/Email-hojun6901%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:hojun6901@gmail.com)

---

## 🚀 What I Build

- **AI-powered Web Services**: GPT와 외부 API를 웹 서비스의 실제 기능으로 연결합니다.
- **Full-Stack Applications**: 사용자 화면부터 인증, 서버 로직, 데이터베이스까지 함께 구현합니다.
- **Interactive AI Demos**: 학습한 머신러닝 모델을 누구나 체험할 수 있는 Streamlit 앱으로 배포합니다.
- **Data-driven Tools**: 데이터를 정리하고 시각화해 사용자의 판단과 반복 업무를 돕습니다.

---

## 🧰 Technical Skills

| Area | Technologies |
| --- | --- |
| Languages | `Java` `Python` `TypeScript` `JavaScript` `SQL` |
| Frontend | `React` `Next.js` `Vite` `Emotion` `Styled Components` |
| Backend | `Spring Boot` `Spring Security` `REST API` `MyBatis` `JWT` `OAuth2` |
| Database & Storage | `MySQL` `Firebase Storage` |
| AI & Data | `OpenAI API` `PyTorch` `Transformers` `scikit-learn` `Pandas` |
| Application & Deploy | `Streamlit` `Vercel` `Git` `GitHub` |

---

## 📦 Featured Projects

### 1. GPT 기반 맞춤형 컴퓨터 견적 서비스

사용자의 목적과 예산을 분석해 PC 부품 조합을 추천하고, 실제 구매 경로까지 연결하는 Team 5Headers의 풀스택 웹 서비스입니다.

#### Key Features

- GPT 응답을 구조화된 JSON으로 변환해 프론트엔드와 데이터베이스에 연동
- 네이버 쇼핑 API를 이용한 부품별 온라인 가격 및 구매 링크 조회
- 카카오맵 API를 이용한 현재 위치 기반 오프라인 매장 검색
- JWT/OAuth2 기반 인증, 북마크, 견적 기록, 계정 관리 기능
- Firebase Storage를 이용한 프로필 이미지 업로드

#### My Contributions

- GPT 기반 견적 생성과 응답 JSON 파싱 로직 구현 및 개선
- GPT 응답 중복 저장 문제와 프론트·백엔드 데이터 구조 불일치 해결
- 회원가입, 로그인, 중복 확인, 사용자 정보, 북마크 API 구현
- 카카오맵·네이버 쇼핑 등 외부 API 연동과 오류 디버깅
- 오프라인 매장 및 북마크 UI와 백엔드 DB 연동

#### Tech Stack

`React` `Spring Boot` `Spring Security` `MySQL` `MyBatis` `OpenAI API` `Firebase`

[Frontend Repository](https://github.com/5Headers/team_project_frontend) · [Backend Repository](https://github.com/5Headers/team_project_backend)

---

### 2. Streamlit AI/ML Showcase

여러 머신러닝 모델과 tool-calling 에이전트를 하나의 인터랙티브 웹 애플리케이션으로 구성한 프로젝트입니다.

#### Key Features

- RandomForest 기반 펭귄 분류 및 feature importance 시각화
- MobileNetV2 기반 이미지 분류와 top-5 결과 제공
- KoELECTRA 기반 한국어 긍정·부정 감성 분석
- 3개 모델을 도구로 호출하는 AI 에이전트와 tool trace 제공
- API 키 없이 기능을 확인할 수 있는 데모 모드
- Streamlit 상태 관리, 캐싱, 챗 UI 및 대시보드 활용

#### Tech Stack

`Python` `Streamlit` `PyTorch` `Transformers` `scikit-learn` `OpenAI API`

[Repository](https://github.com/kwak317/streamline) · [Live Demo](https://streamline-fewhcwgoquxqmznnyr9yx8.streamlit.app)

---

### 3. Deep Learning Model Showcase

MNIST 이미지 분류와 서울 자전거 수요 예측 모델을 직접 체험할 수 있도록 만든 Streamlit 애플리케이션입니다.

#### Key Features

- 업로드한 숫자 이미지를 CNN으로 분류하고 클래스별 신뢰도 표시
- 시간과 날씨 조건을 입력받아 시간당 자전거 대여량 예측
- 시간대별 수요 곡선과 조건별 민감도 시각화
- 모델 학습 노트북부터 웹 앱 패키징과 배포까지 구현

#### Tech Stack

`Python` `PyTorch` `Pandas` `Altair` `Streamlit`

[Repository](https://github.com/kwak317/mini_project) · [Live Demo](https://miniprojectgit-324deds6vhyhjkm7nbrqpe.streamlit.app/회귀_자전거)

---

### 4. AI Service Builder Portfolio

프로젝트, 기술 스택, 개발 관점을 한눈에 전달하기 위해 제작한 개인 포트폴리오 웹사이트입니다.

#### Key Features

- 프로젝트와 성장 방향을 반응형 싱글 페이지로 구성
- 모달 기반 소개, 프로젝트, 연락처 인터랙션
- 실제 서비스와 저장소로 연결되는 프로젝트 링크 제공
- Vercel 기반 배포

#### Tech Stack

`Next.js` `React` `TypeScript` `Vercel`

[Repository](https://github.com/kwak317/portfolio) · [Live Site](https://kwak-hojun-ai-portfolio.vercel.app)

---

## 🧠 Architecture Overview

대표 팀 프로젝트는 다음과 같은 흐름으로 동작합니다.

```text
┌──────────────┐
│     User     │
└──────┬───────┘
       │
       ▼
┌──────────────────────┐
│ React Frontend       │
│ UI · State · API     │
└──────────┬───────────┘
           │ REST API
           ▼
┌──────────────────────┐
│ Spring Boot Backend  │
│ Auth · Business Logic│
└──────┬───────┬───────┘
       │       │
       ▼       ▼
┌──────────┐  ┌─────────────────────────┐
│ MySQL DB │  │ External Services       │
│ Users    │  │ OpenAI · Naver · Kakao │
│ Estimates│  │ Firebase                │
└──────────┘  └─────────────────────────┘
```

---

## ⚙️ Development Workflow

1. **Problem Definition**: 사용자가 겪는 불편함과 반복 과정을 먼저 찾습니다.
2. **Service Design**: 필요한 화면, 데이터, API 흐름을 작은 단위로 나눕니다.
3. **Prototype**: 핵심 기능부터 빠르게 구현해 실제 동작을 확인합니다.
4. **Integration**: 프론트엔드, 백엔드, 데이터베이스와 외부 서비스를 연결합니다.
5. **Debugging**: 데이터 형식, 인증 흐름, 중복 요청 등 경계 영역의 문제를 해결합니다.
6. **Deployment**: 다른 사용자가 직접 확인할 수 있는 형태로 배포합니다.

---

## 📚 Learning Journey

| Repository | Focus |
| --- | --- |
| [korea_it_web_react_study](https://github.com/kwak317/korea_it_web_react_study) | JSX, Props, State, React 컴포넌트 |
| [korea_web_springboot_security](https://github.com/kwak317/korea_web_springboot_security) | Spring Security, JWT, MyBatis |
| [Korea_it_web_spring_boot_study](https://github.com/kwak317/Korea_it_web_spring_boot_study) | Spring Boot 웹 개발 |
| [korea_it_web_dbms_study](https://github.com/kwak317/korea_it_web_dbms_study) | 관계형 데이터베이스와 SQL |
| [Korea_it_web_java_study](https://github.com/kwak317/Korea_it_web_java_study) | Java와 객체지향 프로그래밍 |
| [korea_it_web_html_css_js](https://github.com/kwak317/korea_it_web_html_css_js) | HTML, CSS, JavaScript 기초 |

---

## 📊 GitHub Activity

<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=kwak317&show_icons=true&hide_border=true&theme=transparent)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=kwak317&layout=compact&hide_border=true&theme=transparent)

</div>

---

## 📬 Contact

- Portfolio: [kwak-hojun-ai-portfolio.vercel.app](https://kwak-hojun-ai-portfolio.vercel.app)
- GitHub: [github.com/kwak317](https://github.com/kwak317)
- Email: [hojun6901@gmail.com](mailto:hojun6901@gmail.com)

프로젝트, 협업, 피드백에 관한 이야기를 언제든 환영합니다.

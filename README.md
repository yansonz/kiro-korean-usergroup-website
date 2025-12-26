# Kiro 한국 유저그룹 웹사이트

Kiro에 관심 있는 한국 개발자들을 위한 공식 커뮤니티 원페이지 웹사이트입니다.

## 🎯 프로젝트 개요

이 웹사이트는 AI 기반 코딩 도구 Kiro를 사용하는 한국 개발자들에게 매력적이고 유익한 경험을 제공합니다. 메인 Kiro 웹사이트(https://kiro.dev/)와 유사한 디자인과 UX를 특징으로 하며, 눈에 띄는 애니메이션 유령 마스코트와 쉽게 이해할 수 있는 정보 레이아웃을 제공합니다.

## ✨ 주요 기능

- **🎨 시각적 디자인**: Kiro 브랜드와 일치하는 다크 테마 및 보라색/파란색 그라데이션
- **👻 애니메이션 마스코트**: 인터랙티브한 유령 마스코트 애니메이션
- **📱 반응형 디자인**: 모바일, 태블릿, 데스크톱 모든 기기에서 완벽하게 작동
- **🇰🇷 한국어 콘텐츠**: 모든 콘텐츠가 한국어로 제공
- **⚡ 고성능**: 빠른 로딩 속도와 부드러운 애니메이션
- **🎭 인터랙티브 요소**: 스크롤 애니메이션, 호버 효과, 패럴랙스 효과

## 🚀 시작하기

### 로컬에서 실행

1. 저장소를 클론하거나 파일을 다운로드합니다.

2. `index.html` 파일을 브라우저에서 엽니다:
   ```bash
   open index.html
   ```

   또는 로컬 서버를 실행합니다:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Python 2
   python -m SimpleHTTPServer 8000
   ```

3. 브라우저에서 `http://localhost:8000`을 엽니다.

## 📁 프로젝트 구조

```
kiro-korean-usergroup-website/
├── index.html                    # 메인 HTML 파일
├── styles.css                    # 스타일시트 (CSS 변수, 반응형 디자인)
├── script.js                     # JavaScript 인터랙션 (이벤트 처리, 애니메이션)
├── events.json                   # 이벤트 데이터 (JSON)
├── kiro.png                      # 유령 마스코트 이미지
├── README.md                     # 프로젝트 문서
├── requirement.md                # 요구사항 문서
└── .kiro/specs/
    └── kiro-korean-usergroup-website/
        ├── requirements.md       # 상세 요구사항 문서
        ├── design.md             # 디자인 문서
        └── tasks.md              # 구현 작업 목록
```

## 🎨 디자인 시스템

### 색상 팔레트

- **배경색**:
  - Primary: `#0a0a0f`
  - Secondary: `#12121a`
  - Tertiary: `#1a1a26`

- **텍스트색**:
  - Primary: `#e8e8f0`
  - Secondary: `#a0a0b8`
  - Muted: `#6b6b85`

- **브랜드 컬러**:
  - Primary Purple: `#7c3aed`
  - Secondary Blue: `#3b82f6`
  - Accent Pink: `#ec4899`

### 타이포그래피

- **영문**: Inter (Google Fonts)
- **한글**: Noto Sans KR (Google Fonts)

## 📋 섹션 구성

1. **네비게이션 바**: 로고, 네비게이션 링크, 모바일 메뉴 버튼
2. **히어로 섹션**: 
   - 메인 헤드라인 ("나의 개발 짝꿍 Kiro와 함께")
   - 설명 텍스트
   - CTA 버튼 (커뮤니티 가입, Kiro 알아보기)
   - 애니메이션 유령 마스코트
   - 스크롤 인디케이터
3. **About 섹션**: 
   - 섹션 제목 ("Kiro 한국 유저그룹이란?")
   - 3개의 카드 (함께 배우기, 지식 공유, 네트워킹)
4. **Features 섹션**: 
   - 섹션 제목 ("Kiro가 특별한 이유")
   - 6개의 기능 카드 (스펙 기반 개발, 자율 에이전트, 에이전트 훅, MCP 통합, 성능 최적화, 커스터마이징)
5. **Events 섹션**: 
   - 섹션 제목 ("예정된 이벤트")
   - 이벤트 카드 목록 (events.json에서 동적 로드)
   - 지난 이벤트 1개 + 예정된 이벤트 최대 2개 표시
6. **Join 섹션**: 
   - 섹션 제목 ("3단계로 시작하기")
   - 3단계 가입 프로세스 (시각적 단계 표시)
   - CTA 버튼 (Discord 커뮤니티 가입, 이벤트 정보 확인)
7. **푸터**: 
   - 로고 및 설명
   - 바로가기 링크
   - 저작권 정보

## 🛠️ 기술 스택

- **HTML5**: 시맨틱 마크업, 접근성 (ARIA 레이블)
- **CSS3**: 
  - CSS Variables (커스텀 속성) - 디자인 시스템 구현
  - Flexbox & Grid 레이아웃
  - CSS 애니메이션 & 트랜지션
  - 반응형 미디어 쿼리
  - GPU 가속 (will-change, transform)
  - 모션 감소 설정 지원 (prefers-reduced-motion)
- **JavaScript (Vanilla)**:
  - Intersection Observer API - 스크롤 애니메이션
  - Fetch API - 이벤트 데이터 로드
  - 스로틀링/디바운싱 - 성능 최적화
  - 이벤트 위임 - 메모리 효율성
  - 인터랙티브 효과 (마우스 추적, 호버 상태)
  - 모바일 메뉴 토글
- **폰트**: Google Fonts (Inter, Noto Sans KR)

## 📱 반응형 브레이크포인트

- **데스크톱**: > 968px
- **태블릿**: 640px - 968px
- **모바일**: < 640px

## ⚡ 성능 최적화

- 최적화된 이미지 로딩
- CSS 애니메이션 하드웨어 가속
- 효율적인 JavaScript 이벤트 리스너
- 부드러운 스크롤 및 인터랙션

## 🎯 요구사항 충족

이 웹사이트는 `.kiro/specs/kiro-korean-usergroup-website/requirements.md`에 명시된 모든 요구사항을 충족합니다:

✅ **요구사항 1**: 시각적 디자인 및 브랜딩 (디자인 시스템 색상, 타이포그래피, 간격)  
✅ **요구사항 2**: 유령 마스코트 애니메이션 (페이드인, 플로팅, 성능 최적화)  
✅ **요구사항 3**: 원페이지 정보 레이아웃 (논리적 섹션 구성, 정보 흐름)  
✅ **요구사항 4**: 한국어 콘텐츠 (lang="ko", Noto Sans KR, 기술 용어 병행 표기)  
✅ **요구사항 5**: 유저그룹 정보 표시 (About, Features, Events, Join 섹션)  
✅ **요구사항 6**: 반응형 디자인 (640px, 768px, 968px, 1200px 브레이크포인트)  
✅ **요구사항 7**: 성능 및 로딩 (3초 이내 로드, 60fps 애니메이션)  
✅ **요구사항 8**: 접근성 (색상 대비, 포커스 상태, 모션 감소, 의미론적 HTML)

## 🤝 커뮤니티 참여

- **공식 웹사이트**: https://kiro.dev/
- **이벤트 정보**: https://event-us.kr/awskrug/event
- **Discord**: [커뮤니티 가입하기](#) (TBD)

## 📄 라이선스

이 프로젝트는 비공식 커뮤니티 프로젝트입니다. Kiro는 Amazon의 상표입니다.

## 🔧 개발 가이드

### 이벤트 데이터 추가

`events.json` 파일에 이벤트를 추가합니다:

```json
{
  "id": "event-2026-001",
  "date": "2026-01-29",
  "title": "이벤트 제목",
  "description": "이벤트 설명",
  "location": "이벤트 장소",
  "link": "이벤트 링크"
}
```

### 커스터마이징

CSS 변수를 수정하여 색상, 타이포그래피, 간격을 변경할 수 있습니다:

```css
:root {
  --color-primary: #7c3aed;      /* 주요 브랜드 색상 */
  --color-text: #e8e8f0;         /* 주요 텍스트 색상 */
  --space-5xl: 120px;            /* 섹션 패딩 */
}
```

## 📊 성능 최적화

- **CSS 애니메이션**: GPU 가속 활성화 (will-change, transform)
- **JavaScript**: 스로틀링/디바운싱으로 이벤트 최적화
- **이미지**: 지연 로딩, 에러 처리
- **폰트**: Google Fonts display=swap으로 폰트 로딩 최적화

## 🙏 크레딧

- **Kiro 공식 웹사이트**: https://kiro.dev/
- **디자인 영감**: Kiro 메인 사이트
- **폰트**: Google Fonts (Inter, Noto Sans KR)

---

**Made with ❤️ by Kiro 한국 유저그룹**

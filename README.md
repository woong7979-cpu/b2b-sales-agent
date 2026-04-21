# B2B 세일즈 멀티에이전트 v2

Claude AI 기반 B2B 세일즈 6단계 파이프라인 전략 생성 앱

## 배포 방법 (GitHub + Vercel)

### 1단계 — GitHub에 올리기
1. github.com 에서 새 Repository 생성 (예: b2b-sales-agent)
2. 이 폴더 안의 파일들을 모두 업로드
   - api/chat.js
   - public/index.html
   - vercel.json
   - README.md

### 2단계 — Vercel 배포
1. vercel.com 에서 GitHub 계정으로 로그인
2. "Add New Project" → 위 Repository 선택
3. Environment Variables 추가:
   - Key: ANTHROPIC_API_KEY
   - Value: sk-ant-... (본인 Anthropic API 키)
4. Deploy 클릭

### 3단계 — 완료
- https://your-project.vercel.app 주소로 누구나 접속 가능
- API 키는 Vercel 서버에만 저장되어 외부에 노출되지 않음

## 파일 구조
```
b2b-sales-agent/
├── api/
│   └── chat.js        ← 백엔드 (API 키 숨김)
├── public/
│   └── index.html     ← 프론트엔드
├── vercel.json        ← Vercel 설정
└── README.md
```

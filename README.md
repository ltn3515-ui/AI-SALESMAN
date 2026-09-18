# M10 AI SALESMAN

소상공인을 대신해 고객의 요구를 파악하고, 가격 규칙으로 견적을 계산하고, 예약 요청까지 연결하는 **AI 영업사원 MVP**입니다.

## MVP 핵심 기능
- 실시간 고객 Need 목록
- 구매의도(HIGH/MEDIUM) 표시
- 고객 요구사항 구조화
- Rule Engine 기반 자동 견적
- 견적 확정 / 예약 요청 상태 변경
- AI 상담 시뮬레이터
- 모바일 반응형 UI
- Mock 데이터 기반 즉시 실행

## 설계 원칙
1. LLM은 고객 의도와 조건을 구조화합니다.
2. 실제 가격 계산은 LLM이 아니라 Quote Rule Engine이 담당합니다.
3. 불확실한 조건은 추가 질문으로 보완합니다.
4. 예외 견적은 사람에게 넘길 수 있도록 확장합니다.
5. 장기적으로 AI SALESMAN → NEED ENGINE → NEED MARKET → CPN(Cost Per Need)로 확장합니다.

## 기술 스택
React + TypeScript + Vite + Lucide

## 실행
```bash
npm install
npm run dev
```

## 다음 단계
Supabase/Firebase 저장, 실제 LLM Structured Output, 업체별 Rule Builder, 예약 캘린더, 카카오톡/웹 문의 연결, 상담 전환 분석, 멀티테넌트 SaaS.

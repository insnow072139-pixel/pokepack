# Pokémon Card Pack Game v3

원래 카드팩 개봉 게임 컨셉의 UI로 복원한 버전입니다.

## Render
- Build Command: `npm install`
- Start Command: `npm start`
- Environment Variable: `DATABASE_URL` = Render PostgreSQL Internal Database URL

## GitHub
압축을 푼 폴더의 **내용물**을 저장소 루트에 업로드하세요. `server.js`, `package.json`, `public`이 저장소 최상단에 있어야 합니다.

## 주요 기능
- 30종 카드팩, 가격 낮은 순
- 최대 15,000 TCGdex 카드 풀
- 앞 카드 일반/낮은 등급, 마지막 카드 희귀 슬롯
- 고가 팩일수록 마지막 슬롯 고급 등급 확률 증가
- TCGdex 이미지 재시도: high.webp → high.png → low.webp → low.png → high.jpg
- 이미지 실패 문구 미표시
- PostgreSQL 회원/돈/보유 카드 저장
- bcrypt 비밀번호 해싱
- Socket.IO 온라인/랭킹/배틀 알림

# 2027 정미년 신년운세 4종 · 로로

2027년 정미년(丁未年) 신년운세를 보여주는 웹페이지입니다.
정적 HTML 한 장과 이미지 두 개로 이루어져 있고, GitHub Pages로 배포됩니다.
모든 운세는 100% 무료이며, 서버·AI 호출 없이 브라우저에서만 계산됩니다.

## 보기

https://roro0913.github.io/roro-2027-saju/

## 운세 4종

- **자미두수** — 2027년 명궁·월별 기복·4대 영역·실수 3가지
- **일본 운세** — 九星気学 본명성 + 2027년 오미쿠지(御神籤) + 길방위
- **인디언 운세** — 북미 원주민 수호동물(토템) 12종
- **별자리 운세** — 서양 12궁 2027

## 후원 링크 넣는 곳

`index.html` 안의 `SUPPORT_LINKS` 객체에 후원 링크를 넣으면
후원 시트의 "카카오페이로 후원하기" 버튼이 그 주소로 연결됩니다.
지금은 카카오페이 QR 송금 링크 하나(`KAKAOPAY_LINK`)를 네 단계에 모두 연결해 두었고,
보내는 사람이 송금 화면에서 금액을 직접 입력합니다.
링크를 비워 두면 "준비 중" 안내가 나오고 나머지 기능은 그대로 동작합니다.

```js
const KAKAOPAY_LINK = 'https://qr.kakaopay.com/FKtd5i3WS';
const SUPPORT_LINKS = {
  cookie: KAKAOPAY_LINK,   // 1,000원 · 로로 붕어빵
  coffee: KAKAOPAY_LINK,   // 5,000원 · 로로 아아 한 잔
  cake:   KAKAOPAY_LINK,   // 10,000원 · 로로 당 충전 케이크
  bag:    KAKAOPAY_LINK    // 30,000원 · 로로 새 가방 보태기
};
```

## 구성

- `index.html` — 페이지 본문(스타일·스크립트 포함)
- `assets/roro_fortune.png` — 도사 로로 이미지
- `assets/roro_loading.gif` — 로딩 애니메이션

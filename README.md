# NoTrace Privacy Policy

NoTrace 크롬 확장 프로그램의 개인정보 처리방침(한국어/English/日本語)을 담은 정적 페이지입니다.

공개 주소: https://widkhdl11.github.io/notrace-privacy/

`index.html` 을 고치고 `git push` 하면 1~2분 뒤 같은 주소에 반영됩니다.

## 이 문서가 기준으로 삼은 빌드

`notrace-v0.8-free` (manifest `version: 0.8.0`) 와 대조해 작성했습니다.

- 권한 다섯 개(`history`·`storage`·`bookmarks`·`activeTab`·`tabs`)가 3항의 설명과 일치
- `fetch`·`XMLHttpRequest`·`WebSocket`·`sendBeacon` 전 파일 0건 → 1항의 "외부 전송 없음"
- `config.js` 의 `PAYMENTS_ENABLED = false` → 4항을 「향후 제공 시」 조건문으로 작성

## 확장 프로그램을 고칠 때 같이 고쳐야 하는 것

- **권한을 추가하면** 3항에 그 권한의 사용 이유를 추가한다. 웹스토어 심사는 manifest 와 이 문서를 대조한다.
- **결제를 켜면**(`PAYMENTS_ENABLED = true`) 4항의 조건문을 단정문으로 바꾸고, 웹스토어 「데이터 사용」
  양식의 제3자 공유 항목도 함께 고친다. 지금은 양쪽 다 "없음"으로 맞춰져 있다.
- **저장 위치를 늘리면**(sync/local/session 에 새 키를 쓰면) 2항에 적는다. 2항은 저장하는 것을
  전부 열거하는 자리다.
- 위 중 하나라도 고치면 세 언어의 최종 수정일을 함께 올린다.

## 주의

- 저장소를 비공개로 바꾸거나, 이름을 바꾸거나, GitHub 사용자명을 바꾸면 위 주소가 404가 됩니다.
  그 주소는 크롬 웹스토어에 등록돼 있으므로 끊기면 심사 위반 사유가 됩니다.

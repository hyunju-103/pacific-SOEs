# Pacific SOE Fiscal Risk Monitor — 웹페이지 버전

`index.html` 파일 하나가 대시보드 전체입니다. Streamlit도, 파이썬도, 서버도 필요 없습니다.
파일을 더블클릭하면 내 컴퓨터 브라우저에서 바로 열립니다.

## 탭과 주소

탭을 누르면 해당 화면으로 바뀌고, 탭마다 링크가 따로 있습니다.

| 탭 | 주소 끝부분 |
|---|---|
| Overview | (없음) 또는 `#overview` |
| Sectors | `#sectors` |
| Countries | `#countries` |
| Early warning calculator | `#calculator` |
| Trigger rules | `#triggers` |

## 인터넷에 올리기: GitHub Pages (무료)

1. GitHub에서 새 저장소를 만듭니다. 무료 계정이면 **Public**이어야 합니다. 예: `pacific-soe`
2. "Add file → Upload files"로 `index.html`을 올리고 Commit 합니다.
3. 저장소의 **Settings → Pages**에서 Source를 **Deploy from a branch**, Branch를 **main**, 폴더를 **/ (root)**로 고르고 Save를 누릅니다.
4. 몇 분 뒤 `https://<GitHub아이디>.github.io/pacific-soe/` 주소가 생깁니다.

이 주소를 홈페이지 버튼에 연결하면 됩니다. Streamlit과 달리 잠드는 일이 없어서 누르면 바로 열립니다.

## 다른 방법

- 기관 홈페이지 담당자에게 `index.html`을 주고 홈페이지 서버에 올려 달라고 해도 됩니다. 그러면 기관 도메인 주소로 열립니다.

## 수정할 때

- 논문 수치는 파일 아래쪽 `<script>` 안의 `SECTORS`, `ZSECT`, `COUNTRIES` 등에 있습니다.
- 색상은 파일 위쪽 `:root { ... }` 안에 있습니다 (네이비 #002244, 블루 #009FDA).
- 계산기 프리셋과 트리거 규칙은 설명용 예시 값입니다.

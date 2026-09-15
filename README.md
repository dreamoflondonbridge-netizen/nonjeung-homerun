# ⚾ 논증 홈런

중학교 국어 수업용 논증 학습 야구 미니게임입니다.

## 이미지 교체

`images` 폴더에 아래 파일명을 그대로 사용하면 게임 화면에 자동 적용됩니다.

- `stadium-bg.png` — 야구장 배경·관중석·외야 펜스를 합친 이미지
- `baseball.png` — 공
- `pitcher.png` — 투수
- `batter.png` — 타자
- `runner.png` — 주자
- `defender-1.png` ~ `defender-4.png` — 수비수

사진을 업로드하지 않은 슬롯은 기존 레트로 픽셀 스타일이 fallback으로 보입니다.

배포 사이트: https://dreamoflondonbridge-netizen.github.io/nonjeung-homerun


## 문제 직접 추가·삭제하기

문제는 [questions.js](./questions.js)에서 관리합니다. GitHub에서 이 파일을 열고 연필 아이콘(Edit this file)을 누르면 문제를 수정할 수 있습니다.

- 문제 삭제: 원하는 문제의 `{ ... },` 블록을 삭제합니다.
- 문제 추가: 배열 안에 아래 형식의 블록을 복사해 넣습니다.

    {type:'method',label:'설명 방법',question:'문제 내용',options:['정의','예시','비교','분류'],answer:'정의',explanation:'정답인 이유를 설명합니다.'},

사용 가능한 type은 `argument`, `method`, `structure`, `analysis`, `boss`입니다. 일반 문제를 9개 이상 넣고, `boss` 문제는 마지막 문제용으로 1개 유지하세요. 수정 후 Commit changes를 누르면 GitHub Pages에 자동 반영됩니다.

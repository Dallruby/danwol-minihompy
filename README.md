# 그놈들은 오늘도 멋있었다 · 미니홈피

2004년 단월사립고 학생들의 싸이월드 미니홈피를 모바일 세로형으로 재편한 정적 사이트.
크랙AI 연재작 `2000년대 귀여니 소설풍` 프롬프트의 홍보 · 세계관 소개용.

빌드 없음, 의존성 없음. `index.html` 하나로 동작한다.

## 구조

```
index.html   전체 (스타일 · 마크업 · 스크립트)
bgm/         인물별 BGM 5개 (you · junrae · wonho · seolhee · suhyun)
img/         미니룸 5개 · 사진첩 11장 (webp)
```

아직 안 들어간 것은 YOU 사진 2장뿐이다. 아래 이름 그대로 `img/` 에 넣으면 자동으로 붙는다.

```
img/photo_user_1.webp   img/photo_user_2.webp
```

파일이 없으면 회색 자리 표시가 대신 떠서 레이아웃은 안 무너진다.
마준래는 사진첩 0장이 정상 (캐릭터 코드).

## 로컬 실행

브라우저에서 `index.html` 을 열거나, 오디오 자동재생 확인용으로 간단한 서버를 띄운다.

```
python3 -m http.server 8000
```

## 배포 (GitHub Pages)

`main` 에 푸시하면 `.github/workflows/pages.yml` 이 자동으로 GitHub Pages 에 배포한다.
주소: https://dallruby.github.io/danwol-minihompy/

자세한 콘텐츠 · 스킨 · 시대 고증 규칙은 [`인수인계.md`](./인수인계.md) 참고.

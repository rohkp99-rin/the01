# 🐶 초원의 햇살을 닮은 너에게 (Warm Puppy Letter Card)

따뜻하고 고급스러운 분위기의 인터랙티브 웹 편지 카드입니다.  
전체 화면 배경 이미지 위에 은은한 빛줄기와 하트 파티클이 어우러지며, 애틋한 편지 문구가 위에서 아래로 부드럽게 내려오듯 펼쳐집니다.

---

## ✨ 주요 기능

- **풀스크린 시네마틱 배경**: 강아지 이미지를 전체 화면으로 배치하고, 은은하게 확대되는 켄 번즈(Ken Burns) 줌 효과와 따뜻한 앰버 비네팅을 적용했습니다.
- **캐스케이드 편지 애니메이션**: 고운 바탕체(`Gowun Batang`)로 작성된 편지 문단들이 위에서 아래로 순차적으로 내려오며 나타납니다. 하단의 **다시 읽기** 버튼으로 언제든 애니메이션을 재실행할 수 있습니다.
- **빛줄기 & 하트 파티클 효과**: 대각선으로 비치는 부드러운 햇살 빛줄기(CSS)와 아래에서 위로 떠오르는 하트 및 금빛 입자(HTML5 Canvas)가 몽환적인 분위기를 연출합니다.
- **내장 오르골 멜로디 (Web Audio API)**: 별도의 외부 `.mp3` 파일 없이도 브라우저에서 바로 잔잔한 피아노·오르골 아르페지오가 재생됩니다. 우측 상단 **음악 켜기/끄기** 버튼으로 제어할 수 있습니다.
- **모바일 반응형 디자인**: 데스크톱과 모바일 환경 모두에서 강아지의 모습이 가려지지 않도록 카드 위치와 여백, 글자 크기가 자동으로 최적화됩니다.

---

## 📂 폴더 구조

```text
.
├── index.html      # 메인 HTML, CSS 스타일 및 애니메이션·오디오 스크립트
├── a.jpg           # 전체 화면 배경으로 사용되는 강아지 이미지
└── README.md       # 프로젝트 안내 문서
```

---

## 🚀 실행 및 배포 방법

### 1. 로컬에서 실행하기
별도의 빌드 도구나 서버 설치 없이 `index.html` 파일을 웹 브라우저(Chrome, Safari, Edge 등)로 열면 바로 실행됩니다.

### 2. GitHub Pages로 웹에서 공유하기
1. 이 저장소의 **Settings** > **Pages** 메뉴로 이동합니다.
2. **Build and deployment**의 Source를 `Deploy from a branch`로 선택합니다.
3. Branch를 `main` (또는 `master`), 폴더를 `/ (root)`로 설정한 뒤 **Save**를 누릅니다.
4. 잠시 후 생성되는 `https://<사용자아이디>.github.io/<저장소이름>/` 링크를 통해 모바일이나 PC에서 편지 카드를 공유할 수 있습니다.

---

## 🎨 커스터마이징 가이드

- **편지 내용 수정**: `index.html` 파일 내 `<div class="letter-body">` 영역의 `<p class="letter-line">` 문구를 원하는 내용으로 수정하세요. 문단을 추가할 경우 `style="--order: 4;"`처럼 순번을 1씩 늘려주면 자연스럽게 이어집니다.
- **배경 이미지 변경**: 같은 폴더에 새 이미지를 넣고 `index.html`의 `.bg-image` 스타일에서 `background-image: url('a.jpg');` 경로를 변경하면 됩니다.

---

## 🛠️ 사용 기술

- **HTML5 & CSS3** (Glassmorphism, CSS Keyframe Animations, Flexbox)
- **Vanilla JavaScript** (HTML5 Canvas Particle System, Web Audio API Synthesizer)
- **Google Fonts** (`Gowun Batang`, `Cormorant Garamond`)
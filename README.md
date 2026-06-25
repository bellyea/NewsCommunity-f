# NewsCommunity Frontend

스포츠 뉴스 요약 및 댓글 커뮤니티 서비스의 프론트엔드 프로젝트입니다.

정적 HTML, CSS, JavaScript 기반으로 구현했으며, Spring Boot 백엔드 API와 연동하여 뉴스 목록, 뉴스 상세, 로그인, 회원 프로필, 댓글, 북마크, 고객지원 화면을 제공합니다.

## 주요 기능

- 네이버 스포츠 뉴스 TOP 20 목록 조회
- 뉴스 상세 페이지 및 조회수 처리
- JWT 기반 로그인/로그아웃 화면 연동
- 댓글, 좋아요, 북마크 기능 연동
- 회원 프로필 조회 및 프로필 이미지 표시
- 고객지원 게시글 작성 및 조회
- 날씨 API 연동 UI

## 기술 스택

- HTML
- CSS
- JavaScript ES6
- Fetch API
- AWS CloudFront 연동 이미지 조회

## 폴더 구조

```text
.
├── index.html          # 뉴스 목록 페이지
├── detail.html         # 뉴스 상세 페이지
├── login.html          # 로그인 페이지
├── profile.html        # 프로필 페이지
├── support.html        # 고객지원 페이지
└── static
    ├── js              # API 연동 및 화면 제어 스크립트
    ├── *.css           # 페이지별 스타일
    └── profile_pics    # 기본 프로필 이미지
```

## 백엔드 연동

이 프론트엔드는 별도 백엔드 API 서버와 연동됩니다.

백엔드 저장소: NewsCommunity-b

주요 API 연동 영역:
- /api/login
- /api/signup
- /api/news
- /api/news/details/{id}
- /api/comments
- /api/bookmarks
- /api/user/profile
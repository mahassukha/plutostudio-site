# PLUTO STUDIO — GitHub Pages 사이트

이 폴더를 그대로 GitHub에 업로드하면 웹사이트가 됩니다.

- 사이트 이름: **PLUTO STUDIO (플루토 스튜디오)**
- 문의 이메일: **plutonostudio@gmail.com**
- 포함 페이지: Home / Portfolio / About / Contact
- 운영 방식: 이미지 추가 → GitHub 업로드 → 자동 반영

## 폴더 구조

- `index.html` 홈
- `portfolio.html` 포트폴리오(갤러리)
- `about.html` 소개 + 프로필 사진
- `contact.html` 메일 문의 링크
- `covers.json` 갤러리 데이터(이미지 목록)
- `images/` 표지 이미지 + 프로필 사진
- `style.css` 스타일

## GitHub Pages 켜는 법

1) GitHub에서 새 Repository 생성 (Public 권장)
2) 이 폴더의 파일들을 Repository 루트에 업로드
3) Repository → Settings → Pages  
   - Source: `Deploy from a branch`  
   - Branch: `main` / Folder: `/ (root)`  
4) 생성된 URL로 접속

## 커스텀 도메인(가비아) 연결 요약

- GitHub Settings → Pages → **Custom domain** 에 `www.도메인.com` 입력 후 저장
- 가비아 DNS:
  - `A` 레코드(루트 도메인 @):
    - `185.199.108.153`
    - `185.199.109.153`
    - `185.199.110.153`
    - `185.199.111.153`
  - `CNAME` 레코드:
    - `www` → `username.github.io`

DNS 반영은 보통 수분~최대 24시간 걸릴 수 있습니다.
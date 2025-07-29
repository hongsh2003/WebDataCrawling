# WebDataCrawling

# 📚 Naver Webtoon Thumbnail Crawler

크롬 브라우저와 Selenium, BeautifulSoup을 활용해 **네이버 웹툰** 메인 페이지에 노출된 웹툰들의 썸네일 이미지를 수집하고 저장하는 Python 크롤러입니다.

---

## 🖼️ 기능 소개

- ✅ 네이버 웹툰 메인 페이지 로딩
- ✅ BeautifulSoup을 통한 웹툰 제목 및 썸네일 이미지 URL 추출
- ✅ 이미지 중복 저장 방지 및 파일명 안전화 처리
- ✅ `webtoon_images/` 폴더에 썸네일 이미지 저장

---

## 🛠️ 사용 기술

| 기술 | 설명 |
|------|------|
| Python | 크롤러 작성 언어 |
| Selenium | 동적 웹 페이지 렌더링 대응 |
| BeautifulSoup | HTML 파싱 및 데이터 추출 |
| requests | 이미지 요청 및 다운로드 |
| Pillow (PIL) | 이미지 처리 및 저장 |
| re, os | 정규표현식 및 파일 관리 |

---

## 📁 결과물 예시

- `webtoon_images/` 폴더에 웹툰별 `.png` 썸네일 저장
- 저장된 파일명 예시:
  - `용사생활기록부.png`
  - `참교육.png`
  - `시리도록 불꽃처럼.png`

---

## 🔐 예외 처리 및 보완

- 이미지 다운로드 실패 시 예외 메시지 출력
- Windows에서 사용 불가능한 문자는 정규식으로 제거하여 안전한 파일명 구성

---

## 📝 주의 사항

본 프로젝트는 **개인 학습 및 비상업적 연구 목적**으로만 사용되어야 하며,  
수집한 웹툰 이미지의 저작권은 **NAVER WEBTOON Corp.**에 있습니다.  
상업적 목적의 사용, 무단 배포는 법적 문제가 발생할 수 있습니다.

---

## 👤 개발자 정보

- **이름**: 홍수현
- **GitHub**: https://github.com/hongsh2003
- **Email**: 1639.sue.hong@gmail.com

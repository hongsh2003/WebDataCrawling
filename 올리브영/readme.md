# 🧴 올리브영 스킨케어 랭킹 크롤러

이 프로젝트는 올리브영(OliveYoung) 공식 웹사이트의 **스킨케어 랭킹 1위부터 100위까지**의 상품 정보를 크롤링하여, **MySQL 데이터베이스에 저장**하는 Python 기반 자동화 프로그램입니다.

---

## 📌 주요 기능

- ✅ 올리브영 스킨케어 BEST 100 랭킹 웹 크롤링
- ✅ 상품명, 정가, 할인가, 순위 수집
- ✅ Pandas를 활용한 정리 및 저장
- ✅ SQLite DB 저장 (임시 백업용)
- ✅ MySQL DB 저장 (실제 데이터 적재)

---

## 🛠 사용 기술

- Python 3.x
- pandas
- BeautifulSoup4
- requests
- pymysql
- sqlite3

---

## 🗂 데이터 컬럼 구성

| 컬럼명           | 설명           |
|------------------|----------------|
| `rank_order`     | 순위 (1~100)   |
| `name`           | 상품명         |
| `original_price` | 정가 (없을 수도 있음) |
| `discounted_price` | 할인가       |

---

## 📦 설치 및 실행 방법

### 1. 패키지 설치
```bash
pip install pandas beautifulsoup4 requests pymysql
```

### 2. MySQL 데이터베이스 생성
```sql
CREATE DATABASE oliveyoung CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
```

### 3. Python 실행
```bash
python main.py
```

> 💡 `main.py`에는 크롤링 + SQLite 저장 + MySQL 저장 코드가 포함되어야 합니다.

---

## 💾 예시 결과

- `skincare_ranking1.csv` : CSV 파일로 저장된 랭킹 정보  
- `oliveyoung.db` : SQLite DB 파일  
- `oliveyoung_skincare` : MySQL 테이블 (DB: oliveyoung)

---

## ✍️ 작성자

- 작성자: 홍수현
- 이메일: 1639.sue.hong@gmail.com
- GitHub: https://github.com/hongsh2003

# MySQL 8.0 설치 및 데이터 이행 가이드

Oracle Linux 7.9 환경에서 MySQL 8.0 Community Server 설치 및
Oracle 19c HR 스키마 데이터 이행 가이드입니다.

---

## 환경 구성

| 항목 | 내용 |
|------|------|
| OS | Oracle Linux 7.9 (UEK 5.4.17) |
| DB 버전 | MySQL 8.0 Community Server |
| IP | 192.168.23.67 |
| SELinux | Enforcing |
| firewalld | 활성 (기본 3306 미개방) |

---

## 설치 순서

| 순서 | 문서 | 설명 |
|------|------|------|
| 1 | [MySQL 8.0 설치](./1.%20MySQL%208.0%20설치.md) | MariaDB 제거 / MySQL 설치 / 보안 초기화 / 방화벽 설정 |
| 2 | [Oracle HR 스키마 MySQL 이행](./2.%20Oracle%20HR%20스키마%20MySQL%20이행.md) | Python 기반 DDL 생성 / 데이터 이행 / 검증 |

---

## 주요 특징

- MariaDB 잔재 제거 후 MySQL 8.0 설치
- SELinux Enforcing 환경에서의 설치 및 설정
- firewalld 3306 포트 개방
- mysql_secure_installation 보안 초기화
- Python(cx_Oracle + mysql-connector)을 활용한 Oracle → MySQL 데이터 이행
- Oracle Data Dictionary 기반 DDL 자동 생성
- 테이블별 건수 검증 포함
- Access denied 트러블슈팅 포함


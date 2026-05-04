# MySQL 8.0 설치 가이드

Oracle Linux 7.9 환경에서 MySQL 8.0 Community Server 설치 가이드입니다.
MariaDB 잔재 제거부터 보안 초기화, 방화벽/SELinux 설정까지 전 과정을 다룹니다.

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

| 순서 | 문서 |
|------|------|
| 1 | [MySQL 8.0 설치](./1.%20MySQL%208.0%20설치.md) |

---

## 주요 특징

- MariaDB 잔재 제거 후 MySQL 8.0 설치
- SELinux Enforcing 환경에서의 설치 및 설정
- firewalld 3306 포트 개방
- mysql_secure_installation 보안 초기화
- Access denied 트러블슈팅 포함

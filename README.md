# plecko_gittest
Git Practice Repository

## 1. git 공통 작업 원칙

* 매 작업 시작 전  
```bash
git switch dev
git pull origin dev
git switch -c usr/benkim
```

## 2. PR 권한 (Branch Protection) 및 Code Owner 설정 방법

* 해당 repository  → Settings → Branches → Add branch ruleset

* Ruleset name 설정: ex) PR 규칙

* Enforcement Status: Active

* Branch rules
✔ Require a pull request before merging
✔ Require approvals (1 이상)
✔ Require review from Code Owners

* Code Owner 설정 방법 

1. 아래 경로에 CODEOWNER 파일 생성
.github/CODEOWNERS

2. 기본 설정 (전체 파일에 대해 jhyoo가 코드 오너)
* @PK-jhyoo


3. (필요 시) +폴더별 책임자 지정 가능 
/src/ @jhyoo
/docs/ @benkim


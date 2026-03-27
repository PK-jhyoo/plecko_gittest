# plecko_gittest
Git Practice Repository

---

## 1. Git 공통 작업 시작 전 (필수)
개인 브랜치를(usr/NAME) 항상 최신 상태(dev)로 유지하기 위해 진행한다.

```bash
git switch dev
git pull origin dev
git switch usr/NAME
```

## 2. Pull Request (PR) 규칙 초기 설정 방법
  
```해당 Repository → Settings → Branches → Add ruleset```
* Ruleset Name: ex)PR 규칙
* Enforcement Status: Active
* Branch Rules
    * Require a pull request before merging
    * Require approvals (최소 1명 이상)
    * Require review from Code Owners

### 2-1. Code Owners 설정 방법
* 파일 위치
```.github/CODEOWNERS```

* 파일 내용 (전체 폴더에 대하여 코드 오너 지정)
```* @PK-jhyoo```

* (필요 시) 폴더별 책임자 지정도 가능
```bash
/src/  @jhyoo
/docs/ @benkim
```


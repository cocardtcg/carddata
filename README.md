# Cocard Card Data

코난 TCG 카드 데이터 레포입니다.

## 데이터 URL

https://cocardtcg.github.io/carddata/v1/

## 구조

```
v1/
  manifest.json     # 버전 + 파일별 MD5 해시
  cards/*.json      # 세트별 카드 데이터
  nameTable.json    # 카드 이름 일→한 매핑
  traitTable.json   # 특성 일→한 매핑
  sets.json         # 세트 그룹 정보
  prOrigin.json     # PR 카드 원본 세트 매핑
```

## 업데이트

앱에서 `manifest.json`의 MD5 해시를 비교하여 변경된 파일만 다운로드합니다.

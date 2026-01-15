## Inferface
### Input
`$ARGUMENTS`: 코드분석 및 `CLAUDE.MD`를 생성할 모듈의 경로 (예: `infrastructure/modules/s3-bucket`, `services/user-authentication`)
### Output
`CLAUDE.md` 파일을 ``$ARGUMENTS`에 생성

## Work Item
### 코드분석

### CLAUDE.md 생성
다음 구조의 `CLAUDE.md`를 생성
```
# 개요
- 해당 코드가 무엇을 하는지 간단히 설명

# 아키텍처 
- ASCII 또는 텍스트 기반 흐름도 (해당되는 경우)
- 다른 모듈과의 인터페이스

# 리소스
## Cloud 리소스(해당되는 경우)
생성되는 Cloud(AWS, Azure, GCP 등) 리소스 목록 (테이블 형식)
## Database(해당되는 경우)
```

## Remarks
- 기존 `CLAUDE.md`가 있으면 덮어쓰기 전에 확인요청
- 코드를 기반으로 정확한 문서를 작성
- 한국어로 작성

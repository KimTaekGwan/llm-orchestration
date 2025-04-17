git submodule update --remote dify

# Dify 서브모듈 동기화 방법

## 1. 서브모듈 업데이트

```bash
# 서브모듈의 최신 변경사항을 가져옵니다
git submodule update --remote dify
```

## 2. 커스텀 변경사항이 있는 경우 동기화

dify 디렉토리 내에 커스텀 파일이나 수정사항이 있는 경우, 다음 단계를 따르세요:

```bash
# 1. dify 디렉토리로 이동
cd dify

# 2. 변경사항 커밋
git add .
git commit -m "커밋 메시지"

# 3. 원본 저장소와 동기화
git fetch upstream
git merge upstream/main

# 4. 변경사항을 fork한 저장소에 push
git push origin main

# 5. 메인 디렉토리로 돌아가기
cd ..
```

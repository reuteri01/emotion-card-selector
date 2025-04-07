# 반쯤 감정카드 선택기 배포 패키지

이 패키지는 "반쯤 감정카드 선택기" 애플리케이션의 배포 파일을 포함하고 있습니다.

## 배포 방법

### Cloudflare Pages 배포

1. GitHub 저장소 생성:
   - 이 디렉토리의 내용을 GitHub 저장소로 푸시합니다.

2. Cloudflare Pages 설정:
   - Cloudflare 계정에 로그인합니다.
   - Pages 메뉴에서 "Create a project"를 선택합니다.
   - GitHub 저장소를 연결합니다.
   - 빌드 설정:
     - 프레임워크 프리셋: Next.js
     - 빌드 명령어: `npm run build`
     - 빌드 출력 디렉토리: `.next`
   - 배포 버튼을 클릭합니다.

### 로컬에서 실행

```bash
# 종속성 설치
npm install

# 개발 서버 실행
npm run dev

# 프로덕션 빌드
npm run build

# 빌드 결과 확인
npm run start
```

## 문서

- `deployment-guide.md`: 상세한 배포 가이드
- `user-guide.md`: 사용자 가이드

## 지원

문제가 발생하면 개발자에게 문의하세요.


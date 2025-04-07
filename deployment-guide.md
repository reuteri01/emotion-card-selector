# 배포 가이드

## 1. 빌드 및 최적화

### 빌드 명령어
```bash
# 개발 서버 실행
npm run dev

# 프로덕션 빌드
npm run build

# 빌드 결과 확인
npm run start
```

### 성능 최적화 체크리스트
- 이미지 최적화 (WebP 형식 사용)
- 코드 스플리팅 확인
- 불필요한 종속성 제거
- CSS 최적화
- JavaScript 번들 크기 최소화

## 2. 배포 옵션

### Cloudflare Pages 배포 (권장)
1. Cloudflare 계정 로그인
2. Pages 메뉴에서 "Create a project" 선택
3. GitHub 저장소 연결
4. 빌드 설정:
   - 프레임워크 프리셋: Next.js
   - 빌드 명령어: `npm run build`
   - 빌드 출력 디렉토리: `.next`
5. 환경 변수 설정 (필요한 경우)
6. 배포 버튼 클릭

### Vercel 배포 (대안)
1. Vercel 계정 로그인
2. "New Project" 선택
3. GitHub 저장소 가져오기
4. 프로젝트 설정 확인
5. 배포 버튼 클릭

### 수동 배포
1. 정적 빌드 생성: `npm run build && npm run export`
2. `out` 디렉토리의 파일을 웹 서버에 업로드
3. 웹 서버 설정 (Nginx, Apache 등)

## 3. 도메인 설정
1. 도메인 등록 (필요한 경우)
2. DNS 설정:
   - A 레코드: 서버 IP 주소 지정
   - CNAME 레코드: 서브도메인 설정
3. SSL 인증서 설정 (Let's Encrypt 권장)

## 4. 모니터링 및 분석
1. Google Analytics 설정
2. 오류 모니터링 도구 설정 (Sentry 등)
3. 성능 모니터링 설정 (Lighthouse, PageSpeed Insights)

## 5. 유지 관리
1. 정기적인 종속성 업데이트
2. 보안 패치 적용
3. 백업 전략 수립
4. 사용자 피드백 수집 및 개선사항 반영

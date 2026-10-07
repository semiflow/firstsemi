# Flat AI 홈페이지

정적 사이트(단일 `index.html`). 빌드 불필요.

## 배포 전 수정
- `index.html`의 `mailto:hello@example.com` → 실제 연락 이메일
- 커스텀 도메인: 루트에 `CNAME` 파일 생성, 내용은 도메인 한 줄 (예: `flatai.kr`)

## GitHub Pages 배포
1. 저장소 Settings → Pages → Source: `Deploy from a branch`, 브랜치/폴더 `/ (root)` 선택
2. Custom domain에 도메인 입력 → DNS 확인 후 `Enforce HTTPS` 체크

## 가비아 DNS 설정 (My가비아 → DNS 관리 → 레코드 수정)
| 타입 | 호스트 | 값 |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | `<GitHub사용자명>.github.io.` |

전파까지 수 분~최대 48시간.

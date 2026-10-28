화목 훈련 페이스 신규 앱 v1.0
신규 앱이며 기존 Vercel 프로젝트를 변경하지 않습니다.
배포 방법: Vercel에서 신규 프로젝트를 1회 생성하고 이 폴더의 파일을 루트에 배포하세요.
기존 앱 업데이트가 아닙니다. 실제 서버 배포는 수행하지 않았습니다.
사용자 입력은 각 기기의 localStorage에 저장됩니다.
입력: 3930 또는 39:30. 파트 + 추가 / - 삭제, 최소 1개, 최대 30개.
공유: 브라우저 지원 시 공유 시트, 아니면 PNG 다운로드.

[v1.1] 4930 / 49:30 / 49분30초 입력 지원. Enter 확정 후 다음 PART로 포커스 이동.
기존 앱 업데이트 시 기존 Vercel projectId와 Production URL 확인 후 동일 프로젝트 Production에 배포하세요. 새 프로젝트 생성 금지. 기존 PWA 및 localStorage 데이터 유지.

[v1.2] VO₂max 90% / LT 인터벌 모두 400m, 200m, 100m 각각 원래 계산값에서 정수 반올림하여 표시. 이미지도 동일. 계산 단계에서 미리 반올림하지 않음.
배포 전 확인: 기존 projectId, Production URL, Production 대상, PWA manifest, 사용자 데이터 저장(localStorage key: nirc-tue-thu-pace-v1).
배포 후 확인: 기존 URL 최신 버전, 페이스 표시 및 이미지, 홈 화면 바로가기, 기존 기록 보존. 이 ZIP은 배포가 아님.

[v1.3] 거리별 독립 계산 확정: 10K 총 초 / 10 + (VO₂max -10 또는 LT +10) = 1km 목표 초. 400/200/100m 각각 비례 계산 후 Math.round로 정수 반올림. 100m 반올림값을 배수로 곱하지 않음. 기존 localStorage 키 및 PWA manifest 유지.
기존 Vercel projectId 및 Production URL은 이 파일만으로 확인할 수 없으므로 배포 전에 기존 프로젝트에서 확인 필요. Production 배포 후 기존 URL에서 검증 필요.

[v1.3] 확인된 계산 방식 유지: 10K 기록에서 1km 훈련 페이스를 구한 뒤 400m/200m/100m 각각 독립 계산 및 정수 반올림. 100m 반올림 결과를 배수로 사용하지 않음.
기존 Vercel projectId 및 Production URL은 ZIP만으로 확인할 수 없으므로 배포 전 확인 필요.

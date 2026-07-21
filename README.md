# 조선 8도 수산물 지도 PWA (루트 아이콘 최종본)

## 업로드 파일
다음 파일 8개를 GitHub 저장소 루트에 그대로 올리면 됩니다.

- index.html
- manifest.json
- app.js
- service-worker.js
- data.json
- icon-192.png
- icon-512.png
- UI_AUDIT.json

## GitHub Pages 설정
1. 저장소에서 **Add file → Upload files**
2. 위 8개 파일을 모두 업로드
3. **Settings → Pages**
4. **Deploy from a branch** 선택
5. **Branch: main / Folder: /(root)** 선택
6. **Save**

## 홈 화면 아이콘 설치
### 안드로이드
- Chrome에서 GitHub Pages 주소 열기
- **앱으로 설치** 또는 **홈 화면에 추가** 선택

### 아이폰
- Safari에서 주소 열기
- **공유 → 홈 화면에 추가**

## 비고
- 이번 최종본은 아이콘 파일을 별도 폴더 없이 루트에 두도록 정리했습니다.
- 아이콘은 제공된 `조선_팔도지의_전통_아름다움.png`를 192px, 512px 규격으로 반영했습니다.


## v10.3 수정
- PC 마우스 오버 통계표를 아이콘 위가 아닌 좌우 측면에 표시
- 동쪽 도(함길도·강원도·경상도)는 오른쪽, 서쪽 도는 왼쪽에 표시
- 함길도 등 화면 상단 지역의 통계표 잘림 방지


## v10.5 105개 품목 카드 개정
- 105개 기준 카드의 현대 대응명, 계절·어기, 근거 문구를 검색증강 비교표 최종본 기준으로 반영했습니다.
- 239개 지역 기록 카드에도 동일 기준을 연동 반영했습니다.
- app.js가 등록하는 service-worker.js를 패키지에 포함했습니다.


## v10.5.1 교정
- JSON 내 SVG 줄바꿈이 JavaScript 문자열을 끊던 오류를 수정했습니다.
- 로컬에서 index.html을 직접 열어도 빈 화면이 생기지 않도록 내장 데이터 구문을 재생성했습니다.


## v10.5.3 실행 교정
- v10.5.2에서 잘못 재포장된 index.html을 제거하고, 문법검사를 통과한 교정본 index.html을 복원했습니다.
- service-worker.js를 루트에 포함하고 캐시 버전을 v10.5.3으로 갱신했습니다.

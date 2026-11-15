# 3D Marble Roulette (Three.js Edition)

기존 2D 마블 룰렛을 **Three.js + Cannon-es(3D 물리 엔진)** 기반으로 재구성하여, 입체적인 3D 트랙, 포토 피니시 슬로우 모션, 네온 블룸(Bloom) 효과, 3D 사운드, 그리고 **참여자 서식 불러오기(`.txt`, `.csv`, `.json`)** 기능을 지원하는 웹 애플리케이션입니다.

## 참고자료 및 원작자 표시 (Credits)
- **원작 (Original Concept & Format):** [lazygyu - Marble Roulette](https://lazygyu.github.io/roulette/) ([GitHub Repository](https://github.com/lazygyu/roulette))
- 본 프로젝트는 원작의 참여자 입력 서식(`이름*가중치`, 쉼표/줄바꿈 구분) 및 핵심 규칙(당첨 순위 지정, 셔플, 2배속 등)을 참고하여 3D 환경으로 새롭게 구현했습니다.

## 주요 기능
1. **Three.js 3D 스펙타클 연출**
   - `UnrealBloomPass` 네온 발광 효과, 실시간 그림자, 충돌 스파크 & 우승 폭죽(Confetti)
   - 자동 추적(Auto Follow) / 전체 뷰 / 자유 시점(OrbitControls) 카메라 전환
   - 목표 등수 구슬이 결승선에 근접하면 발동하는 **포토 피니시 슬로우 모션**
   - Web Audio API 기반 실시간 효과음 (핀 충돌, 범퍼, 부스터, 우승 팡파레)
2. **4가지 3D 코스**
   - 네온 피라미드 (Neon Pyramid)
   - 회전 풍차 캐니언 (Spinning Windmill)
   - 범퍼 & 부스터 (Turbo Chaos)
   - 메가 드롭 계곡 (Mega Drop)
3. **기존 서식 호환 & 파일 불러오기/내보내기**
   - 직접 입력: `짱구*2, 철수*3, 유리` (쉼표 또는 줄바꿈 구분, `*숫자` 가중치 지원)
   - 파일 불러오기(드래그 앤 드롭 지원): `.txt`, `.csv`, `.json`
   - 서식 저장(`.txt`) 및 CSV 양식 다운로드

## GitHub Pages 배포 방법
1. GitHub에서 새 저장소(Repository)를 생성합니다. (예: `marble-roulette-3d`)
2. 이 폴더(`index.html`, `README.md`, `.nojekyll`)의 파일들을 저장소 루트에 업로드(push)합니다.
3. 저장소 상단 **Settings** → 좌측 메뉴 **Pages**로 이동합니다.
4. **Build and deployment**의 Source를 **Deploy from a branch**로 선택하고, Branch를 `main` (폴더: `/ (root)`)으로 설정한 뒤 **Save**를 누릅니다.
5. 1~2분 후 `https://<내_깃허브_아이디>.github.io/<저장소_이름>/` 주소로 접속할 수 있습니다.

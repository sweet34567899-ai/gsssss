# Elemental Gaze (프로토타입) — Forge 1.20.1

## 빌드
1. JDK 17 설치.
2. Forge 1.20.1 MDK(47.3.x)를 받아 압축을 풀고, 이 프로젝트의 `src/`, `build.gradle`, `settings.gradle`을 덮어쓴다.
   (gradlew, gradle/ 폴더는 MDK 것을 그대로 사용)
3. `./gradlew build` → `build/libs/elementalgaze-0.1.0.jar` 을 `mods/` 폴더에 넣는다.
   개발 테스트는 `./gradlew runClient`.

## 조작
- R: 전투 모드 토글 (켜면 좌클릭 = 캐릭터 일반공격)   G: 성장 화면(스킬/스탯 레벨업)
- Z: 원소 전투 스킬(E)   X: 원소 폭발(Q)   (키 설정에서 변경 가능)

## 관리자 명령어 (OP)
- /gaze status | /gaze energy <n> | /gaze roll | /gaze reset | /gaze setchar <id>
- 예: /gaze energy 100 (두 번) → 빈 신의 눈 → 원소 발현

## 프로토타입 한계
- 몹 부착 원소는 1종, 반응은 증발/융해/과부하/감전/초전도/빙결만 구현
- 인챈트 활동, 설치 블록 추적(광질 어뷰징 방지)은 미구현
- 스킬 이펙트는 바닐라 파티클, 사운드는 바닐라 사운드로 대체
- 모든 수치는 data/elementalgaze/gaze_characters/*.json 및 config 에서 조정

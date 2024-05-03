# kotlin-baseball-precourse
- 카카오 테크 캠퍼스 1회차 미니과제
- 충남대학교 Android 1조 노수진

## 숫자 야구 게임 기능 요구 사항

### 1. 핵심 게임 플레이
플레이어는 컴퓨터(상대방)가 무작위로 생성한 1부터 9까지의 서로 다른 세 자리 숫자를 맞춰야 한다.

### 2. 게임 힌트 제공
- **스트라이크**: 추측한 숫자가 정확하고 위치도 정확한 경우
- **볼**: 추측한 숫자가 정확하지만 위치가 틀린 경우
- **낫싱**: 추측한 숫자가 모두 틀린 경우

### 3. 승리 조건
플레이어가 세 자리 숫자를 모두 정확하게 맞히면 게임에서 승리한다.

### 4. 게임 종료 옵션
게임이 끝난 후 플레이어는 게임을 다시 시작하거나 종료할 수 있다.

### 5. 입력 검증
- 사용자 입력이 1에서 9까지의 서로 다른 세 자리 숫자로 구성되었는지 검증한다.
- 잘못된 입력을 제공할 경우 **`IllegalArgumentException`**을 발생시키고 애플리케이션은 종료된다.



## 기능 목록(커밋 단위)

### 1. 프로젝트 설정, README 문서화
- 기본 README 문서 작성을 위한 프로젝트 초기화 수행
- 게임 방법과 규칙에 대한 README 문서를 업데이트
### 2. generator 생성
- 컴퓨터(상대방)가 1부터 9까지의 임의의 숫자 세 개를 생성
### 3. 사용자 입력 처리
- 사용자 입출력을 처리하는 Console 구현
- 사용자 입력을 검증하고 잘못된 입력에 대한 예외 처리 기능 추가
- 입력값에 따른 유닛 테스트 수행
### 4. 스트라이크,볼 판정 로직
- 스트라이크와 볼을 판정하는 핵심 게임 로직을 구현
- 결과값에 따른 유닛 테스트 수행
### 5. 게임 힌트 표시
- 사용자의 추측에 기반하여 게임 힌트(스트라이크, 볼, 낫싱)를 표시하는 기능을 구현
### 6. 게임 승리 확인
- 사용자가 게임을 이겼는지 확인하는 로직을 추가
### 7. 게임 재시작 또는 종료 옵션
- 게임 재시작 또는 종료 옵션을 구현
- 사용자가 잘못된 값을 입력할 경우 **`IllegalArgumentException`** 구현
### 8. 통합 테스트
- 통합 테스트를 수행하고 발견된 버그를 수정
### 9. 마무리 및 코드 정리
- 코드 가독성과 성능 향상을 위한 코드 정리
- 주석 추가
- README 파일 정리
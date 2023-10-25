## 구현할 기능 정리

1. 게임 시작 전
   - 게임 시작 안내 문구 출력
   
2. 게임 시작
   - 컴퓨터의 랜덤한 숫자 저장
     - 유저가 입력한 숫자 저장
       - 예외 처리
         - 3자리의 숫자가 아닌 경우 `IllegalArgumentException` 발생
         - 1 ~ 9까지의 숫자가 아닌경우 `IllegalArgumentException` 발생
         - null인 경우 `IllegalArgumentException` 발생
     - 컴퓨터의 수와 유저의 수 비교
       - 자리와 수 모두 같으면 `스트라이크` 판정
       - 숫자만 같으면 `볼` 판정
       - 아무것도 일치하지 않으면 `낫싱`판정
       - `3 스트라이크`달성 시 `게임 종료` 판정
       
3. 게임 종료 
   - 게임 종료 시 `1` 입력, `새로운 게임 시작`
   - 게임 종료 시 `2` 입력, `완전히 게임 종료`
   
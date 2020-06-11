# java-calculator
문자열 계산기 미션 저장소

## 학습 테스트  
  
### String 클래스에 대한 학습 테스트
        - split 했을 때 잘 분리되는지 확인하는 학습 테스트 구현  
          반환하는 값의 경우 assertj의 contain(), containsExactly() 사용  
        - String의 substring()을 사용해 () 괄호 제거하고 반환하도록 구현  
        - String의 charAt() 메소드 사용해 특정 위치 문자 가져오는 학습 테스트 구현  
          위치 값을 벗어나면 StringIndexOutOfBoundsException이 발생할 때 학습 테스트 구현  
          JUnit의 @DisplayNames을 활용해 의도 드러나도록 구현      
  
### Set Collection에 대한 학습 테스트  
        - Set의 size()를 활용해 Set의 크기 확인하는 테스트 구현
        - Set의 contains()를 활용해 1,2,3이 존재하는지 확인하는 학습테스트 구현  
          JUnit의 ParameterizedTest로 중복 코드 제거  
        - 2의 contains 메소트가 false일 때에 대한 테스트도 가능하도록 구현  
  
## 단위테스트
        - 사칙연산 수행하는 계산기 구현
        - 우선순위 아닌 입력 값에 따라 계산 순서 결정

## 기능 구현 목록
    - 문자열 입력
    - 공백을 기준으로 문자열 분리
    - 입력이 틀린 경우 다시 입력 
        + 숫자 뒤에 숫자 오는 경우
        + 연산자 뒤에 연산자 오는 경우애
        + 연산자로 문자열이 끝나는 경우
    - 분리한 문자열의 개수만큼 차례로 계산
        * 하나의 연산 끝나면 그 수와 다음 연산 진행
    - 연산 결과 출력
        
# javascript-lotto-precourse

## 기능 구현
1. 입출력 기능
  -  입력
     - [x] 금액 입력 : `구입금액을 입력해 주세요.\n`
     - [x] 당첨 번호 입력 (쉼표로 구분) : `당첨 번호를 입력해 주세요.\n`
     - [x] 보너스 번호 입력 : `보너스 번호를 입력해 주세요.\n`
  - 출력
    - [x] 구매 개수 : `${구매개수}개를 구매했습니다.`
    - [x] 로또 번호 출력
    - [x] 당첨 내역 출력 : `${일치한 개수}개 일치 (${수익}원) - ${해당 로또 개수}개`
    - [ ] 수익률 출력 : `총 수익률은 ${수익률}%입니다.`
      - [ ] 소수점 둘째 자리에서 반올림
    - [ ] 예외 사항 시 에러 문구 출력, 에러 문구는 [ERROR]로 시작
          ex) [ERROR] 로또 번호는 1부터 45 사이의 숫자여야 합니다.
2. 구매한 로또 번호들 확인 및 저장
    - [x] 구입 금액 / 1000 개의 로또 개수 확인
    - [x] 로또 번호 - 오름차순으로 저장
3. 일치 여부 확인 및 개수 저장
  - [x] : 하나의 로또 번호와 당첨 번호 일치 비교
  - [x] : 일치한 로또 번호의 개수 저장
  - [x] : 보너스 번호 일치 시, 다른 숫자로 저장
4. 에러 및 예외 처리
   - [ ] 로또 번호 숫자의 범위가 1~45가 아닌 경우
   - [ ] 1개의 로또에 중복되는 숫자가 들어가 있을 경우
   - [ ] 구입 금액, 당첨 번호, 보너스 번호가 숫자가 아닌 경우
   - [ ] 구입 금액이 1000원으로 나누어 떨어지지 않는 경우

## 프로그래밍 요구 사항
- [ ] indent(인덴트, 들여쓰기) depth를 3이 넘지 않도록 구현한다.
  - 예를 들어 while문 안에 if문이 있으면 들여쓰기는 2이다.
- [ ] 3항 연산자를 쓰지 않는다.
- [ ] 함수(또는 메서드)가 한 가지 일만 하도록 최대한 작게 만들어라.
- [ ] Jest를 이용하여 정리한 기능 목록이 정상적으로 작동하는지 테스트 코드로 확인한다.
- [ ] 함수(또는 메서드)의 길이가 15라인을 넘어가지 않도록 구현한다.
- [ ] else를 지양한다.
- [ ] 구현한 기능에 대한 단위 테스트를 작성한다. 단, UI(System.out, System.in, Scanner) 로직은 제외한다.
- @woowacourse/mission-utils에서 제공하는 Random 및 Console API를 사용하여 구현해야 한다.
  - [ ] Random 값 추출은 Random.pickNumberInRange()를 활용한다.
  - [ ] 사용자의 값을 입력 및 출력하려면 Console.readLineAsync()와 Console.print()를 활용한다.
- Lotto 클래스
    - [ ] 제공된 Lotto 클래스를 사용하여 구현해야 한다.
    - [ ] Lotto에 numbers 이외의 필드(인스턴스 변수)를 추가할 수 없다.
    - [ ] numbers의 접근 제어자인 #은 변경할 수 없다.
    - [ ] Lotto의 패키지를 변경할 수 있다.


## 공통 피드백
- [ ] 값을 하드 코딩하지 않는다.
- [ ] 클래스는 필드, 생성자, 메서드 순으로 작성한다.
- [ ] 한 메서드가 한 가지 기능만 담당하게 한다.
- [ ] 테스트를 작성하는 이유에 대해 본인의 경험을 토대로 정리해본다.
- [ ] 처음부터 큰 단위의 테스트를 만들지 않는다.
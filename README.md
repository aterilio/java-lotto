# 로또
## 진행 방법
* 로또 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

---

## 기능 목록
* 로또 구입 금액을 입력받으면 로또를 구매한다.
  * [x] 로또는 구입 금액 1000원 당 1장을 구매할 수 있다.
  * [x] 로또 구입 금액이 음수이면 예외가 발생한다.
* 로또는 중복되지 않는 1-45 범위의 숫자 6개로 구성된다.
  * [ ] 1-45 범위에 속하지 않는 숫자가 있으면 예외가 발생한다.
  * [ ] 중복된 숫자가 있으면 예외가 발생한다.
* 당첨 번호를 입력받아 생성된 로또와 비교하여 당첨 여부를 판정한다.
  * [ ] 입력받는 당첨 번호는 쉼표(,)로 분리되는 숫자의 나열이며 공백은 무시한다.
  * [ ] 숫자가 아닌 값이 입력되면 예외가 발생한다.
  * [ ] 1-45 범위에 속하지 않는 숫자가 있으면 예외가 발생한다. (중복)
  * [ ] 중복된 숫자가 있으면 예외가 발생한다. (중복)
  * [ ] 당첨 번호와 로또 일치 갯수에 따라 당첨금이 정해진다.
    * 6개가 일치하면 당첨금은 2,000,000,000원이다.
    * 5개가 일치하면 당첨금은 1,500,000원이다.
    * 4개가 일치하면 당첨금은 50,000원이다.
    * 3개가 일치하면 당첨금은 5,000원이다.
    * 3개 미만으로 일치하면 당첨금은 없다.
* 당첨 결과 판정 후 당첨 통계를 출력한다.
  * [ ] 각 일치 갯수에 따른 당첨 횟수를 누적으로 표기한다.
  * [ ] 수익률을 표기한다.
    * 수익률 = 수익 / 구매금액 (버림하여 소수점 둘째자리까지 표기)
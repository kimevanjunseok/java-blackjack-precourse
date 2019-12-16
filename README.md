# 우아한 테크코스 프리코스 3주차

> 블랙잭

## 기능 요구사항

- 블랙잭 게임을 진행하는 프로그램을 구현한다. 블랙잭 게임은 딜러와 플레이어 중 카드의 합이 21 또는 21에 가장 가까운 숫자를 가지는 쪽이 이기는 게임이다.
- 플레이어는 게임을 시작할 때 배팅 금액을 정해야 한다. 카드의 숫자 계산은 카드 숫자를 기본으로 하며, 예외로 Ace는 1 또는 11로 계산할 수 있으며, King, Queen, Jack은 각각 10으로 계산한다.
- 게임을 시작하면 플레이어는 두 장의 카드를 지급 받으며, 두 장의 카드 숫자를 합쳐 21을 초과하지 않으면서 21에 가깝게 만들면 이긴다. 21을 넘지 않을 경우 원한다면 얼마든지 카드를 계속 뽑을 수 있다. 단, 카드를 추가로 뽑아 21을 초과할 경우 배팅 금액을 모두 잃게 된다.
- 처음 두 장의 카드 합이 21일 경우 블랙잭이 되면 베팅 금액의 1.5배를 딜러에게 받는다. 딜러와 플레이어가 모두동시에 블랙잭인 경우 플레이어는 베팅한 금액을 돌려받는다.
- 딜러는 처음에 받은 2장의 합계가 16이하이면 반드시 1장의 카드를 추가로 받아야 하고, 17점 이상이면 추가로 받을 수 없다. 딜러가 21을 초과하면 그 시점까지 남아 있던 플레이어들은 가지고 있는 패에 상관 없이 승리해 베팅 금액을 받는다.

## 기능 구현

1. [  ] 참여할 사람의 이름을 입력받는 함수를 구현한다
   1. [X] 이름은 쉼표 기준으로 분리해야한다.
   2. [  ] 입력 예외처리를 해야한다.(빈 값일 경우)
2. [X] 각 이름별로 배팅할 수 있는 함수를 구현한다.
3. [X] 각 이름, 배팅 Player 클래스에 할당한다.
4. [X] 딜러, 참여자에게 카드를 지급하는 함수를 구현한다.
   1. [X] 모든 카드 종류를 가지고 온다.
   2. [X] Random 카드를 분배한다.
   3. [X] 분배한 카드인지 중복 확인한다.
   4. [X] 받은 카드를 보여준다.
   5. [X] 블랙잭이 있는지 확인한다.
5. [X] 카드의 합을 구하는 함수를 구현한다.
   1. [X] 참여자는 21이하면 카드를 뽑을 것인지 선택할 수 있다.
   2. [X] 딜러는 16이하면 카드를 뽑는다.
   3. [X] 딜러와 참여자 카드와 결과를 보여준다. 
6. [  ] 결과를 출력하는 함수를 구현한다.
   1. [X] 딜러와 참여자의 최종 점수 계산을 보여준다.
   2. [X] 딜러와 참여자의 수익을 계산한다.
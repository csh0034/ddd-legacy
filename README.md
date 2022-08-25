# 키친포스

## 퀵 스타트

```sh
cd docker
docker compose -p kitchenpos up -d
```

## 요구 사항

- 제품
  - [ ] 제품을 등록할 수 있어야 한다.
  - [ ] 제품 등록시 가격은 0보다 작을수 없다.
  - [ ] 등록된 제품의 가격을 변경 할 수 있어야 한다. 
    - [ ] 해당 제품이 포함된 메뉴중 하위 제품의 가격 총합이 메뉴 가격보다 작을 경우 메뉴를 숨김 처리한다.
  - [ ] 등록된 모든 제품을 조회 할 수 있어야 한다.
- 메뉴 그룹
  - [ ] 메뉴 그룹을 등록할 수 있어야 한다.
  - [ ] 메뉴 그룹 등록시 이름은 반드시 존재해야한다.
  - [ ] 등록된 모든 메뉴 그룹을 조회 할 수 있어야 한다.
- 메뉴
  - [ ] 메뉴는 반드시 메뉴 그룹에 속해야 한다.
  - [ ] 메뉴를 등록할 수 있어야 한다.
    - [ ] 반드시 하나 이상의 제품을 등록해야 한다.
    - [ ] 수량은 0개 이상이어야 한다.
  - [ ] 메뉴 가격을 변경할 수 있어야 한다.
    - [ ] 변경하려는 가격이 하위 제품 가격의 총합보다 클 경우 가격을 변경할 수 없다.
  - [ ] 메뉴를 표시할수 있어야 한다.
    - [ ] 메뉴 가격이 하위 제품 가격의 총합보다 클 경우 표시상태로 변경할 수 없다.
  - [ ] 메뉴를 숨김처리 할 수 있어야 한다.
  - [ ] 등록된 모든 메뉴를 조회 할 수 있어야 한다.
  - [ ] 메뉴에는 다수의 제품이 포함 될 수 있으며 0 개 이상의 수량을 등록 할 수 있어야 한다.
- 테이블
  - [ ] 테이블을 등록 할 수 있어야 한다.
  - [ ] 테이블에 앉을 경우 점유 상태로 변경 되어야한다.
  - [ ] 테이블을 치울때는 반드시 주문완료 상태여야 하며 테이블을 초기상태로 변경해야한다.
  - [ ] 테이블의 손님수를 변경할 수 있어야 한다.
    - [ ] 테이블이 점유 상태인 경우에만 가능해야 한다.
  - [ ] 등록된 모든 테이블을 조회 할 수 있어야한다.
- 주문
  - [ ] 주문의 경우 배달, 포장, 매장식사가 가능해야 한다.
  - [ ] 주문을 등록 할 수 있어야 한다.
    - [ ] 배달의 경우 배달주소를 입력 해야 한다. 
    - [ ] 매장식사의 경우 테이블이 점유상태가 아니여야한다.
    - [ ] 주문이 완료될 경우 주문대기 상태가 된다.
  - [ ] 주문수락 상태로 변경할 수 있어야 한다.
    - [ ] 주문대기 상태에서만 가능해야 한다.
    - [ ] 배달일 경우 라이더에게 배달요청을 해야한다.
  - [ ] 주문제공 상태로 변경할 수 있어야 한다.
    - [ ] 주문수락 상태에서만 가능해야 한다.
  - [ ] 배달중 상태로 변경할 수 있어야 한다.
    - [ ] 배달의 경우에만 가능해야 한다.
    - [ ] 주문제공 상태에만 가능해야 한다.
  - [ ] 배달완료 상태로 변경할 수 있어야 한다.
    - [ ] 배달중 상태에서만 가능해야 한다.
  - [ ] 주문완료 상태로 변경할 수 있어야 한다.
    - [ ] 배달일 경우 배달완료 상태에서만 가능해야 한다.
    - [ ] 포장, 매장식사의 경우 주문제공 상태에서만 가능 해야한다. 
    - [ ] 매장식사의 경우 테이블을 초기상태로 변경해야한다.
  - [ ] 등록된 모든 주문을 조회할 수 있어야 한다.

## 용어 사전

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
|  |  |  |

## 모델링

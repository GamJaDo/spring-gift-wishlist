# spring-gift-wishlist

---

# 1단계 - 유효성 검사 및 예외 처리
## 기능 요구 사항
### 상품으르 추가하거나 수정하는 경우, 클라이언트로부터 잘못된 값이 전달될 수 있다. 잘못된 값이 전달되면 클라이언트가 어떤 부분이 왜 잘못되었는지 인지할 수 있도록 응답을 제공한다.
* 상품 이름은 공백을 포함하여 최대 15자까지 입력할 수 있다.
* 특수 문자
    - 가능: (), [], +, -, &, /, _
    - 그 외 특수 문자 사용 불가
* "카카오"가 포함된 문구는 담당 MD와 협의한 경우에만 사용할 수 있다.

## 기능
* 생성/업데이트 시 제품 데이터 유효성 검사
    - 제품 이름은 최대 15자.
    - 특정 특수 문자 허용.
    - "카카오" 포함 금지(승인된 경우 제외).

--- 
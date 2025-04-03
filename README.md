## 프로젝트

## Getting Started

### Prerequisites

#### Running Docker Containers

`local` profile 로 실행하기 위하여 인프라가 설정되어 있는 Docker 컨테이너를 실행해주셔야 합니다.

```bash
docker-compose up -d
```

### SEQUENCE  
#### 잔액  
<img src="https://github.com/user-attachments/assets/20ca6a68-1d38-43e5-a6a1-5060f1933126" width="450" />  


#### 쿠폰  
<img src="https://github.com/user-attachments/assets/dcd3c1c4-3075-4213-b8dc-99bd8cd7eceb" width="500" />  


#### 쿠폰을 사용한 주문
<img src="https://github.com/user-attachments/assets/7f2e74ba-7d0d-4217-a715-dbc7434c9e1d" width="700" />  


### ERD  
![e-commerce erd](https://github.com/user-attachments/assets/3046d8a6-dff4-4e48-b401-4badfd13bc5c)   


### API 명세
#### 잔액  
- 잔액 조회
  /api/v0/balance [GET]
- 잔액 충전
  /api/v0/balance/charge [POST]  
  
#### 상품  
- 상품 상세 조회
  /api/v0/products/{productId} [GET]
- 상위 상품 조회
  /api/v0/products/top-selling [GET]  
  
#### 주문  
- 주문 조회
  /api/v0/orders/{orderId} [GET]  
- 주문 생성
  /api/v0/orders [POST]  
  
#### 결제  
- 결제 생성
  /api/v0/payments [POST]
  
#### 선착순 쿠폰  
- 쿠폰 조회
  /api/v0/coupons [GET]  
- 쿠폰 발급
  /api/v0/coupons [POST]  

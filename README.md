---  
# 1. 상품카테고리 테이블 설계  
### 테이블 명칭 : category   

컬럼명| 데이터타입        | 기본값 | 생략가능     |설명
---|--------------|-----|----------|---|   
id | Number(9)    |     | NOT NULL | 상품 카테고리 ID  
id_parent | Number(9)    |     | NOT NULL |  부모 상품 카테고리  
name | varchar(256) |     | NOT NULL |  카테고리 명칭  
created_timestamp | Date         | CURRENT_TIMESTAMP | NOT NULL |  카테고리 생성일  
update_timestamp | Date         |     |   |  카테고리 수정일  
---
# 2. 기능
1. 카테고리 등록/수정/삭제 APi
2. 카테고리 조회 API
 * 상위 카테고리를 이용해서 하위 카테고리 조회가능
 * 상위 카테고리 지정하지 않을시 전체 카테고리 반환

# 3. 설치 및 실행방법
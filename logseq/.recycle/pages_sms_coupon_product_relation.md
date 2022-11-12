- #schema #cms #mall-learning #营销模块数据库表解析（二）
  id:: 636f356b-3757-48e2-a266-abe83f4e0702
-
- ```
  create table sms_coupon_product_relation
  (
     id                   bigint not null auto_increment,
     coupon_id            bigint comment '优惠券id',
     product_id           bigint comment '商品id',
     product_name         varchar(500) comment '商品名称',
     product_sn           varchar(200) comment '商品条码',
     primary key (id)
  );
  
  ```
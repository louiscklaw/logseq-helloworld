- #schema #cms #mall-learning #商品模块数据库表解析
-
- ```
  create table pms_product_ladder
  (
     id                   bigint not null auto_increment,
     product_id           bigint comment '商品id',
     count                int comment '满足的商品数量',
     discount             decimal(10,2) comment '折扣',
     price                decimal(10,2) comment '折后价格',
     primary key (id)
  );
  
  ```
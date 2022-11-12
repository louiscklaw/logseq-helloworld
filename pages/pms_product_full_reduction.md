- #schema #cms #mall-learning #商品模块数据库表解析
-
- ```
  create table pms_member_price
  (
     id                   bigint not null auto_increment,
     product_id           bigint comment '商品id',
     member_level_id      bigint comment '会员等级id',
     member_price         decimal(10,2) comment '会员价格',
     member_level_name    varchar(100) comment '会员等级名称',
     primary key (id)
  );
  
  ```
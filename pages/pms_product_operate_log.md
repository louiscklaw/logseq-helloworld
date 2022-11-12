- #schema #cms #mall-learning #商品模块数据库表解析
-
- ```
  create table pms_product_operate_log
  (
     id                   bigint not null auto_increment,
     product_id           bigint comment '商品id',
     price_old            decimal(10,2) comment '改变前价格',
     price_new            decimal(10,2) comment '改变后价格',
     sale_price_old       decimal(10,2) comment '改变前优惠价',
     sale_price_new       decimal(10,2) comment '改变后优惠价',
     gift_point_old       int comment '改变前积分',
     gift_point_new       int comment '改变后积分',
     use_point_limit_old  int comment '改变前积分使用限制',
     use_point_limit_new  int comment '改变后积分使用限制',
     operate_man          varchar(64) comment '操作人',
     create_time          datetime comment '创建时间',
     primary key (id)
  );
  ```
-
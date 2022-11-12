- #schema #cms #mall-learning #订单模块数据库表解析（一）
-
- > 订单中包含的商品信息，一个订单中会有多个订单商品信息。
-
- ```sql
  create table oms_order_item
  (
     id                   bigint not null auto_increment,
     order_id             bigint comment '订单id',
     order_sn             varchar(64) comment '订单编号',
     product_id           bigint comment '商品id',
     product_pic          varchar(500) comment '商品图片',
     product_name         varchar(200) comment '商品名称',
     product_brand        varchar(200) comment '商品品牌',
     product_sn           varchar(64) comment '商品条码',
     product_price        decimal(10,2) comment '销售价格',
     product_quantity     int comment '购买数量',
     product_sku_id       bigint comment '商品sku编号',
     product_sku_code     varchar(50) comment '商品sku条码',
     product_category_id  bigint comment '商品分类id',
     sp1                  varchar(100) comment '商品的销售属性1',
     sp2                  varchar(100) comment '商品的销售属性2',
     sp3                  varchar(100) comment '商品的销售属性3',
     promotion_name       varchar(200) comment '商品促销名称',
     promotion_amount     decimal(10,2) comment '商品促销分解金额',
     coupon_amount        decimal(10,2) comment '优惠券优惠分解金额',
     integration_amount   decimal(10,2) comment '积分优惠分解金额',
     real_amount          decimal(10,2) comment '该商品经过优惠后的分解金额',
     gift_integration     int not null default 0 comment '商品赠送积分',
     gift_growth          int not null default 0 comment '商品赠送成长值',
     product_attr         varchar(500) comment '商品销售属性:[{"key":"颜色","value":"颜色"},{"key":"容量","value":"4G"}]',
     primary key (id)
  );
  ```
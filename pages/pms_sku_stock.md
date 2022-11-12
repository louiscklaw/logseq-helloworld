- #schema #cms #mall-learning #商品模块数据库表解析
-
- comment:
	- SKU(Stock K[]()eeping Unit)是指库存量单位
	- SPU(Standard Product Unit)是指标准产品单位。
	- 举个例子：iphone xs是一个SPU，而iphone xs 公开版 64G 银色是一个SKU。
-
- ```
  create table pms_sku_stock
  (
     id                   bigint not null auto_increment,
     product_id           bigint comment '商品id',
     sku_code             varchar(64) not null comment 'sku编码',
     price                decimal(10,2) comment '价格',
     stock                int default 0 comment '库存',
     low_stock            int comment '预警库存',
     sp1                  varchar(64) comment '规格属性1',
     sp2                  varchar(64) comment '规格属性2',
     sp3                  varchar(64) comment '规格属性3',
     pic                  varchar(255) comment '展示图片',
     sale                 int comment '销量',
     promotion_price      decimal(10,2) comment '单品促销价格',
     lock_stock           int default 0 comment '锁定库存',
     primary key (id)
  );
  
  ```
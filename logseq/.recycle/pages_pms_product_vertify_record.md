- #schema #cms #mall-learning #商品模块数据库表解析
  id:: 636f34bc-2b32-41aa-aa62-9be0225bee16
-
- ```
  create table pms_product_vertify_record
  (
     id                   bigint not null auto_increment,
     product_id           bigint comment '商品id',
     create_time          datetime comment '创建时间',
     vertify_man          varchar(64) comment '审核人',
     status               int(1) comment '审核后的状态：0->未通过；2->已通过',
     detail               varchar(255) comment '反馈详情',
     primary key (id)
  );
  
  ```
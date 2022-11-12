- #schema #cms #mall-learning #商品模块数据库表解析
-
- ```
  create table pms_product_category_attribute_relation
  (
     id                   bigint not null auto_increment,
     product_category_id  bigint comment '商品分类id',
     product_attribute_id bigint comment '商品属性id',
     primary key (id)
  );
  ```
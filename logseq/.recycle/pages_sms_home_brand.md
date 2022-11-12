- #schema #cms #mall-learning #营销模块数据库表解析（三）
-
- ```
  create table sms_home_brand
  (
     id                   bigint not null auto_increment,
     brand_id             bigint comment '商品品牌id',
     brand_name           varchar(64) comment '商品品牌名称',
     recommend_status     int(1) comment '推荐状态：0->不推荐;1->推荐',
     sort                 int comment '排序',
     primary key (id)
  );
  ```
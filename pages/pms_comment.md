- #schema #cms #mall-learning #商品模块数据库表解析
-
- ```
  create table pms_comment
  (
     id                   bigint not null auto_increment,
     product_id           bigint comment '商品id',
     member_nick_name     varchar(255) comment '会员昵称',
     product_name         varchar(255) comment '商品名称',
     star                 int(3) comment '评价星数：0->5',
     member_ip            varchar(64) comment '评价的ip',
     create_time          datetime comment '创建时间',
     show_status          int(1) comment '是否显示',
     product_attribute    varchar(255) comment '购买时的商品属性',
     collect_couont       int comment '收藏数',
     read_count           int comment '阅读数',
     content              text comment '内容',
     pics                 varchar(1000) comment '上传图片地址，以逗号隔开',
     member_icon          varchar(255) comment '评论用户头像',
     replay_count         int comment '回复数',
     primary key (id)
  );
  
  ```
-
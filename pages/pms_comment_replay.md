- #schema #cms #mall-learning #商品模块数据库表解析
-
- ```
  create table pms_comment_replay
  (
     id                   bigint not null auto_increment,
     comment_id           bigint comment '评论id',
     member_nick_name     varchar(255) comment '会员昵称',
     member_icon          varchar(255) comment '会员头像',
     content              varchar(1000) comment '内容',
     create_time          datetime comment '创建时间',
     type                 int(1) comment '评论人员类型；0->会员；1->管理员',
     primary key (id)
  );
  
  ```
-
- ![](https://github.com/macrozheng/mall-learning/raw/master/docs/images/database_screen_30.png)
-
- ![](https://github.com/macrozheng/mall-learning/raw/master/docs/images/database_screen_31.png)
-
- ![](https://github.com/macrozheng/mall-learning/raw/master/docs/images/database_screen_32.png)
-
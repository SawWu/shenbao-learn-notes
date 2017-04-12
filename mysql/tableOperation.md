
# 表操作

插入
insert [into] 表名 [(列名1, 列名2, 列名3, ...)] values (值1, 值2, 值3, ...);

    insert into students values(NULL, "王刚", "男", 20, "13811371377");
    insert into students (name, sex, age) values("孙丽华", "女", 21);


查询
select 列名称 from 表名称 [查询条件];
=、>、<、>=、<、!= 以及一些扩展运算符 is [not] null、in、like 等。 还可以对查询条件使用 or 和 and 进行组合查询

    select * from students where age > 21;
    select * from students where name like "%王%";
    select * from students where id<5 and age>20;


更新
update 表名称 set 列名称=新值 where 更新条件;

    update students set name="张伟鹏", age=19 where id=1;

删除
delete from 表名称 where 删除条件;

    delete from students;
    delete from students where id=2;
    delete from students where age<20;







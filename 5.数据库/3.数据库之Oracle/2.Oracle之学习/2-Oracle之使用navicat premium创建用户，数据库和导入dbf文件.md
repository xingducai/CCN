总操作流程：
- 1、创建用户
- 2、创建数据库
- 3、连接数据库
- 4、导入表

***

# 创建用户

```sql
create user SSM identified by "DKLi123456";

grant  connect,resource,dba,create session,create any table,select any dictionary to SSM;

alter user SSM account unlock;
```

- 测试

![](image/2-1.png)


# 创建数据库

![](image/2-2.png)

![](image/2-3.png)

![](image/2-4.png)

![](image/2-5.png)

# 连接数据库

![](image/2-6.png)

![](image/2-7.png)


# 导入表

![](image/2-8.png)

![](image/2-9.png)
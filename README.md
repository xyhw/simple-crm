# Simple CRM

## 简介

不懂CRM，没有关系，你只要会做业务，就会用Simple CRM。
没有什么难以理解的概念，不需要更多的文化和知识，适合中小微企业。
从寻找客户，联系客户，管理客户，最后达到成交，以及维持关系。都是你熟悉的事情。

## 功能

### 用户

1. 用户列表 O
2. 用户的添加、编辑和删除 O
3. 用户的登录 O
4. 用户的基本信息修改 O
5. 用户的密码修改 O
6. 用户的锁定和解锁 O


### 客户

1. 客户列表 O
2. 客户明细 O
3. 客户地图展示 
4. 客户上传、删除图片 O
5. 转交客户 O
6. 退回客户 O
7. 对客户添加联系 O
8. 修改联系
9. 删除联系
10. 数据获取 G和B （O）
11. 客户标签

### 收益

1. 客户收益创建
2. 客户收益编辑
3. 客户收益删除
4. 收益统计
5. 收益预测

### 配置

1. 联系类型的创建、编辑和删除
2. 客户阶段的创建、编辑和删除
3. 客户标签的创建、编辑和删除


## 运行

修改.env.example为.env，并且填入两个地图对应的的API调用KEY，是服务端KEY，这个可以到对应的地图开发者页面免费申请。

## Docker

docker build --pull --rm -f "Dockerfile" -t simple-crm:latest "server"

docker run --rm -d  -p 5700:5700/tcp simple-crm:latest
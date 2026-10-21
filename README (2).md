```
# 图书情报检索与统计平台
数据管理系统实训项目 | MongoDB + PyMongo

## 一、项目概述
本项目为高校图书馆图书情报检索与统计平台，基于MongoDB文档数据库，实现图书、读者、借阅流水管理，提供检索、统计、权限管理功能，使用PyMongo开发命令行程序。

### 业务功能清单
- ✅ MongoDB服务部署，自定义数据目录
- ✅ 普通集合、固定集合、时间序列集合、视图建模
- ✅ 精确检索、范围检索、多条件组合检索、排序投影
- ✅ 聚合管道：分类统计、借阅趋势、热门排行、跨表关联
- ✅ 索引优化、只读/读写账号权限控制
- ✅ PyMongo模块化菜单程序开发
- ✅ Compass图形化验收与数据导出

## 二、实验环境
- 操作系统：Windows11
- 数据库：MongoDB Community 端口27017
- 可视化：MongoDB Compass
- 开发：Python3.10 + PyCharm + pymongo
- 数据库名：`library`
- 集合：books、readers、borrow_logs、category_stats
- 特殊集合：book_logs（固定集合）、borrow_logs（时序集合）、book_in_stock（视图）

## 三、项目文件清单
```

├─ mongodb_connect.py   # 数据库连接模块
├─ book_manager.py      # 图书管理模块
├─ reader_manager.py    # 读者管理模块
├─ borrow_manager.py    # 借阅流水模块
├─ stat_manager.py      # 统计聚合模块
├─ main.py              # 主菜单程序
├─ books.txt、readers.txt、borrow_logs.txt  # 原始数据集
├─ books.json、category_stats.json          # 导出成果

```

## 四、实验总结
本次实训围绕MongoDB文档数据库完成图书情报检索统计平台开发，依次完成数据库部署、数据建模、多类型查询、聚合统计、索引优化、权限配置与PyMongo程序开发。
项目中使用了固定集合、时间序列集合、视图等MongoDB特色结构，理解了时序数据存储方案；通过聚合管道实现多维度统计报表；建立索引优化高频查询，区分只读、读写账号实现访问控制。
开发模块化Python命令行程序，把数据库操作封装为独立模块，代码结构清晰。同时使用MongoDB Compass完成图形化校验，对比命令行结果，保证数据一致。
过程中遇到时序集合参数配置、数据库连接泄漏等问题，调试后掌握了排错思路。本次实训掌握了NoSQL数据库的开发流程，为后续非关系型数据库开发打下基础。

## 五、项目访问
本项目基于GitHub Pages部署，在线展示地址：
https://9d9m.github.io/图书馆/
```
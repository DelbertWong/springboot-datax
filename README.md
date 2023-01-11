![Java](https://woolson.gitee.io/npmer-badge/Java-555555-1.8-44cc11-check-ffffff-square-gradient-shadow.svg)
![springboot](https://woolson.gitee.io/npmer-badge/springboot-555555-2.x-44cc11-check-ffffff-square-gradient-shadow.svg)
## preparation
- Language: Java 8
- Environment: MacOS, 16G RAM
- Database: Mysql5.7
- 建议Python2.7


## todo list

* [x] springboot重构项目
* [x] 集成swagger，方便调试
* [x] 集成mybatis plus和Mysql数据库存放应用数据
* [x] 网页端修改并持久化job配置的json到数据库
* [x] 网页端实时查看抽取日志，类似Jenkins的日志控制台输出功能
* [x] 实时查看抽取日志BUG功能修复
* [ ] 网页端各种读写插件模板生成，可以在页面组装使用
* [ ] 实现datax分布式作业
* [ ] 实现部分写插件支持自动建表功能
* [ ] 实现定时任务来调度抽取作业

## 前端项目
源码在 `datax-vue-admin-ui` 目录
## how to run
### 1. 下载datax打包之后的文件或者github拉取datax代码打包，配置环境变量
```
 DATAX_HOME=G:\learndemo\springboot-datax\datax\bin
```

### 2. 执行datax-web/db下面的sql文件并修改application.yml数据库配置信息

### 3. application.yml配置数据抽取日志文件保存路径
                          
```
etlLogDir: D:\temp\logs\datax-web\
```

### 4. idea启动 datax-admin

### 5. 启动成功后打开页面
http://localhost:8080/index.html#/datax/job
![](https://github.com/WeiYe-Jing/datax-web/blob/master/doc/img/20191119100901.png)

### 6. 点击作业配置，创建作业
![](https://github.com/WeiYe-Jing/datax-web/blob/master/doc/img/20191119101258.png)

### 7. 完成创建作业之后，点击同步任务，选择任务，点击启动
![](https://github.com/WeiYe-Jing/datax-web/blob/master/doc/img/20191119101431.png)

### 8. 可以点击查看日志，实时获取日志信息
![](https://github.com/WeiYe-Jing/datax-web/blob/master/doc/img/20191119102551.png)

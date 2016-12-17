RAPv0.14.1 Docker 自动化部署
-----------
RAP是一个可视化接口管理工具 通过分析接口结构，动态生成模拟数据，校验真实接口正确性， 围绕接口定义，通过一系列自动化工具提升我们的协作效率。我们的口号：提高效率，回家吃晚饭！

拆分redis mysql rap 部署到不同容器中

## 启动方法

1. 下载安装docker和docker-compose

2. clone工程
```
git clone https://github.com/denonzhu/RAP.git
```

3. 进入build-web,执行命令

```
docker build -t rap-web .
```

4.进入根目录,执行命令
```
docker-compose up -d
```

5.自定义配置
config.properties是配置文件，如果修改mysql密码，请相应修改根目录docker-compose.yml中的密码，重新编译

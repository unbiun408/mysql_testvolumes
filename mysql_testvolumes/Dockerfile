# 使用官方 MySQL 镜像作为基础镜像
FROM mysql:8.0

# 设置环境变量
ENV MYSQL_ROOT_PASSWORD=root_password
ENV MYSQL_DATABASE=my_database
ENV MYSQL_USER=my_user
ENV MYSQL_PASSWORD=my_password

# 复制初始化脚本到容器中
COPY ./init.sql /docker-entrypoint-initdb.d/

# 暴露 MySQL 端口
EXPOSE 3306

# 启动 MySQL 服务
CMD ["mysqld"]

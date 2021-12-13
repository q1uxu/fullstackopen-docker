# [FullStackOpen-Docker](https://fullstackopen.com/zh/part12)

## 介绍

这是一个简单的todo app，使用React.js、Express.js、Nginx，MongoDB和Redis开发，通过Docker把这几个项目串联起来


## 运行方法

1. 安装[Docker](https://www.docker.com/)
2. git clone本项目
3. 进入/todo-app目录，输入 `docker-compose up` 启动生产环境，或者输入`docker-compose -f docker-compose.dev.yml up`启动开发环境
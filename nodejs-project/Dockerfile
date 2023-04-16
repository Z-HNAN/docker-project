# 基础镜像
FROM node:16-buster-slim
# FROM node:16-alpine

# 安装 pnmp 等工具
RUN npm install -g pnpm && \
    npm install -g typescript && \
    npm install -g ts-node

# 设置全局的.npmrc文件
RUN echo "registry=https://registry.npm.taobao.org/" > /root/.npmrc

# 创建一个工作目录
WORKDIR /app

# 定义挂载卷
VOLUME /root/.pnpm-store
VOLUME /app/project0
VOLUME /app/project1
VOLUME /app/project2
VOLUME /app/project3
VOLUME /app/project4
VOLUME /app/project5
VOLUME /app/project6
VOLUME /app/project7
VOLUME /app/project8
VOLUME /app/project9

# 设置环境变量
ENV NODE_ENV=production

# 保持容器一直运行
ENTRYPOINT ["/bin/sh", "-c"]
CMD ["tail", "-f", "/dev/null"]

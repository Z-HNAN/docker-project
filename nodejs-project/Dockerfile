# 基础镜像
FROM --platform=$BUILDPLATFORM node:16-alpine

# 安装 pnmp 等工具
RUN npm install -g pnpm && \
    pnpm install -g typescript && \
    pnpm install -g ts-node

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

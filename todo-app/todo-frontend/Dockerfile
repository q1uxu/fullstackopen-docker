# 测试
FROM node:16 AS test-stage

WORKDIR /usr/src/app

COPY . .

ENV CI=true

RUN npm ci

RUN npm run test

# 构建
FROM node:16 AS build-stage

WORKDIR /usr/src/app

COPY --from=test-stage /usr/src/app /usr/src/app

RUN npm run build

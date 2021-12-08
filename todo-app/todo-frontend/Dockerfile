# 构建
FROM node:16 AS build-stage

WORKDIR /src/usr/app

COPY . .

ENV REACT_APP_BACKEND_URL=//localhost:12600

RUN npm ci

RUN npm run build

# 运行
FROM nginx

COPY --from=build-stage /src/usr/app/build /usr/share/nginx/html

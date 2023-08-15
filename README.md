# 使用 docker 搭建 graphite+grafana 的 apm 平台

1. 安装 docker www.docker.com

2. compose

```
docker-compose up
# 后台启动
docker-compose up -d
```

3. localhost:3000 登录

4. 默认密码 admin admin a121144

5. 左侧导航 add Datasource => graphite

6. URL => http://graphite-statsd

7. 点击 SAVE&TEST

8. 启动 node 应用，使用 express-statsd 打点上报

9. 在 panel 的 query 中可以查看 http 数据了

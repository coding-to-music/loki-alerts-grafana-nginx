# loki-alerts-grafana-nginx

# 🚀 Alerting with Loki v2 on Docker Example 🚀

https://github.com/coding-to-music/loki-alerts-grafana-nginx

From / By Ruan Bekker https://github.com/ruanbekker/loki-alerts-docker

https://github.com/ruanbekker/loki-alerts-docker

https://blog.ruanbekker.com/blog/2020/11/06/how-to-setup-alerting-with-loki/

## Environment variables:

```java

```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/loki-alerts-grafana-nginx.git
git push -u origin main
```

## Results:

Grafana http://localhost:3000

loki http://localhost:3100

alertmanager http://localhost:9093

nginx Webserver http://localhost:80

http-client calls nginx Webserver constantly

# loki-alerts-docker

Alerting with Loki v2 on Docker Example

## Usage

Dependency is to install the loki docker driver:

```
docker plugin install grafana/loki-docker-driver:latest --alias loki --grant-all-permissions
```

Replace your config:

```
SLACK_WEBHOOK_URL="https://hooks.slack.com/services/xx/xx/xx" SLACK_CHANNEL="#notifications" ./parse_configs.sh
```

Boot the stack:

```
docker-compose up -d
```

Then follow the [blogpost](https://blog.ruanbekker.com/blog/2020/11/06/how-to-setup-alerting-with-loki/):

- https://blog.ruanbekker.com/blog/2020/11/06/how-to-setup-alerting-with-loki/

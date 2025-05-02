<div align="center">
<img src="./public/favicon.svg" alt="预览"/>

<h1 align="center">简约风格的网址导航页</h1>

[演示环境](https://www.luode.vip) 

![Snipaste_2023-05-08_09-15-08](public/png/QQ截图20231019212432.png)

</div>

# 启动

## 安装依赖
```bash
npm install -g pnpm
pnpm install
```

## 启动项目
```bash
npm run dev
```

# docker容器

## latest 版本

```shell
docker pull luode0320/web-start:latest
```

启动:

```shell
docker run -d \
--restart=always \
--name web  \
-p 2000:2000 \
luode0320/web-start:latest
```

挂载配置(要先准备好配置文件):
```shell
docker run -d \
--restart=always \
--name web  \
-p 2000:2000 \
-v /usr/local/src/web/preset.json:/app/src/preset.json
luode0320/web-start:latest
```

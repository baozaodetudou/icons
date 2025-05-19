### `README.md`

````markdown
# Icons Pack 服务

该项目使用 Docker 部署一个图标打包服务，容器镜像为 `verky/icon-pack:latest`。

---

## 🚀 快速开始

### 1. 克隆项目
```bash
git clone <仓库地址>
cd icons
````

### 2. 启动服务

使用 Docker Compose 启动服务：

```bash
docker-compose up -d
```

### 3. 验证服务是否启动

```bash
docker-compose ps
```

服务启动后，访问：

```
http://localhost:5000
```

---

## 📂 目录结构

```
.
├── docker-compose.yml   # Docker Compose 配置文件
├── icons                # 图标文件夹（映射至容器）
└── README.md            # 使用说明
```

---

## ⚙️ 配置说明

### 环境变量

| 变量名        | 说明   | 默认值   |
| ---------- | ---- | ----- |
| SITE\_NAME | 服务名称 | icons |

### 端口映射

| 宿主机端口 | 容器端口 |
| ----- | ---- |
| 5000  | 5000 |

### 挂载目录

| 宿主机路径   | 容器路径        |
| ------- | ----------- |
| ./icons | /app/images |

---

## 🛠️ 常用命令

### 查看日志

```bash
docker-compose logs -f
```

### 停止服务

```bash
docker-compose down
```

### 更新服务

1. 拉取最新镜像

   ```bash
   docker pull verky/icon-pack:latest
   ```
2. 重启服务

   ```bash
   docker-compose up -d
   ```

---

## 📌 注意事项

1. 确保宿主机的 `./icons` 目录存在且有读写权限。
2. 更新镜像时，请先停止容器再启动，以确保更新生效。

---

## 💬 联系方式

如有问题或建议，请联系开发者。

```

---

这个 `README.md` 文件详细说明了项目的安装、使用和常见操作。如果需要进一步调整或添加其他信息，请告诉我！😊
```

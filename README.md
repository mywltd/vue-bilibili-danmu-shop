# vue-bilibili-danmu-shop

> 由 **魅影** 维护（[www.vuphub.fun](https://www.vuphub.fun)）。基于原作者 **苏青安 / 何俊杰** 的作品进行二次修改，遵循 MIT 协议，保留原作版权信息，详见 [LICENSE](LICENSE)。

⚠️ 本项目仅供学习交流使用，禁止用于商业或非法用途。

​`vue-bilibili-danmu-shop`​ 是一个基于 Vue 3 和 Vite 构建的前端项目，用于配合 [php-bilibili-danmu](https://github.com/mywltd/php-bilibili-danmu) 项目的积分商城模块。该前端页面为用户提供商品浏览与积分兑换等交互功能，依赖后端提供的 API 实现积分管理和订单处理等服务。

> 如果你选择通过 Docker 一键部署整套系统，则无需关注该前端仓库，部署过程将自动完成。

## 项目特点

- **前后端分离架构**：前端基于 Vue 3 构建，后端使用 PHP 提供 RESTful API 接口。
- **实时积分管理**：用户在直播间互动（如发送弹幕、开通大航海）可获得积分。
- **积分商城兑换**：用户可使用积分兑换商城内的虚拟或实物商品。

## 预览

| <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo01.png"> | <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo02.png"> | <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo03.png"> |
| --- | --- | --- |
| <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo04.png"> | <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo05.png"> | <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo06.png"> |
| <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo07.png"> | <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo08.png"> | <img src="https://raw.githubusercontent.com/mywltd/vue-bilibili-danmu-shop/main/src/assets/preview/demo09.png"> |



## 安装与运行

### 1. 克隆项目

```bash
git clone https://github.com/mywltd/vue-bilibili-danmu-shop.git
cd vue-bilibili-danmu-shop
```

### 2. 安装 Node.js

请前往 Node.js 官网下载安装适合你操作系统的版本：

👉 [https://nodejs.org/zh-cn](https://nodejs.org/zh-cn)

建议使用长期支持（LTS）版本。

### 3. 配置环境变量

复制 `.env.example`​ 为 `.env`​：

```bash
cp .env.example .env
```

根据你的部署情况，填写后端 API 地址、密钥等参数。相关信息可在机器人控制台的系统配置中查看。

### 4. 安装依赖并构建项目

```bash
npm install
npm run build
```

构建完成后，静态文件将生成于 `dist/`​ 目录中，可部署至任意静态资源服务器（如 Nginx、Vercel 等）。

### 下载预构建包

- **Actions 产物**：仓库 Actions → 选择成功的 `Build Dist` → Artifacts 下载 `vue-bilibili-danmu-shop-dist*.zip`（保留 30 天）
- **Release 产物**：打 `v*` 标签后，在 Releases 页面下载同名 zip（长期可下）

手动触发：Actions → Build Dist → Run workflow，可填写后端 API 地址。

也可在仓库 Variables 配置默认值：

| Variable | 说明 |
|----------|------|
| `VITE_API_URL` | 后端 API 地址 |
| `VITE_APP_NAME` | 商城名称 |

---

## 🧩 配套项目

[![Core](https://img.shields.io/badge/php--bilibili--danmu--core-B站交互核心模块-blueviolet?style=for-the-badge&logo=php)](https://github.com/mywltd/php-bilibili-danmu-core)
[![Docker](https://img.shields.io/badge/php--bilibili--danmu--docker-Docker一键部署容器-2496ed?style=for-the-badge&logo=docker)](https://github.com/mywltd/php-bilibili-danmu-docker)
[![API](https://img.shields.io/badge/php--bilibili--danmu-项目本体-007acc?style=for-the-badge&logo=php)](https://github.com/mywltd/php-bilibili-danmu)
[![Admin](https://img.shields.io/badge/vue--bilibili--danmu--admin-前端：管理后台-42b883?style=for-the-badge&logo=vue.js)](https://github.com/mywltd/vue-bilibili-danmu-admin)
[![Shop](https://img.shields.io/badge/vue--bilibili--danmu--shop-前端：移动端积分商城-3eaf7c?style=for-the-badge&logo=vue.js)](https://github.com/mywltd/vue-bilibili-danmu-shop)

## 致谢与版权

- 原作者：[苏青安 / 何俊杰](https://github.com/zxc7563598)
- 原仓库：[zxc7563598/vue-bilibili-danmu-shop](https://github.com/zxc7563598/vue-bilibili-danmu-shop)
- 本仓库：由 **魅影** 维护，基于原作二次修改（MIT）
- 个人网站：[www.vuphub.fun](https://www.vuphub.fun)

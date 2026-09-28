[简体中文](README.md) | [English](README.en.md)

# seal-d2-admin

> seal（海豹）项目四期重构前端模板，基于 [D2Admin](https://github.com/d2-projects/d2-admin-start-kit) 1.7.2（Element UI）二次开发，后端为 [seal](https://github.com/hequan2017/seal)。

## 项目介绍

seal-d2-admin 使用 D2Admin 快速开发框架替换 seal 原 iview-admin 版前端。目前已接入 seal 后端的登录认证（`/api/token`）与用户信息接口（`/system/api/user_info`），其余业务页面可基于 D2Admin 模板继续扩展，适合想用 Vue + Element UI 技术栈为 seal 开发前端的开发者参考。

## ✨ 功能特性

- 登录认证：`AccountLogin` 对接后端 `/api/token` 获取 Token，`AccountLoginInfo` 获取用户信息
- D2Admin 完整框架能力：多标签页、侧边栏菜单、菜单搜索（快捷键 s）、主题切换、国际化（简体中文/英文）、页面缓存等
- 内置演示页面 page1 / page2 / page3、前端日志收集页、404 页面
- 支持 Mock 数据与 No Mock 构建（`npm run build:nomock`），提供开发/部署多环境 `.env` 配置
- Travis CI 自动构建，并通过 qshell 上传七牛云 CDN

## 🛠 技术栈

- Vue 2.6 + Vue Router + Vuex，vue-cli 3 构建
- UI：Element UI 2.11（D2Admin 1.7.2 模板）
- axios 0.18、mockjs、lowdb、dayjs

## 🚀 快速开始

```bash
# 安装依赖
npm install

# 本地开发
npm run dev

# 生产构建
npm run build

# No Mock 构建
npm run build:nomock
```

- 网络请求公共地址通过 `.env` 中的 `VUE_APP_API` 配置（默认 `/api/`）
- 页面标题前缀 `VUE_APP_TITLE`、国际化语言 `VUE_APP_I18N_LOCALE` 等均在 `.env` 中配置
- 使用前需先部署好后端 [seal](https://github.com/hequan2017/seal)

## 🔗 相关项目

- 后端：[seal](https://github.com/hequan2017/seal)
- iview-admin 版前端：[seal-vue](https://github.com/hequan2017/seal-vue)
- D2Admin 文档：<https://fairyever.com/d2-admin/doc/zh/learn-guide/>

## 📄 许可证

[MIT](LICENSE)

## 作者

> 何全

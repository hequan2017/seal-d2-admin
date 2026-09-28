[简体中文](README.md) | [English](README.en.md)

# seal-d2-admin

> The phase-4 front-end template of the seal project, rebuilt on [D2Admin](https://github.com/d2-projects/d2-admin-start-kit) 1.7.2 (Element UI), working with the [seal](https://github.com/hequan2017/seal) back-end.

## Introduction

seal-d2-admin replaces the original iview-admin-based front-end of seal with the D2Admin rapid-development framework. It is already wired to the seal back-end for login (`/api/token`) and user info (`/system/api/user_info`); further business pages can be built on top of the D2Admin template. It is a useful reference for developing a Vue + Element UI front-end for seal.

## ✨ Features

- Login: `AccountLogin` obtains a token from the back-end `/api/token` endpoint, `AccountLoginInfo` fetches user info
- Full D2Admin framework capabilities: multi-tab pages, sidebar menus, menu search (hotkey s), theme switching, i18n (Simplified Chinese / English), page caching, etc.
- Built-in demo pages page1 / page2 / page3, a front-end log collection page and a 404 page
- Supports both mock data and No-Mock builds (`npm run build:nomock`), with multi-environment `.env` configuration
- Travis CI build, published to the Qiniu CDN via qshell

## 🛠 Tech Stack

- Vue 2.6 + Vue Router + Vuex, built with vue-cli 3
- UI: Element UI 2.11 (D2Admin 1.7.2 template)
- axios 0.18, mockjs, lowdb, dayjs

## 🚀 Quick Start

```bash
# Install dependencies
npm install

# Develop locally
npm run dev

# Production build
npm run build

# No-Mock build
npm run build:nomock
```

- The base API address is configured via `VUE_APP_API` in `.env` (default `/api/`)
- The page title prefix `VUE_APP_TITLE`, i18n locale `VUE_APP_I18N_LOCALE`, etc. are configured in `.env`
- Deploy the [seal](https://github.com/hequan2017/seal) back-end first

## 🔗 Related Projects

- Back-end: [seal](https://github.com/hequan2017/seal)
- iview-admin-based front-end: [seal-vue](https://github.com/hequan2017/seal-vue)
- D2Admin docs: <https://fairyever.com/d2-admin/doc/zh/learn-guide/>

## 📄 License

[MIT](LICENSE)

## Author

> He Quan (何全)

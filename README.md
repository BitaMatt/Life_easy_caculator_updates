# 生計易公開更新 / Life Easy Public Updates

這個倉庫只用於公開發布「生計易」的可下載版本、Web 靜態站點與更新清單。

This repository only hosts public Life Easy release artifacts, the Web build, and the public update manifest.

## 公開內容 / Public content

- `latest.json`：App 使用的最新穩定版更新清單 / latest stable update manifest used by the app.
- `docs/`：Web 正式版靜態檔案 / production Web static files.
- GitHub Releases：Android APK、Web 壓縮包及中英雙語更新日誌 / Android APK, Web archive, and bilingual release notes.

## 安全 / Security

本倉庫**不得**存放 API Key、Access Token、Android 簽名私鑰、密碼、帳號憑證或任何私人資料。

This repository **must never** contain API keys, access tokens, Android signing keys, passwords, account credentials, or private user data.

Android APK 的 SHA-256 會寫入 `latest.json`；Android 正式更新同時依賴固定 Release 簽名密鑰，密鑰只保存在安全備份與 GitHub Actions Secrets 中。

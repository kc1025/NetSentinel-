NetSentinel 是一套輕量化、無代理程式（Agentless）的集中日誌審查與合規自動化監控系統。

## 核心運作機制（日誌匯入架構）
本系統不直接遠端連入各主機抓取資料，而是仰賴各核心設備將 Syslog / 紀錄檔集中寫入至指定目錄（預設：/volume1/Public/log/），主排程腳本 monitor.sh 每日直接解析該目錄下的資料庫與文字檔。

## 管理後台位址與預設帳密
- 後台網址：http://x.x.x.x:8095
- 預設帳號：admin
- 預設密碼：admin（首次登入強制修改）

## 排程執行指令
/volume1/docker/netsentinel/monitor.sh


<img width="4096" height="4915" alt="image" src="https://github.com/user-attachments/assets/7ea8b14a-d746-4bb0-bbfe-5ca72bbbab0a" />

<img width="783" height="780" alt="截圖 2026-11-05 上午10 04 06" src="https://github.com/user-attachments/assets/20a12c60-18da-4ec9-9a3b-99354f808840" />

# 石頭寶寶(Stone Baby)
## 系統描述
本系統主要分為十一個部分。分別為店商平台系統（Web-based Online Shopping Platform 
System, WOSPS）、企業品牌電商子系統（Commodity Management Subsystem,CMS）、 服務
管理子系統（Service Management Subsystem, SMS）、搜尋與搜尋引擎優化管理系統
（Search and SEO Management System, SEOMS）、行銷管理子系統（Marketing Management 
Subsystem, MMS）、會員管理子系統（Membership and Account Management Subsystem, 
MAMS）、營運與財務管理子系統（Operational and Financial Management Subsystem, 
OFMS）、部落格管理子系統（Blog Management Subsystem, BMS）、購物車子系統
（Shopping Cart Management Subsystem, SCMS）、訂單及物流管理子系統（Order and 
Logistics Management Subsystem, OLMS）、商品管理子系統(Product Management 
Subsystem,PMS)、資料庫子系統（Database System, DBS）。 
## 系統架構圖
![image](https://github.com/user-attachments/assets/9420bc21-2aec-423a-8858-e93ffe8c89ee)
## 操作概念
Role A：一般使用者/消費者操作概念（Client Operational Concepts） 
消費者/使用者經由「店商平台系統」瀏覽商品。使用「搜尋與搜尋引擎優化管理系統」查
詢商品。選購商品後，加入「購物車子系統」協助保管商品以及進行提醒。結帳前須申請
會員，進入「會員管理子系統」。確認訂單以及追蹤物流進入「訂單及物流管理子系統」。
針對商品問題，透過「服務管理子系統」進行客服。利用「部落格管理子系統」了解更多
購物資訊、活動資訊。 
Role B：商場營運管理者操作概念（Operating Officer Concepts） 
透過「企業品牌電商子系統」讓消費者了解商場品牌資訊。使用「商品管理子系統」管理
商品狀態，包括上下架商品、管理商品數量/定價、發放/調整商品文案。使用「訂單及物
流管理子系統」可管理商品出貨狀況及物流進度。透過「行銷管理子系統」制定優惠券、
優惠期限、活動辦理等。透過「部落格管理子系統」投放購物資訊、活動資訊吸引消費者
購物並挖掘潛在消費者。透過「營運與財務管理子系統」自動生成財務報表，進而分析商
場的財務狀況。透過「服務管理子系統」，針對消費者問題進行客服。透過「會員管理子系
統」了解消費者個別購物情形，可客製化制定商品投放資訊。 
Role C：商場平台技術管理者操作概念（Technology Officer Concepts） 
消費者購物數據於「資料庫子系統」結合資料庫與市場調查數據資訊，經由營運、行銷管
理者與數據分析管理者之結果分析，再制定、調整演算法。透過「搜尋與搜尋引擎優化管
理系統」方便消費者快速搜尋到想要的商品。透過「店商平台系統」顯示符合搜尋字詞的
所有商品，推薦相關商品以及消費者可能喜歡之商品。透過「營運與財務管理子系統」制
定商品財務會計及營運分析報表公式於每期自動生成報表，提供營運、行銷管理者與數據
分析管理者之結果分析。 
## 資料庫綱要
![image](https://github.com/user-attachments/assets/fdc594fc-f244-48cd-9577-418db6b549b9)
## 頁面展示
![image](https://github.com/user-attachments/assets/3cd711f9-7a8a-43cf-8d21-34d4509429ba)
![image](https://github.com/user-attachments/assets/a7ef9251-0e85-488e-a729-b39cc05b4238)


# 操作流程
## 前置
### 安裝Django
   [按照網頁流程操作到Install Django](https://www.w3schools.com/django/django_install_django.php)
   
### 安裝XAMPP
第一步：安裝XAMPP（版本8.0.30）　　
![image](https://github.com/xzh0623/StonePet-Haven/assets/126553336/c014abd2-5562-452c-8f98-72294d5bdfdc)  
第二步：執行指令安裝  
![image](https://github.com/xzh0623/StonePet-Haven/assets/110615484/896567bb-7e71-45f9-8f15-10ea43e59bc2)　　
![image](https://github.com/xzh0623/StonePet-Haven/assets/110615484/ae22d749-e342-4619-9b73-78558c51db35)　　

第三步：執行XAMPP（開啟Apache MySQL，有本地SQL不用開啟）　　
![image](https://github.com/xzh0623/StonePet-Haven/assets/126553336/5975119d-1832-4553-bcc0-1a8603c8fdc5)  

### 進入資料庫管理頁面
![image](https://github.com/xzh0623/StonePet-Haven/assets/122630372/4e1a6f33-f647-4948-b11d-d7e6d1f6c37f)　　
* 進入後點擊新增，新增資料庫，名稱為web_development　　
![image](https://github.com/xzh0623/StonePet-Haven/assets/122630372/39305534-32d1-4117-8394-c2242ce8d55b)
* 將資料匯入至資料庫　　
![image](https://github.com/xzh0623/StonePet-Haven/assets/122630372/8ad1893f-d54f-42df-9729-ac9b6056aa97)　　
![image](https://github.com/xzh0623/StonePet-Haven/assets/122630372/bb9d4764-18b3-49a3-8bdb-85b9f2c58258)
* 選取完web_development.sql往下拉按下匯入按鈕，如果資料庫理沒有資料再匯入一次試試看　　

## 執行
執行XAMPP（開啟Apache, MySQL（如有連接本地SQL不用開啟）），到資料夾啟動vscode
![image](https://github.com/xzh0623/StonePet-Haven/assets/122630372/4a1ba02d-b5e7-4172-8d1a-46dfda538aaa)
先執行
```
python/py manage.py migrate
python/py manage.py collectstatic
python/py manage.py runserver
```
備註：如果圖片沒有顯示，使用前需要先設定 setting.py 裡面的```debug=true```，執行runserver後打開網頁讓他可以蒐集到圖片等快取資料，再把```debug=false```，重啟網站方可使用

### 使用者登入
資料庫有使用者資料可以使用  
登入使用者帳號：  
* 帳號：choco234  
* 密碼：234　（密碼皆為帳號後的數字）

### 管理員登入
* 帳號：hsiao
* 密碼：123

---
### 甘特圖
```mermaid
gantt
    title 甘特圖
    dateFormat  YYYY-MM-DD
    axisFormat  %m月%d號

    section 任務名稱
    研讀計畫       :a1, 2025-01-01, 1d
    任務分配       :a2, after a1, 4d
    取得匯總       :a3, after a1, 17d
    程式開發       :a4, after a2, 70d
    安裝硬體       :a5, after a3, 10d
    程式測試       :a6, after a4, 30d
    撰寫使用手冊   :a7, after a5, 25d
    傳授檔案       :a8, after a5, 20d
    系統測試       :a9, after a6, 25d
    使用者訓練     :a10, after a7, 20d
    使用者測試     :a11, after a9, 25d
```
```mermaid
graph LR
    no1["研讀計畫<br>編號:1<br>開始:第0天<br>結束:第1天<br>需時:1天"]
    no2["任務分配<br>編號:2<br>開始:第1天<br>結束:第5天<br>需時:4天"]
    no3["取得匯總<br>編號:3<br>開始:第1天<br>結束:第18天<br>需時:17天"]
    no4["程式開發<br>編號:4<br>開始:第5天<br>結束:第75天<br>需時:70天"]
    no5["安裝硬體<br>編號:5<br>開始:第18天<br>結束:第28天<br>需時:10天"]
    no6["任務分配<br>編號:6<br>開始:第75天<br>結束:第105天<br>需時:30天"]
    no7["取得匯總<br>編號:7<br>開始:第28天<br>結束:第53天<br>需時:25天"]
    no8["程式開發<br>編號:8<br>開始:第28天<br>結束:第48天<br>需時:20天"]
    no9["安裝硬體<br>編號:9<br>開始:第105天<br>結束:第130天<br>需時:25天"]
    no10["任務分配<br>編號:10<br>開始:第53天<br>結束:第73天<br>需時:20天"]
    no11["取得匯總<br>編號:11<br>開始:第130天<br>結束:第155天<br>需時:25天"]

    no1 --> no2
    no1 --> no3
    no2 --> no4
    no3 --> no5
    no4 --> no6
    no5 --> no7
    no5 --> no8
    no6 --> no9
    no7 --> no10
    no8 --> no10
    no9 --> no11
    no10 --> no11

```


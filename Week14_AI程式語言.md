# Week 14 AI必學程式語言 — Python 的應用

---

## A. 為何選 Google Colab？

* **免費使用**，省下鈔票，讓時間花在編程，不用煩惱錢包
* **免安裝**，瀏覽器打開，立刻寫代碼
* **免費GPU**， NVIDIA T4/A100，高效能，讓深度學習順暢
* **完美結合 Google Drive**，專案檔案輕鬆存取，資料夾共享簡單
* **多人即時協作**，不論是在宿舍還是咖啡館，和夥伴一起熱烈討論專案，享受協作

---

### 如何快速上手 Colab

1. 打開Colab → `File ▸ New Notebook`
2. 立刻執行第一行代碼：`print("Hello, sexy Python!")`
3. 記得啟用 GPU（`Runtime ▸ Change runtime type ▸ Hardware accelerator ▸ GPU`）

```python
!nvidia-smi -L
```

---

## B. Python 快速入門 

### 1. 為什麼要學 Python？

* **語法簡單，容易上手**，不用被複雜的規則綁住
* **功能強大，生態豐富**，不論資料科學、機器學習、還是自動化
* **廣泛應用於 AI 領域**，讓作品充滿智慧與未來感
* **跨平台自由**，電腦、雲端隨時隨地用
* **活躍社群**，永遠有夥伴一起挑戰新高度

---

### 2. 實戰練習快速體驗

**Demo 1: 取得 2025 年整年度月曆**

```python
import calendar
print(calendar.calendar(2025))
```

---

**Lab: 用 Python 玩轉生日**

```python
import calendar
y = int(input("輸入出生年："))
m = int(input("輸入出生月："))
d = int(input("輸入出生日："))
weekday = calendar.weekday(y, m, d)
days = ["星期一", "星期二", "星期三", "星期四", "星期五", "星期六", "星期日"]
print(f"出生在{days[weekday]}")
```

---

**Demo 2: 小小計算，玩轉轉換**

```python
c = float(input("請輸入攝氏溫度："))
f = c * 9 / 5 + 32
print(f"{c}°C 轉成華氏是 {f}°F，熱情不減！")
```

---

### 3. 用 Python 玩出風格

* 控制流程：`if`條件判斷，讓程式定
* 字串操作：翻轉句子
* 迴圈：重複節奏
* List操作：收納整理

---

**小挑戰：**

```python
# 印出倒三角星星形狀
for i in range(5, 0, -1):
    print(" " * (5 - i) + "★ " * i)
```



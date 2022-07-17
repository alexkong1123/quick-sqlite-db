# Quick-sqlite
### Overview
一個輕量級的鍵值數據庫基礎sqlite。
### Install
```
pip install quick-sqlite-database
```
### 例子
```py
from quick_sqlite import Database

db = Database("example.db")

db.set("name", "Dada878")

db.get("name") #Dada878
```
### 文檔
```Database(path, tableName?)```\
連接到數據庫

```db.set(key,value)```\
key設置值

```db.get(key)```\
key獲取值

```db.append(key,more)```\
為key值增加更多

```db.get_all()```\
將所有鍵和值作為數組返回
```db.get_all_key()```\
將所有鍵作為數組返回\

```db.delete(key)```\
按鍵刪除項目

```db.exists(key)```\
檢查鍵是否存在，返回布爾值

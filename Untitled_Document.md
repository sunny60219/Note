### ER-Model轉換成資料庫的SOP
1. 確認有幾個實體，也就是有幾個資料表  
2. 確認實體之間可能存在的關聯為何?(銷售?生產?)  
3. 決定每個實體的屬性，也就是資料表欄位  
4. 確認每個實體的主鍵
5. 確認資料表間的關聯關係為何種(1:1? 1:N? M:N?)

---
### 將關聯種類轉換為資料表

`完整的新刪修查基本為非同步作業`

| 同步函式| 非同步函式 (async)|
| ----------- | ----------- |
| void Test() {}      | async void TestAsync() {}  |
|     | async Task TestAsync() {} (以前寫法)        |
| int Test() {}    | async Task<int> TestAsync() {}  |
| string Test() {} | async Task<string> TestAsync() {}  |
| Customer Test() {} | async Task<Customer[]> TestAsync() {} |
| List<Customer> Test() {} | async Task<List<Customer>> TestAsync() {}  |
| IEnumerable<Customer> Test() {} | async Task<IEnumerable<Customer>> TestAsync() {} |

---
### 非同步作業 (世代)
`盡量使用第三代，效率佳`

1. Callback
2. 事件
3. async / await

---
### Get使用場合
1. 網址列
2. a連結
3. img src="..."



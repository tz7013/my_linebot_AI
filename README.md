## 使用line bot自動聊天機器人
### 程式編寫內容：
1. 使用Flask架設伺服器
2. 設定AI聊天機器人
3. 接收Line的POST請求，將輸入的訊息回傳給AI
4. 將AI回應的訊息傳到line

### 程式內容說明：
1. 儲存不同使用者的聊天訊息：
   一個line bot聊天機器人可以對不同使用者聊天, 為了分別每個使用的聊天訊息, 建立一個全域變數的dict, 儲存每個使用者的聊天訊息。
2. 保存每個使用者十筆訊息：
   為了避免訊息資料量過大, 使用了判斷式每個使用者訊息超過十筆將刪除最新兩筆。

更詳細的步驟建立line bot機器人可以參考以下我的筆記：
https://hackmd.io/N8lIDhsUS0C7oQN71H2Phw

掃描以下QR code可加入好友進行聊天, 這裡使用Render Wed Service免費版部屬AI程式, 超過15分鐘沒有請求會進入休眠, 重新請求需等待約1分鐘
第一次傳訊息沒有回應的話, 等約一分鐘再傳送一次就可以了
![image](https://github.com/user-attachments/assets/f7f84f8c-0a26-4c16-9074-a859bb368ebf)

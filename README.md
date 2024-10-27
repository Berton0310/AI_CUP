# AI_CUP :memo:
## 使用RAG相似度召回與答案比對結果  
### 總題數/正確/錯誤 : 50/46/4 答對率: 92%
### 以下是錯誤題號  
qid:111,question無卡提款服務是否可在ATM 機器上開通？,Rag_answer:149,Correct:76,  ⚠️:BM25答對  
qid:121,question有哪些方法可以手動檢查WebATM元件的安裝狀態？,Rag_answer:448,Correct:414,  
qid:135,question誰可以申辦玉山e指信貸,Rag_answer:138,Correct:28,  ⚠️:此題答案有誤  
qid:138,question要怎麼開通簡訊密碼?,Rag_answer:463,Correct:339,   ⚠️:463,399選項一樣 339多網址
## 補充  
### 原問題:     
無卡提款服務是否可在ATM 機器上開通？  
### RAG結果(第1):
'source':'faq448.txt',0.4812203347682953)  
### 正確答案(第5):  
'source': 'faq414.txt',0.5057258605957031)
### 刪除問號:
無卡提款服務是否可在ATM 機器上開通  
### RAG結果(第1):
'source': 'faq414.txt'},0.4786915183067322)
### 原問題RAG結果(第1):
'source':'faq448.txt',0.48257482051849365)
## 檔名對應
### text faq 原始程式碼  
### rag text json取問題答案  
## 問題  
### 資料集標點符號大小寫不一致 query統一補上小寫'?'
### 

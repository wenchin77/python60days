### 1. 在速度較慢的時候，可以先從哪邊開始檢查？
1. 讀取資料型態，因為資料型態會影響速度，例如 pkl 格式就比 csv 快 6 倍（可先將檔案用 pandas 讀入再轉 pkl or hdf 格式處理）
2. 使用內建函數或自定義函數，用內建的會比較快
3. 找有沒有向量化的資料處理方法，可加速

### 2. 資料過大時應採取什麼方式讓記憶體占用量下降？
將欄位型態降級，不需要存太多元素在一個數字中

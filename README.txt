# 挖挖（勿作怪異用途）

開網站需要收益，不然再大的夢想也很難維持，轉貼一則新聞關於 Pirate Bay
> 侵權網站不能像一般的網站一樣透過置放廣告賺錢，所以他們是如何維持營運呢？作為知名盜版網站之一的 Pirate Bay 就被發現他們的 JavaScript 代碼中，有包括著「借用」來訪客人的電腦處理器來進行挖掘 Monero 虛擬金幣，而且不能拒絕啊。不過這代碼似乎只有在搜尋結果頁和類別列表頁生效，大家可以試著留意 CPU 有沒有變得更高負荷
http://chinese.engadget.com/2017/09/18/pirate-bay-hijacks-cpus-for-digital-currency-mining/

以下教您如何實作一個瀏覽器「 挖礦 」，開始之前，你需要大略熟悉：

  - 英文
  - HTML 與 JAVACRIPT
  - *伺服器原理（非必要）

### 第一步：

申請一個 [Coinhive](https://coin-hive.com/)帳號，它提供挖礦的礦池、程式。而我們整個作品也都是靠它。
並且取得你的 Site Key (public)
fPOZ20CLfEKwaSYVYm7FtCPUaKMWooct

### 第二步：

下載這個Github的壓縮檔，解壓縮後找到index.html。
把原本的KEY：fPOZ20CLfEKwaSYVYm7FtCPUaKMWooct)  換成你的 KEY。
```html
    <script type="text/javascript">
    var miner = new CoinHive.Anonymous('fPOZ20CLfEKwaSYVYm7FtCPUaKMWooct', {
        threads: 2
    });
    </script>
```
### 第三步：

於 [Coinhive](https://coin-hive.com/)的後台 https://coin-hive.com/dashboard 觀察變化


![以下為範例圖：](dashboard.png)
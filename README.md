# 橫式卷軸社群──噗浪網頁UI設計──RE_myPLURK_UI X CSS
![RE_myPLURK_UI](https://images.plurk.com/5ViUFy9HQrHUvpN2Rh4rwu.png)
### 整體規劃與撰寫耗時:約七日
<br /><br />

# 優化內容
### 1. 拉高河道，使視覺更加廣闊
### 2. 個人資訊面板的收合，觀看資訊不受限螢幕尺寸
### 3. 將整體視覺風格整合更為統一
### 4. 噗文增加更為明顯的層級關係、游標懸浮回饋
### 5. 個人化噗浪獸
<br />
<br />


### 原版頁面
![原版](https://images.plurk.com/1mR22fyusQkFMWZLg4Qw39.png)
### 優化後新版頁面
![新版](https://images.plurk.com/41bBfoPBvIPxgwP5W8O1zY.png)
<br /><br />
實際效果可至此處查看、使用:<br />
[展示RE_myPLURK_UI](https://www.plurk.com/pmihle)

<br /><br />
# 目錄
[一、	噗浪頁面簡介](#one)<br />
[二、	優化動機與想優化之處](#two)<br />
[三、	修改提案](#three)<br />
[四、 修改後成果展示](#four)<br />
[五、 額外個人化設定](#five)<br /><br /><br />

<span id="one"> </span>
 ### 一、	噗浪頁面簡介
噗浪的網頁版頁面區塊大致分為上方導覽列、中間瀏覽噗文可左右滾動的橫軸河道、下方為含有個人資訊以及發表噗文的主控版。而噗浪官方提供使用者撰寫CSS語法以修改個人版面，增加個人化的風格彈性。<br /><br />
此為原版頁面設計:<br /><br />
![原版](https://images.plurk.com/1mR22fyusQkFMWZLg4Qw39.png)![原版2](https://images.plurk.com/4yCbrkuoi8djuYhE8PCse.png)
<br /><br /><br /><br />
<span id="two"> </span>
### 二、	優化動機與想優化之處
#### 1. 無法瀏覽所有資訊範圍
現代人電腦普及，瀏覽社群網頁已是日常生活的消遣之一，不過每個人使用的螢幕大小不同，以我來說，我平時使用的是筆記型電腦，螢幕較小，雖然能夠看見的頁面範圍已足夠個人方便使用發表貼文的功能，不過當造訪他人頁面時，使用者會無法直接看見對方的自我介紹資訊、點選加入好友、關注的按鈕(黃框處)，需將頁面下拉。<br /><br />
造訪他人的頁面時:<br /><br />
![他人頁面1](https://images.plurk.com/5wAUsh4AUAaE8cYWN35dTn.png)![他人頁面2](https://images.plurk.com/4J5g54StU6F2sDCWX77Dbt.png)<br /><br />
而對於使用者於個人頁面時，下方主控版的部分除了發文欄為必要區塊，自我介紹、Karma值、好友、粉絲、勳章等資訊，並非日常使用頻繁的區塊，在瀏覽時會壓縮時間軸上呈現的噗文空間。(黃框處)<br /><br />
![使用者個人頁面黃框](https://images.plurk.com/5BqOrHQrAHDhr44Qb9aBI3.png)<br /><br />
#### 2. 色彩與元件形狀
由於背景圖片會隨使用者而改變，整體風格與色調也會一同改變，不過噗文的底色、訊息提示的紅色標籤較難以融入使用者個人化頁面。
而噗文的形狀為長方形，視覺上較為尖銳，與下方主控台預設的圓角風格不同。若噗文密集時也會造成畫面視覺凌亂，也遮住使用者喜愛的背景。<br />
點擊噗文觀看留言、圖片時所呈現的背景顏色也為實色的白色，視覺效果較為生硬、銳利。<br /><br />
![原版點選圖片彈出視窗](https://images.plurk.com/5xsewoLJIbD1aDYMGw9Rbn.png)![原版點選噗文展開](https://images.plurk.com/4lMueLFdlKjMenzto0Gj5v.png)<br /><br />
#### 3. 河道畫面擁擠
當噗文較多的時候，河道上的噗文排列較為密集，給視覺帶來擁擠的感覺。<br /><br />
![原版](https://images.plurk.com/3mS85F2yP9TRvhUZICw1VN.png)<br /><br />
<br /><br />
<span id="three"> </span>
### 三、	修改提案
#### 1.	Framework
#### 網頁版面<br />
將河道拉高，使噗文能夠距離更開，去除時間軸線打破分隔，並且將發文面板置於最下方，將整體空間擴張。<br />
而個人資訊收合於頭貼並且置於畫面左上角的圓圈處，Karma值放置在頭貼下方。在點入他人頁面時，噗浪的河道會於最左邊有個空區塊，放置於此較不會阻擋使用者觀看河道上的噗文。<br />
將噗文、發文面板、發文者頭貼等元件改為圓角，使視覺更柔和、美觀。<br /><br />
![網頁框架](https://images.plurk.com/6lu3JQqie2ssJ4vR8Z9QOr.png)<br /><br />
#### 個人資訊版面<br />
當游標懸浮於頭貼時將可展開個人資訊，涵蓋暱稱、帳號ID、性別、自我介紹，並將背景包覆卡碼值。<br /><br />
![個人資訊版面框架](https://images.plurk.com/2AdQkpAOoC1Kzv87H3KzdA.png)<br /><br />
#### Karma值資訊版面<br />
當游標懸浮於Karma值時將可展開追蹤和統計，涵蓋好友、粉絲、徽章、登入時間等。<br /><br />
![Karma值資訊版面框架](https://images.plurk.com/7IGo4feomtmTNiaeFfSBiN.png)<br /><br />
#### 2.	訂定主用色
以較為柔和的紅與黑色為主，讓整體畫面更和諧，不會太過亮麗刺眼。並且透過不同透明度的白色以表示層級關係。而帶有透明度的色彩可以透出背景，讓畫面更有溫度。<br /><br />
![主色](https://images.plurk.com/1XhSLrtf8OI380vEuy7FiL.png)<br /><br />
<br /><br />
<span id="four"> </span>
### 四、 修改後成果展示
#### 1. 幾乎滿版的河道
![新版](https://images.plurk.com/1mR22fyusQkFMWZLg4Qw39.png)<br /><br />
#### 2.元件
#### 噗文
增加圓角、透明度增添視覺柔和效果。<br /><br />
![噗文](https://images.plurk.com/702GT8ZHSrueLS50jj8pNu.png) <br /><br />
#### 點開圖片後的彈跳視窗、噗文展開後
以不同透明度表示層級關係，而游標懸浮於回應時，該回應的透明度由opacity:0.5;改為opacity:0.8;，以表示滑到哪個回應。<br /><br />
![圖片彈跳視窗](https://images.plurk.com/2fYsQfqKp1I6m0TctQc61x.png) ![噗文展開](https://images.plurk.com/5XaRpygoSiMdSOzzyObFzd.png) <br /><br />
#### 顯示發表噗文時間
去掉時間軸線和預設的顯示發表噗文時間，修改為使用者觸碰到該則噗文時，顯示於下方，可在不影響觀看噗文的情況下，得知此則噗文的發表時間。<br /><br />
![發噗時間](https://images.plurk.com/12jmggoQjvFKdIlfkKeRTv.png)
#### 噗文回應數
將噗文回應數改為對話框形狀，並且在未讀的部分以陰影表現發亮提示的效果。<br /><br />
![已讀框](https://images.plurk.com/4QTmvwHdfRkb1tO2cmoBFe.png) ![未讀框](https://images.plurk.com/3PnN8Z9FIUp2bI2PZaD7Cf.png)<br /><br />
#### 發文面板
發文面板於游標未懸浮時透明度降低為opacity:0.3;，使網頁整體視覺效果加大，懸浮時為opacity:0.3;讓使用者方便使用。<br /><br />
未懸浮時:<br />
![發文面板_未懸浮](https://images.plurk.com/2HehU7vsOQuDqIUrFejVL8.png)<br /><br />
懸浮時:<br />
![發文面板_懸浮](https://images.plurk.com/6l3LxRosaJEIZf2vtH9DBI.png)<br /><br />
#### 訊息通知欄
修改訊息通知欄，統一整體色彩、透明度及圓角風格，並且置於發文面板左側。<br /><br />
![訊息通知欄_未懸浮](https://images.plurk.com/mH5caMzhpR6YkRetYnUqs.png)<br /><br />
當游標懸浮時會反紅回饋。<br /><br />
![訊息通知欄_懸浮](https://images.plurk.com/5f644yXWtjltW5WtFBsuOk.png)<br /><br />
#### 時間軸上標示的日期
由於去掉了時間軸和顯示每則噗發文的時間，原時間軸的位置變為寬敞，所以以較為清晰的opacity:1的黑色來標註瀏覽噗文日期的分隔點。<br /><br />
![訊息通知欄_懸浮](https://images.plurk.com/497zeb28Q2IgV8Q2YEP0F1.png)<br /><br />
#### 3. 個人資訊與Karma值面板的收合
利用互動的效果展開個人資訊，不必受限於螢幕大小需要下拉頁面才能觀看和點選，使用動畫效果增添了趣味性。在進入頁面時頭貼與卡碼值會有縮放的動畫，提示使用者去觸碰它們。<br /><br />
![個人資訊與Karma值面板](https://github.com/SevenPan07/RE_myPLURK_UI/blob/main/READMEimage/%E5%80%8B%E4%BA%BA%E7%89%88%E9%9D%A2%E5%B1%95%E6%BC%94.gif)<br /><br />
<br /><br />
<span id="five"> </span>
### 五、額外個人化設定
#### 噗浪獸
預設在畫面右上角的噗浪獸(另稱為噗寶)為噗浪的特色之一，此圖像會隨著節日不同而變化，官方有提供不同的選擇供使用者依喜好更換。<br />
使用者可以css方式置換噗浪獸的圖片，也可利用官方的框架更改為互動式噗寶可以讓使用者與自己喜愛的角色互動，產生療癒放鬆的心情。<br />
互動效果分別為待機時、游標懸浮時(以游標手指提示使用者點選)、點選時。<br /><br />
![gif噗寶](https://github.com/SevenPan07/RE_myPLURK_UI/blob/main/READMEimage/%E5%99%97%E5%AF%B6%E5%B1%95%E6%BC%94.gif)

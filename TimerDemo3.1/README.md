# TimerDemo3.1
[2016.11.10課後練習作品]

C＃七段顯示器(英文文件)<br/>
http://rockvignesh25.blogspot.tw/2012/02/seven-segment-display-in-c.html<br/>
運用到本週所教的Graphics就可達成<br/>
------
[實際應用]<br/>
使用之前 2016.02.24 的 FL_Timer3.1(TimerDemo3.1) 作品，<br/>
參考C#七段顯示器(英文文件)，加入其中，<br/>
此七段顯示器是運用到Graphics來SHOW出計時的時間。<br/>
(影片簡單DEMO它有的功能：開始/暫停、停止並歸零、顯示小數秒、視窗最上層顯示)<br/>
<br/>
由於只有把觸發開關加入在timer_Tick事件的程式碼，<br/>
原文的計時器誤差校正寫法都沒更動，而Graphics的繪圖效能會影響timer的觸發頻率，<br/>
就會在程式連續計時，超過1天~1天半之間，發現誤差。<br/>
本作品原先使用在協助上份工作的效率上，因此計時的數值準確性是重要的，<br/>
於是額外找到校正的方法，加以改善(紀錄起始時間，在一定時間後再抓取時間，校正)。<br/>
By Yu-Yi,Lin(Field-Long) 林侑億 20170420 整理<br/>

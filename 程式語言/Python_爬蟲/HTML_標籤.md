# HTML_主要標籤

#html #head #title #body

```html
<html> <!-- 網頁起始 -->

<head> <!-- 標頭 -->
    <title> <!-- 網頁標題-->
        標題123
    </title>
</head>

<body becolor="blue" text="red" link="black" vlink="blue" alink="yellow" background="images/bg1.jpg">
    <!-- body(網頁內容) 
    becolor="控制背景顏色" 
    text="控制文字顏色" 
    link="控制連結顏色" 
    vlink="控制已閱讀過的顏色" 
    alink="控制正在連結的顏色"            background="插入背景圖"-->

    網頁內容 <!-- 網頁內容 -->
</body>

</html>
```

# 超連結 a

#html #a #href

```html
<html>

<head>
    <title>
        title 123
    </title>
</head>

<body>
    <a href="https://www.ifreesite.com/color/#google_vignette" target="new">
        <!-- a(超連結標籤)，href="超連結路徑"，target="開新視窗(new)" -->

        精選六大領域課程 <!-- 超連結顯示文字 -->
    </a>
</body>

</html>
```

# 表格 table

#html #table

```html
<html>

<head>
    <title>
        標題123
    </title>
</head>

<body>

    <table border="2" bordercolor="green" bgcolor="blue" width="70%" height="50" cellpadding="50" cellspacing="10">
        <!-- table(插入表格)                 
         border="表格框線" 
	     bordercolor="框線顏色"  
	     bgcolor="背景顏色" 
	     width="寬度" 
         height="高度" 
         cellpadding="表格與文字之間的距離" 
         cellspacing="表格與表格之間的距離" -->

        <tr> <!-- 表格欄標籤-->
            <td>01</td> <!-- 表格列標籤-->
            <td>02</td>
            <td>03</td>
        </tr>
        <tr align="right" valign="top"> <!-- align="水平對齊(right、left、center)" valign="垂直對齊(top、middle、bottom)" -->

            <td align="center" valign="bottom">04</td>
            <!-- align="水平對齊(right、left、center)" valign="垂直對齊(top、middle、bottom)" -->

            <td>05</td>
            <td>06</td>
        </tr>
        <tr>
            <td rowspan="2">07</td> <!-- rowspan="垂直合併表格(記得刪除10儲存格)" -->
            <td colspan="2">08</td> <!-- colspan="水平合併表格(記得刪除09儲存格)" -->
        </tr>
        <tr>
            <td>11</td>
            <td>12</td>
        </tr>

    </table>
</body>

</html>
```

# 置中 center

#html #center

```html
<html>

<head>
    <title>
        <title>title 123</title>
    </title>
</head>

<body>
    <center>
        這裡的內容會置中 <!-- center(置中標籤) 在裡面的所有內容都會合併 -->
    </center>
</body>

</html>
```

# 粗_斜_底

#html #粗體 #斜體 #底線

```html
<html>

<head>
    <title> title 123 </title>
</head>

<body>
    <b>粗體</b> <!-- 粗體 -->
    <i>斜體</i> <!-- 斜體 -->
    <u>底線</u> <!-- 底線 -->
</body>

</html>
```

# HTML 特殊符號

#html #sub #sup #small #mark #nbsp #amp #quot #lt #gt

```html
<html>

<head>
    <title>
        special command
    </title>
</head>

<body>
    <sub> <!-- sub(下標) -->
        下標
    </sub>

    版權所有<sup> <!-- sup(上標) -->
        C
    </sup><br>

    NormL<small> <!-- small(縮小文字) -->
        small
    </small>Normal<br>

    Normal <mark>Marked</mark> Normal <br> <!-- mark(螢光標記) -->

    <del>$1600</del><br> <!-- del(刪除線) -->

    文 &nbsp; 文字文字 &nbsp; 文字文字文字<br> <!-- &nbsp;(文字空白) -->

    文 &amp; 文字文字 &amp; 文字文字文字<br> <!-- &amp;(&) -->

    文 &quot; 文字文字 &quot; 文字文字文字<br> <!-- &quot;("") -->

    文 &lt; 文字文字 &lt; 文字文字文字<br> <!-- &lt;(<) -->

    文 &gt; 文字文字 &gt; 文字文字文字<br> <!-- &gt;(>) -->

</body>

</html>
```

# 無序清單 ul

#html #ul

```html
<html>

<head>
    <title>
        title 123
    </title>
</head>

<body>
    <ul type="circle"> <!-- 有序清單顯示成空心圓點 -->
        <li>data 1</li> <!-- 清單內容 -->
    </ul>

    <ul type="disc"> <!-- 有序清單顯示成實心圓點 -->
        <li>data 1</li>
    </ul>

    <ul type="square"> <!-- 有序清單顯示成方塊 -->
        <li>data 1</li>
    </ul>

</body>

</html>
```

# 水平線 hr

#html #hr

```html
<html>

<head>
    <title>
        title 123
    </title>
</head>

<body>
    <hr> <!-- 水平線標籤 -->
    <hr color="blue"> <!-- 水平線設為藍色-->
    <hr size="50"> <!-- 水平線高度-->
    <hr width="500"> <!-- 水平線寬度設為 500 畫素-->
    <hr width="50%"> <!-- 水平線寬度設為螢幕的 50 %-->
    <hr align="left"> <!-- 水平線至左對齊-->
</body>

</html>
```

# 跑馬燈 marque

#html #跑馬燈

```html
<html>

<head>
    <title>
        跑馬燈
    </title>
</head>

<body>
    <marquee bgcolor="yellow" loop="1" direction="right" behavior="altermate" scrollamount="2">
        <!--bgcolor="背景色"
            width="寬"
            height="高"
            loop="跑幾次"
            direction="控制行進的方向(right／up／down)"
            behavior="slide文字碰到底邊就會停止／alternate左右碰撞"
            scrollamount="速度參數值，通常設定 1~10 的範圍，數字越大跑得越快。"
        -->
        <img src="images\bg1.jpg">
        <img src="images\bg1.jpg">
        <img src="images\bg1.jpg">
        <img src="images\bg1.jpg">
        <img src="images\bg1.jpg">
    </marquee>
</body>

</html>
```

# 標題 1~6

#html #h1 #h2 #h3 #h4 #h5 #h6

```html
<html>

<head>
    <title>
        title 123
    </title>
</head>

<body>
    <h1> title 1 </h1> <!-- 標題一 -->

    <h2> title 2 </h2> <!-- 標題二 -->

    <h3> title 3 </h3> <!-- 標題三 -->

    <h4> title 4 </h4> <!-- 標題四 -->

    <h5> title 5 </h5> <!-- 標題五 -->

    <h6> title 6 </h6> <!-- 標題六 -->
</body>

</html>
```

# 有序清單 ol

#html #ol

```html
<html>

<head>
    <title>
        title 123
    </title>
</head>

<body>
    <ol type="A"> <!-- 有序清單顯示成 A. B. C...-->
        <li> data 1 </li> <!-- 清單內容 -->
    </ol>

    <ol type="A"> <!-- 有序清單顯示成 a. b. c...-->
        <li> data 1 </li>
    </ol>

    <ol type="A"> <!-- 有序清單顯示成 I. II. III...-->
        <li> data 1 </li>
    </ol>

    <ol type="A"> <!-- 有序清單顯示成 i. i. iii...-->
        <li> data 1 </li>
    </ol>

    <ol type="A" start="3"> <!-- 有序清單顯示成 1. 2. 3...-->
        <li> data 1 </li>
    </ol>
</body>

</html>
```

# 斷行_段落_格式化

#html #br #p #pre

```html
<html>

<head>
    <title>
        title 123
    </title>
</head>

<body>
    <p> <!-- p(段落標籤) -->
        這裡的內容是一個斷落<br> <!-- br(斷行標籤) -->
        這裡的內容是一個斷落<br>
        這裡的內容是一個斷落<br>
        這裡的內容是一個斷落<br>
        這裡的內容是一個斷落<br>
        這裡的內容是一個斷落<br>
        這裡的內容是一個斷落<br>
        這裡的內容是一個斷落<br>
    </p>

    <pre>                           <!-- pre(格式化標籤) -->
            這裡的文字是格式化形式
            這裡的文字是格式化形式
            這裡的文字是格式化形式
            這裡的文字是格式化形式
            這裡的文字是格式化形式
        </pre>
</body>

</html>
```

# 插入圖片 img

#html #img

```html
<html>

<head>
    <title>
        title 123
    </title>
</head>

<body>
    <img src="images/bg1." width="50%" height="80%" align="right">
    <!-- img(插入相片) src="圖片路徑" width="寬度" height="高度" align="對齊" -->
</body>

</html>
```

# 按鈕 button

#html #button

```html
<html>

<head>
    <title>
        button
    </title>
</head>

<body>
    <button>
        button_1
    </button>

    <button disabled>
        button_2
    </button>

    <button><a href="https://dotblogs.com.tw/YiruAtStudio/2021/03/31/193907">
            button_3
        </a></button>
</body>

</html>
```

# 崁入本機音樂 audio

#html #崁入 #本機 #音樂

>Note
>檔案路徑要回上一層可以使用 ../

```html
<html>

<head>
    <title>
        insert MP3
    </title>
</head>

<body>
    <audio controls="controls">
        <source src="..\網頁範例\assets\music\王ok-唇膏.mp3">
        瀏覽器不支援此播放格式
    </audio>
</body>

</html>
```

# 崁入本機影片 audio

#html #崁入 #本機 #影片

```html
<html>

<head>
    <title>
        insert MP3
    </title>
</head>

<body>
    <audio controls="controls">
        <source src="..\網頁範例\assets\music\王ok-唇膏.mp3">
        瀏覽器不支援此播放格式
    </audio>
</body>

</html>
```

# 崁入YT影片 iframe

#html #崁入 #Youtube

```html
<html>
    <head>
        <title>
            Insert Youtube video
        </title>
    </head>

    <body>
        <iframe 
        width="949" 
        height="438" 
        src="https://www.youtube.com/embed/KhEAe2_T-4c" 
        title="[Playlist] 뉴욕에서 듣는 Johnny Stimson" 
        frameborder="0" 
        allow=
            "accelerometer; 
            autoplay; 
            clipboard-write; 
            encrypted-media; 
            gyroscope; 
            picture-in-picture; 
            web-share" 
            referrerpolicy=
                "strict-origin-when-cross-origin" 
                allowfullscreen>
        </iframe>
    </body>
</html>
```

# 崁入Google地圖 iframe

#html #崁入 #Google_Map

```HTML
<html>
    <head>
        <title>
            insert google map
        </title>
    </head>

    <body>
        <iframe 
            src=
                "https://www.google.com/maps/embed?pb=!1m28!1m12!1m3!1d116476.54391242431!2d120.55917221899419!3d24.17552022632207!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!4m13!3e9!4m5!1s0x346915407fb935b1%3A0xe4da182bedb7b871!2zNDM05Y-w5Lit5biC6b6N5LqV5Y2A5Lit5bGx5LiA6Lev5LiA5q61NTLomZ_nv5Tlu6Potbfph43lt6XnqIvooYw!3m2!1d24.213739099999998!2d120.54886169999999!4m5!1s0x3469235d7fb2c4a7%3A0x1cc856130460088d!2z5ZyL56uL5Yuk55uKIOenkeaKgOWkp-WtuA!3m2!1d24.1461668!2d120.73285879999999!5e0!3m2!1szh-TW!2stw!4v1723259120141!5m2!1szh-TW!2stw" 
            width="800" 
            height="600" 
            style="border:0;" 
            allowfullscreen="" 
            loading="lazy" 
            referrerpolicy="no-referrer-when-downgrade">
        </iframe>
    </body>
</html>
```

# 網頁不共用框架 iframe

#html #iframe #不共用 #框架

```HTML
<html>

<head>
    <title>
        iframe
    </title>
</head>

<body>

<!-- 崁入 a1.html 框架到 首頁 -->
<iframe src="pages/a1.html" width="700" height="300"></iframe>

<!-- 崁入 a2.html 框架到 首頁 -->
<iframe src="pages/a1.html" width="700" height="300"></iframe>


</html>
```

# 網頁共用框架 iframe

#html #iframe #共用 #框架

> 需在目錄新增
> /pages/a1.html
> /pages/a2.html

![[網頁共用框架 iframe.png]]

```html
<html>

<head>
    <title>
        共同框架_iframe
    </title>
</head>

<body>
    <button> <!-- 崁入 首頁的框架 到 首頁的框架 -->
        <a href="index.html" target="main">首頁</a>
    </button><br>

    <button> <!-- 崁入 a1.html 到 首頁的框架 -->
        <a href="pages/a1.html" target="main">頁面一</a>
    </button><br>

    <button> <!-- 崁入 a2.html 到 首頁的框架 -->
        <a href="pages/a2.html" target="main">頁面二</a>
    </button><br>

    <iframe name="main" src="https://www.dotblogs.com.tw/YiruAtStudio" width="800" height="800"></iframe>
</body>

</html>
```

## /pages/a1.html 內容

```html
<html>

<head>
    <title>
        Insert Youtube video
    </title>
</head>

<body>
<iframe width="560" height="315" src="https://www.youtube.com/embed/WHD7uNXFspk?si=7Ub6zEfLWbU6bvNg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</body>
</html>
```

# 表單 from

```html
<html>

<head>
    <title>
        表單
    </title>
</head>

<body>
    <form id="abc" method="get/post" action="abc.py" enctype="multipart/form-data"> <!-- 表單開始 -->
        <!--
                id="abc"    
                表單的名稱，不重複命名，
                通常在javascript呼叫的時候會使用，如果未使用到可以省略
                
                method="get/post"
                方法method= 最常使用的方式(GET、POST)
                GET在網頁url上送資料，大家都可以看到(適合較一般類型的資料)
                POST如果資料是需要隱密的，例如密碼資訊等，這時候就要選擇POST傳輸
                
                action="abc.py"
                按下submit 時表單要送到的後端處理頁面
                
                enctype="multipart/form-data"
                如果你的檔案需要上傳多媒體(例如圖片、音檔)等，需要加入此行
                
            -->
    </form> <!-- 表單結束 -->
</body>

</html>
```

# 表單_輸入 input

```html
<html>

<head>
    <title>
        表單
    </title>
</head>

<body>
    <form> <!-- 表單開始 -->
        帳號:<input type="text"><br> <!-- 讓使用者輸入文字 -->
        密碼:<input type="password"><br> <!-- 讓使用者輸入隱碼 -->
        <input type="submit"><br> <!-- 送出按鈕 -->
    </form> <!-- 表單結束 -->
</body>

</html>
```

# 表單_輸入屬性 input

```html
<html>

<head>
    <title>
        表單
    </title>
</head>

<body>
    <form> <!-- 表單開始 -->
        帳號:<input type="text" size="50" maxlength="10" placeholder="請輸入姓名" value="AAA">
            <!-- 
                size="50"                   格子大小
                maxlength="10"              輸入最大值
                placeholder="請輸入姓名"     提示文字
                value="AAA"                 預設值
            -->
    </form> <!-- 表單結束 -->
</body>

</html>
```
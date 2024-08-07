---
title: Android_Termux_Git_Setting
tags:
  - Termux
---


#### Use Termux clone gitgub repositories on the Android

</br>

>## 1. 在 Android 上安裝 [Termux](https://f-droid.org/zh_Hant/packages/com.termux/)

在 F-Droid 上下載 Termux 接著安裝

![[Images/Termux.png]]

</br>

>## 2. Termux 存取 Android 內部儲存空間

* 開啟 Termux，依序輸入以下指令

```txt
pkg install termux-am
```

```txt
pkg install git
```

* 當跑出 Do you want to continue? 時，輸入 Y 並按下 Enter 繼續

</br>

```txt
termux-setup-storage
```

* 這時會彈出對話窗，同意存取手機內部儲存空間

</br>

>## 3. Github 的 Token 設定

1. 登入 Github 點選右上角大頭照後選擇 `Settings`

    </br>

2. 側邊欄進入 `Developer settings`

    </br>

3. 側邊欄點選 `Personal access tokens` > `Tokens (classic)`

    </br>

4. `Generate new token` > `Generate new token (classic)`

    </br>

5. 以下設置

    ![alt text](/Images/Program_setting/Android_Termux/Android_Termux_Git_Setting/Generate_new_token.png)

    </br>

6. 至頁面最下按下 `Generate token`

    </br>

7. 之後就會獲得一組 token（請務必牢記，可以先複製貼上到剪貼簿上，稍後會用到）

    ![alt text](/Images/Program_setting/Android_Termux/Android_Termux_Git_Setting/token.png)

    </br>

>## 4. 使用 Termux 進入到想存放 Vault 的位置

> 這邊以裝置內部儲存空間的 Documents 為例

1. 開啟 Termux，輸入以下指令

    ```txt
    cd ~/storage/shared/Documents
    ```

    </br>

2. 到 Github 的 `Your repositories` ，進入同步用 Vault 的 Repository，按下 `<> Code` 的按鈕，並複製 HTTPS 下的網址

    ![alt text](/Images/Program_setting/Android_Termux/Android_Termux_Git_Setting/github_http.png)

    </br>

3. 繼續輸入以下指令，使用 Git Clone 來把 Github 上的 Vault 抓取進 Android 裝置中

    ```txt
    git clone https://github.com/XXX/XXX.git
    ```

    >上述 git clone 後面的網址請貼上剛才在 Repository 中複製的網址

4. 顯示 `Username for 'https://github.com':` 輸入自己於 Github 註冊的 Email address

    </br>

5. 顯示 `Password for 'xxxxxxxxxx':` 輸入剛才於 Github 中設定的 Token（此時的輸入，游標不會有所移動是正常的，請放心及正確輸入完，或是可以用複製貼上的方式）

    </br>

6. 當顯示 `Resolving deltas: 100%, done.` 或是沒有錯誤訊息時代表已經成功把 Git Repository clone 到內部儲存空間中了，也已經完成 Android 同步設定了，可以到裝置的我的檔案中去查看

    </br>

7. 打開 Obsidian APP > Open folder as vault > 選取剛才 clone 下來的 Vault 即可

    </br>

>## 5. 結語

以上步驟完成即完成了將先前同步備份到 Github 上的 Vault 同步到自己的 Android 裝置，</br>
此時也可以進入到 Obsidian Git 的第三方外掛程式中去看看自己的備份時間設定。

>## 6. 額外補充

當不同裝置在同步時可能會遇到版本衝突</br>
（多發生在手機跟電腦交互時的 workspace.json 跟 workspace-mobile.json 檔案上），</br>
可以考慮將這些在不同工作區會重新 build 的檔案加入到 .gitignore 中，</br>
或是有一定的 Git 相關知識可以去解這些衝突，</br>
因為有時會遇到的衝突會不太一樣，</br>
這就交給大家有遇到的時候再去處理了。

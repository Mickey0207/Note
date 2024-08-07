---
title: "Obsidian_Github_Setting"
tags:
  - Obsidian
  - Github
  - Setting
---


Use Obsidian clone github repositories on the Phone </br>
and comply git_push git_pull commit.

</br>

>## 1. 安裝Obsidian

### 1. Android 用戶

到 Google play 下載 [Obsidian](https://play.google.com/store/apps/details?id=md.obsidian&hl=zh_TW&pli=1) 並且安裝。

![alt](assets/Images/obsidian_github_setting/Android_Obsidian.png)

</br>

### 2. iOS 用戶

到 App Store 下載 [Obsidian](https://apps.apple.com/tw/app/obsidian-connected-notes/id1557175442) 並且安裝。

![alt](/images/obsidian_github_setting/iOS_Obsidian.png)

</br>

>## 2. 創建一個筆記

### 1. 創建一個新的筆記

打開 Obsidian 點選 `Create new vault`

![alt](/images/obsidian_github_setting/Create_vault.png)

</br>

### 2. 筆記設定

* `Vault name` Obsidian 的筆記名稱
* `Vault location` Obsidian 的筆記儲存位置

![alt](/images/obsidian_github_setting/Vault_setting.png)

</br>

### 3. Obsidian 外掛程式安裝

1. 頁面向`右滑`
2. 點選右上角的`齒輪`，進入設定
3. 點選 `第三方外掛程式`
4. 瀏覽 `社群外掛程式`
5. 搜尋 [Git](obsidian://show-plugin?id=obsidian-git)

    ![alt](/images/obsidian_github_setting/Search_Git.png)

    </br>

6. 安裝並啟用 Git

    ![alt](/images/obsidian_github_setting/Installed_Git.png)

    </br>

>## 3.  Clone Github rerepositories

1. 在主畫面下滑 開啟命令面板

    ![alt](/images/obsidian_github_setting/Enter_Code.png)

    </br>

2. 輸入以下命令

    ```txt
    Git: Clone an existing remote repo
    ```

    </br>

    ![alt](/images/obsidian_github_setting/Clone_repo.png)

    </br>

3. 出現`Enter remote URL`

    至要複製的 Github 儲存庫 複製 Git URL 然後貼上

    </br>

    ![alt](/images/obsidian_github_setting/Github_https.png)

    </br>

4. 出現`Enter directory for clone.`

    這是要我們輸入本地目錄，直接下一步就好,不需要田任何東西。

    </br>

5. 出現`Does your remote repo contain a .obsidian`

    這是詢問我們 Github 的儲存庫中有沒有`.obsidian`的資料夾，
    </br>如果是第一次複製就選擇 `NO`
    </br>如國是第二次含以上就選擇`Yes`

    </br>

6. 出現`To avoid conflicts, the local .obsidian directory`

    這是詢問是否要刪除本地的 .obsidian 資料夾，
    </br>如果是第二次含以上複製就需要選擇
    </br>`Delete all your local config and plugins`

    </br>

7. 出現`Specify depth of clone`

    這是詢問要複製什麼樣的檔案，直接略過下一步即可。
    </br> 就會將所有儲存庫的資料都複製下來

    </br>

>到這裡就將儲存庫成功複製下來了!!!

</br>

>## 4. 作者設定

在 Obsidian 中必需要設定作者才能執行 Commit Pull Push。

1. 打開設定

    </br>

2. 打開 Git 選項

    </br>

3. 下滑至 `Author name for commit` 填入 Github 的使用者名稱

    </br>

4. 下滑至 `Author email for commit` 填入 Github 的 E-mail 帳號

![alt](/images/obsidian_github_setting/Author_setting.png)

</br>

>## 5. 提交變更 Commit

### 畫面下滑打開命令面板後搜尋 `commit`

1. `Git: commit staged` 提交預存的檔案

    </br>

2. `Git: commit all change` 提交所有更改

    </br>

3. `Git: commit staged with specific messenger` 提交預存的檔案並帶有訊息

    </br>

4. `Git: commit all change with specific messenger` 提交所有更改並帶有訊息

![alt](/images/obsidian_github_setting/Commit.png)

>## 6. Git pull

### 1. 畫面下滑打開命令面板後搜尋 `Git: Pull`

</br>

>## 7. Git push

### 1. 畫面下滑打開命令面板後搜尋 `Git: Push`

1. 第一次 Push 會出現以下視窗，輸入 Github 的用戶名即可。

    ![alt](/images/obsidian_github_setting/User_name.png)

    </br>

2. 第一次 Push 會出現以下視窗，輸入 Github 的個人金鑰即可。

    ![alt](/images/obsidian_github_setting/personal_access_token.png)

    </br>

>## 7. Github 個人金鑰

1.登入 Github 點選右上角大頭照後選擇 `Settings`

2.側邊欄進入 `Developer settings`

3.側邊欄點選 `Personal access tokens` > `Tokens (classic)`

4.Generate `new token` > `Generate new token (classic)`

5.以下設置

![alt](/images/obsidian_github_setting/New_personal_access_token.png)

6.至頁面最下按下 `Generate token`

7.之後就會獲得一組 token

![alt](/images/obsidian_github_setting/token(class).png)

</br>

>## 8. 後記

實際使用過後，有時會出現一些問題，如 Pull 他無法成功，
</br>原因在於行動裝置版上的Obsidian的Git不是非常穩定，
</br>作者也有提供相關論述，所以建議電腦端用VS Code，可以穩定的運行Git，
</br>這樣才不至於資料會不見，最多只是以上步驟要重來。

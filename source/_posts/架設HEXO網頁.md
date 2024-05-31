---
title: 架設HEXO網頁
date: 2024-05-31 14:15:57
tags: 
- hexo
- 前端

---
### 架設網站前的準備工作
[Node.js官網](https://nodejs.org/en)

1. 載入最新的node.js 和 npm
2. 檢查 node.js 是否成功下載，那就是查詢下載的版本
3. 輸入 `$ node -v` 只要版本數字是跟你下載官網上顯示的版本相同即是下載完成
4. 輸入`$ npm -v` 看到版本數字及是下載完成



### HEXO 網站架設第一步
[HEXO官網](https://hexo.io/zh-tw/)

1. 打開終端機輸入指令
2. `$ npm install hexo-cli -g`
3. 輸入 `hexo init blog` 載入部落格套件
4. 終端機輸入指令進入 `cd blog`
5. 可以開啟伺服器 `hexo server` 看看你的網頁是否架設成功


### 新增部落格新的文章

1. 輸入 `hexo new + 新貼文標題`
2. 撰寫內容
3. 連接 Github new repository
4. 更改 `_config.yml` 下方 `URL` 的現有資料，並新增以下組態:
   ```# URL
   ## Set your site url here. For example, if you use GitHub Page, set url as 'https://username
   github.io/project'
   url: https://(username).github.io/(project)

5. 在 GitHub Pages 上部署 Hexo 
      [部屬連結](https://github.com/hexojs/hexo-deployer-git)

6. 安裝 hexo-deployer-git.
7. 清空 `_config.yml` 下方 `deploy` 的現有資料，並新增以下組態:
    ```deploy:
    type: git
    repo: https://github.com/<username>/<project>
    # example, https://github.com/hexojs/hexojs.github.io
    branch: gh-pages
 

7. 將你的 github 名稱和 repository 檔名輸入上去
8. `hexo clean`
9.  `hexo deploy`

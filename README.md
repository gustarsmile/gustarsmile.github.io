# edu.omilkyway.org

這個 repo 只做兩件事：

1. **替整個帳號的 GitHub Pages 設定自訂網域。** `CNAME` 檔寫的是 `edu.omilkyway.org`。GitHub 的規則是：帳號網站（也就是這個 `gustarsmile.github.io` repo）設了自訂網域之後，同一個帳號底下、自己沒有另外設網域的專案網站，都會改用這個網域，例如 `https://edu.omilkyway.org/taishang-ganying-pian/`；原本的 `https://gustarsmile.github.io/<repo>/` 會自動轉過來。所以各作品的 repo 不必各自設定。
2. **放 `https://edu.omilkyway.org/` 的首頁**（`index.html`），列出各個作品的連結。新增作品時在這裡加一行。

DNS 在 Cloudflare：`edu` 是一筆 CNAME，指到 `gustarsmile.github.io`，設成「僅 DNS」（不要開 Proxy，GitHub 才發得出 HTTPS 憑證）。

要還原成 `gustarsmile.github.io`：到這個 repo 的 Settings → Pages 把 Custom domain 清掉（或刪掉 `CNAME` 檔）即可。注意讀者存在瀏覽器裡的進度是跟著網域的，換網域會歸零。

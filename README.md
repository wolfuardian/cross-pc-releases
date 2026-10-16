# cross-pc releases

cross-pc 的發佈檔：在 Windows 檔案總管按右鍵「跨電腦 ▸ 複製／貼上」，經由 Google 雲端硬碟把檔案傳到另一台電腦的相同位置。原始碼不在這個 repo。

## 安裝

開「命令提示字元」或 PowerShell（一般權限，不要用系統管理員身分），貼上：

```
powershell -NoProfile -ExecutionPolicy Bypass -Command "[Net.ServicePointManager]::SecurityProtocol='Tls12'; irm https://github.com/wolfuardian/cross-pc-releases/releases/latest/download/install-context-menu.ps1 | iex"
```

最新版會下載到 `C:\Workshop\Scripts\cross-pc`。第一次安裝時會請你選擇 Google 雲端硬碟資料夾，裡面要有 `@temp-transmit`。之後的新版本會在通知區域圖示提示，按下即可更新。

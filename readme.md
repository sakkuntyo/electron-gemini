https://gemini.google.com を開くだけの electron アプリ

<img width="1266" height="766" alt="image" src="https://github.com/user-attachments/assets/8c1018d0-2a7c-4d94-940c-96f958ef5efd" />

一度ログインすると、再起動しても最初から chatgpt と話せる画面に行く様になります。

# 使い方
以下からダウンロードして展開し、 exe を実行します

https://github.com/sakkuntyo/electron-chatgpt/releases/download/1.0.0/chatgpt-client-1.0.0-win32-x64.zip

# 概要
- chatgpt に聞いて作成
  - https://chatgpt.com/share/6877ad5f-9e3c-8013-8ea0-e4b8b682039b
- nodejs 18.15 で動作確認。
- package.json は index.js -> main.js へ変更する以外に変更していません。
- npm install したパッケージは npx で使用する必要がありました。

# メモ
- 動作確認
  - ```npx electron .```
- パッケージング
  - ```npx electron-packager . chatgpt-client --platform=win32 --arch=x64 --icon=icon.ico --overwrite```

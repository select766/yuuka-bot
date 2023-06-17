# yuuka-bot
ユウカなりきりLINE Bot (ChatGPT)

ブルーアーカイブのユウカっぽい口調でチャットしてくれるチャットボットの試作品。

[「LINE Botをつくってみよう ～APIを試して学んでしっかりわかる～」](https://github.com/mochikoAsTech/startLINEBot)に沿ってシステムを構築する。AWS Lambdaに `aichatbot.py` をデプロイする。

注意
- 複数ユーザからのアクセスがあると何が起こるかわからない。会話の文脈をAWS Lambdaで動作するPythonコードのグローバル変数に保持しており、ユーザの識別をしていないため。文脈は数分で忘れる。

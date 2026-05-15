Daily Performance Plan v4 - Public Safe Version

修正内容:
- iPhone/Safariで「前日」ボタンを押すと2日前になる問題を修正しました。
- iPhone/Safariで「翌日」ボタンを押しても同じ日付のままになる問題を修正しました。
- 原因は JavaScript の toISOString() がUTC日付に変換され、日本時間で1日ずれることでした。
- 日付計算をローカル日付ベースに変更しています。
- Service Workerのキャッシュ名を daily-plan-v5 に更新しました。
- チーム名・対戦相手名は含めない公開用仕様を維持しています。

更新方法:
1. ZIPを展開
2. GitHubの既存リポジトリに以下5ファイルをすべて上書きアップロード
   - index.html
   - data.js
   - manifest.webmanifest
   - service-worker.js
   - README.txt
3. Commit changes
4. Safariで公開URLを開いて再読み込み
5. ホーム画面アプリを開き直す

古い表示が残る場合:
- Safariで公開URLを開いて下に引っ張って再読み込み
- それでも直らない場合は、ホーム画面アイコンを一度削除して再追加

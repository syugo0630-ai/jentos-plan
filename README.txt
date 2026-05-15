Daily Performance Plan v3 - Public Safe Version

修正内容:
- undefined表示の原因を修正しました。
- data.jsに「ウォームアップ / メイン / 補強 / クールダウン / 強度目安 / アドバイス」を全日付分で生成しています。
- index.html側にも旧データ形式へのfallbackを入れています。
- Service Workerのキャッシュ名を daily-plan-v4 に更新し、古いキャッシュを破棄します。
- チーム名・対戦相手名は含めない公開用仕様を維持しています。

GitHub Pages更新方法:
1. ZIPを展開
2. 既存リポジトリ内の以下5ファイルを上書きアップロード
   - index.html
   - data.js
   - manifest.webmanifest
   - service-worker.js
   - README.txt
3. Commit changes
4. Safariで公開URLを開き、再読み込み
5. ホーム画面アプリを開き直す

古い表示が残る場合:
- Safariで公開URLを開く
- 共有ではなく、ページを下に引っ張って再読み込み
- それでも残る場合は、Safariの履歴/Webサイトデータ削除、またはホーム画面アイコンを一度削除して追加し直してください。

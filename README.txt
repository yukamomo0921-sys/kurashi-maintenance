くらしメンテ v22

変更点：
・ヘッダー左のラッコの絵を、提供されたおこじょのイラストに変更
・「ひとつずつ進めよう」を非表示にし、日付を大きく表示
・右下のシャボン玉絵文字を削除
・今日の予定／今日の獲得ポイントを「数字＋pt」の表示に変更
・v21までの既存機能を引き継ぎ

GitHub Pages公開時は、このフォルダ内のファイル一式をリポジトリにアップロードしてください。


v24: Firebase account and cross-device sync
- Firebase Authentication: Email/password
- Cloud Firestore document: users/{uid}/appData/main
- The first sign-in on an account uploads this device's local data if no cloud document exists.
- If a cloud document already exists, its data is loaded onto this device.
- For GitHub Pages, add the published hostname to Firebase Authentication > Settings > Authorized domains.
- Keep the Firebase project on the Spark plan. Scheduled Firestore backups are not enabled.

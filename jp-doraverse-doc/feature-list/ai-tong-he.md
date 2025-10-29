---
description: Doraverseにアプリを統合し、AIが複数のサービスを横断して業務を一元管理できるようにします。
icon: circle-nodes
---

# AI 統合

メール、ドキュメント、CRMなど、複数のタブやアプリを行き来していると、作業のたびに時間や情報が分断されてしまいます。意思決定が遅れたり、細かな情報を見落としたり、「ちょっとした更新」もコピー＆ペーストや確認作業で1時間かかることもあります。

この課題を解決するのが、Doraverseの統合機能です。アプリをDoraverseに統合し、1つの場所で業務を完結できます。

#### Doraverseの統合とは

Doraverseの統合機能では、お客様の許可のもとで各種アプリと接続し、AIがデータ取得・文脈把握・アクション実行・業務完結まで自動化します。アプリ間の切り替えや手作業は不要です。

**50以上のアプリと統合可能**（例）：

* **Google Workspace**：Gmail、Drive、Sheets、Slides、Calendar、Meet
* **Microsoft365**：Outlook
* **ワークマネジメント／生産性**：Notion、Slack
* **営業・オペレーション**：HubSpot
* **エンジニアリング**：GitHub

今後も順次追加予定です。

***

### アプリを統合する手順

ホーム画面のチャットバーか&#x3089;**「統合管理」**&#x3092;開き、統合可能なアプリ一覧を表示します。連携したいアプリ&#x306E;**「接続」**&#x3092;クリックしてください。

<figure><img src="https://82687067-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbDXFRztwECY7ehfFFQoP%2Fuploads%2FxIFRjiVEZfgqY4NkQacl%2FScreenshot%202025-10-23%20at%2021.09.19.png?alt=media&#x26;token=6a398072-563e-498b-bc24-25f835237117" alt=""><figcaption></figcaption></figure>

<figure><img src="https://82687067-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbDXFRztwECY7ehfFFQoP%2Fuploads%2Fj9OYUn69hVWJxKQbz9Tv%2FScreenshot%202025-10-23%20at%2021.05.39.png?alt=media&#x26;token=4d701750-b1cd-4e7e-8cc0-f20b4c67c764" alt=""><figcaption></figcaption></figure>

**「Composio」**&#x306E;同意画面にリダイレクトされますので、OAuth経由でサインインし、要求されているスコープ（権限）を確認します。必要最小限のスコープのみ許可することを推奨します（後から拡張やアクセスの取り消しも可能です）

<figure><img src="https://82687067-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbDXFRztwECY7ehfFFQoP%2Fuploads%2F9LopbpPMnt5wp9EUobwQ%2FScreenshot%202025-10-23%20at%2021.17.15.png?alt=media&#x26;token=ef1aed92-6e23-4153-97b1-f06ee2517e2e" alt=""><figcaption></figcaption></figure>

承認が完了すると、自動的にDoraverseに戻り、アプリの統合が完了します。

📌 注意：ComposioはOAuth認証のSOC 2パートナーです。スコープやデータ保存、アクセス取り消しの詳細は[統合 - データコントロール](../help-center/faqs/integration-data-controls.md)をご参照ください。

***

### 統合済みアプリの利用方法

**「統合管理」**&#x304B;ら利用したい統合済みアプリを選択します。複数選択も可能です。

<figure><img src="https://82687067-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbDXFRztwECY7ehfFFQoP%2Fuploads%2FoHlXIs7eGa4htVMdHAk0%2FScreenshot%202025-10-23%20at%2021.16.09.png?alt=media&#x26;token=3850b1ba-01a3-49ab-a71d-98681dd5dd1c" alt=""><figcaption></figcaption></figure>

\
**統合モード**に入ると、Doraverseは自動的にモデル&#x3092;**「Doraverse統合」**&#x306B;切り替え、最適なパフォーマンスを発揮します。

あとはAIにやりたいことを指示するだけです。

<figure><img src="https://82687067-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FbDXFRztwECY7ehfFFQoP%2Fuploads%2FtVcLMs9rtoaHohMNlvrz%2FScreenshot%202025-10-23%20at%2021.13.07.png?alt=media&#x26;token=ed315b63-ea80-45f5-8149-8418ea4fd41d" alt=""><figcaption></figcaption></figure>

***

### クイックレシピ（アイデア＋そのまま使えるプロンプト例）

よく使われる業務は、下記のような短いプロンプトをチャットに貼り付けるだけでOKです。細かい手順はDoraverseが自動で補完します。

**Gmail / Outlook**

* **仕分け＆下書き**：「直近20件のメールを要約し、優先度を付けて、上位5件の返信案を作成してください。」
* **返信案作成**：「今週未返信のスレッドを探して、丁寧なリマインド返信を下書きしてください。」
* **スケジューリング**：「3日以上返信していないスレッドに丁寧なフォローアップを書いてください。」
* **フィルタ＆整理**：「14日以上前のニュースレターをすべてアーカイブし、各送信者の最新号だけ残してください。」

**Google Docs**

* **要点からドラフト作成**：「このメモをもとに、見出しとアクション項目付きの1ページ提案書を作成してください。」
* **ブラッシュアップ**：「このドキュメントを明確に編集し、冒頭に簡潔なエグゼクティブサマリーを追加してください。」

**Google Sheets**

* **KPIスナップショット**：「{file} からKPIを取得し、トレンドを含む週間サマリーを作成してください。」
* **データ整理**：「{sheet\_name} シートの重複を検出し、会社名を正規化してください。」

**Google Slides**

* **アウトラインから資料作成**：「このアウトラインをもとに10枚の営業資料を作成し、スピーカーノートを付けてPDFにエクスポートしてください。」
* **ブランド更新**：「{file} にマスターテンプレートを適用し、レイアウトの不具合を修正してください。」

**Google Calendar**

* **1日の予定まとめ**：「本日の会議、重複、準備メモを8項目で要約してください。」
* **時間予約**：「来週の空き時間から45分枠を探して、セラピーの予定を入れてください。」

**Google Meet**

* **会議ダイジェスト**：「本日のプロダクト同期のノート／録画から、担当者別のアクション項目を抽出してください。」
* **共有**：「会議サマリーを参加者にメール送信してください。」

**Slack**

* **チャンネル要約**：「{topic} の直近24時間をまとめ、トレンドと緊急チケット5件を抽出してください。」
* **アナウンス**：「{#channel} にリリースノートを投稿し、DocsやGitHubへのリンクを添付してください。」

**Notion**

* **会議ノートDB**：「{task} 用のNotionページを作成し、参加者・決定事項・次のアクションを記載してください。」
* **タスク登録**：「この箇条書きをNotionのタスクDBに変換し、担当者と期限を設定してください。」

**HubSpot**

* **自動ログ**：「直近のクライアントメールを{contact}に記録し、金曜のフォローアップタスクを追加してください。」
* **パイプライン更新**：「{client}用の新規案件を作成し、{employee}にアサインしてください。」

**GitHub**

* **PRレビューまとめ**：「{repo}のオープンPRを一覧化し、リスク要約と担当者への次アクションを記載してください。」
* **リリースノート**：「{ver}以降のマージ済みPRを人間向けのリリースノートにまとめてください。」


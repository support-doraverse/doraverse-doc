---
description: アプリをDoraverseに統合する際のデータアクセスと利用方法についてご案内します。
icon: circle-nodes
---

# 統合とデータコントロール

## Doraverseはどのようにアプリと統合しますか？

Doraverseは、Composio（当社のSOC 2準拠の統合パートナー／サブプロセッサー）を利用したOAuth経由でアプリと統合します。OAuthにより、パスワードを共有せずに、範囲が限定された取り消し可能なアクセス権を付与できます。

## Composioとは？私のデータはどう扱われますか？

ComposioはOAuthの仲介を行う統合プラットフォームです。お客様がリクエストしたアクション（例：Slackチャンネルの読み取り、Notionページの作成）のみを実行し、その結果をDoraverseに返します。Composioによるデータの収集・利用方法は[プライバシーポリシー](https://composio.dev/privacy)でご確認いただけます。

## Doraverseは統合したアプリからどのようなデータにアクセスできますか？

OAuth認証時にお客様が承認した最小限のスコープのみをリクエストします（最小権限の原則）。

Composio経由で利用できる主なツールキットとアクション例：

<table><thead><tr><th width="92.77166748046875">アプリ</th><th width="227.07586669921875">ツールキット・主なアクション</th><th width="235.5535888671875">データカテゴリ</th><th>スコープの例</th></tr></thead><tbody><tr><td><strong>Gmail</strong></td><td>メールボックス接続、メッセージの送受信・閲覧</td><td>メッセージメタデータ、承認済みメッセージ本文・添付ファイル、送信権限があれば送信も可</td><td><p><code>gmail.readonly</code></p><p><code>gmail.send</code></p></td></tr><tr><td><strong>Google Drive</strong></td><td>50以上のアクション（コメント作成/削除、ショートカット作成など）</td><td>ファイル/フォルダのメタデータ、読み取り権限があればファイル内容、書き込み権限があれば操作可</td><td><p><code>drive.readonly</code></p><p><code>drive.file.picker</code> </p></td></tr><tr><td><strong>Google Docs</strong></td><td>ドキュメントの作成・閲覧・更新</td><td>承認済みドキュメントのメタデータ・内容</td><td><code>documents</code><br><code>drive.file</code></td></tr><tr><td><strong>Google Slides</strong></td><td>プレゼンテーションの作成・複製・更新</td><td>承認済みプレゼンテーションのメタデータ・スライド内容</td><td><p><code>read.slide</code></p><p><code>edit.slide</code> </p></td></tr><tr><td><strong>Google Sheets</strong></td><td>シート範囲の読み取り・更新など</td><td>承認済みシートのメタデータ、セル値・範囲</td><td><code>spreadsheets</code><br><code>drive.file</code></td></tr><tr><td><strong>Google Calendar</strong></td><td>イベントの管理・閲覧</td><td>カレンダーリスト、イベント（タイトル・時間・参加者など）</td><td><code>calendar</code><br><code>calendar.events</code></td></tr><tr><td><strong>Google Meet</strong></td><td>Meet連携による会議調整</td><td>Meet/Calendarスコープで許可された会議メタデータ（リンク・時間など）</td><td><p><code>meetings.space.crea</code></p><p><code>calendar.events</code></p></td></tr><tr><td><strong>Slack</strong></td><td>チャンネル・メッセージの閲覧、書き込み権限があれば投稿も可</td><td>承認済みチャンネルリスト、メッセージ、書き込み権限があれば投稿可</td><td><p><code>channels:history</code></p><p><code>chat:write</code></p></td></tr><tr><td><strong>Notion</strong></td><td>30以上のアクション、ページ・データベースの作成・更新</td><td>統合で共有したページ・データベース・プロパティ、スキーマメタデータ</td><td>スコープ文字列なし（ページ/DB共有で権限付与）</td></tr><tr><td><strong>HubSpot</strong></td><td>設定したスコープに応じたCRMエンドポイント利用</td><td>承認済みCRMオブジェクト（コンタクト・企業・取引など）</td><td><p><code>crm.objects.contacts.write</code></p><p><code>crm.objects.deals.write</code></p></td></tr><tr><td><strong>GitHub</strong></td><td>800以上のアクション（イシュー、PR、リポジトリの読み書き等）</td><td>リポジトリメタデータ、イシュー/PR内容、リポジトリスコープがあればコード、書き込み権限があれば操作可</td><td><p><code>repo</code></p><p><code>read:org</code></p></td></tr><tr><td><strong>Outlook</strong> </td><td>Outlookツールキット、必要に応じてOneDrive/Teams/SharePoint/Excelの追加スコープ</td><td>メール、カレンダー、ファイル、Teams/チャンネル等</td><td><code>Mail.Read</code>, <code>Calendars.Read</code></td></tr></tbody></table>

**📌 ご注意:** 実際のアクセス範囲はComposioの同意画面で設定したスコープに準じます。

## Doraverseは私のデータをAIモデルの学習に利用しますか？

いいえ。統合アプリから取得したコンテンツはリクエストの実行のみに使用され、汎用モデルの学習には利用されません。（Googleコネクタの場合、「Improve the model for everyone」がONでもコネクタ経由の内容は学習に使われません。）

## どのAI／モデルプロバイダーが私のデータを処理しますか？

機能によっては、Doraverseが選択したモデルやAgentにプロンプトやコンテキストを送信する場合があります。タスクに必要な範囲のみ共有されます。現在のサブプロセッサー一覧は[support@doraverse.com](mailto:support@doraverse.com)までご請求いただけます。

## Doraverseが私の知らないうちにアプリで操作を行うことはありますか？

いいえ。自動アクション（例：Slackへの投稿、Notionページの作成、GitHub PRへのコメントなど）は、アプリごとにお客様が明示的に有効化した場合のみ実行され、すべて監査ログに記録されます。

## 統合の切断・権限の取り消し方法は？

Doraverseでの操作方法：**チャットバー → 統合管理** に進み、切断したいアプリを選択して「切断」をクリックしてください。OAuthトークンは直ちに無効化されます。

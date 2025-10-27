---
description: ワークスペースのメンバーを管理できます。メンバーの招待、ロールの割り当て、削除が可能です。
---

# 👤 メンバー管理

[メンバーを招待](member-management.md#add-members)

[ロールを変更](member-management.md#change-roles)

[メンバーを削除](member-management.md#removing-members)

[ワークスペース所有者の退会](member-management.md#workspace-owners-leaving)

「メンバー」タブでは、DoraverseのWorkspaceメンバーを管理・整理できます。

ナビゲーション：**アカウント → 管理者設定 → メンバー**

ここでできること：

* 現在のメンバー一覧、割り当てられたロール、有料席数を確認できます。
* メールアドレス、ロール、最終アクティブ日時でメンバーを検索できます。
* 新しいメンバーの招待、ロールの変更、メンバーの削除が行えます。

<figure><img src=".gitbook/assets/Member Management.png" alt=""><figcaption></figcaption></figure>

***

## メンバーを招待

1.  **「メンバーを招待」**&#x3092;クリックします。

    📌 **注意：**&#x57;orkspaceの利用可能な席数の範囲内でのみメンバーを招待できます。
2. 詳細を入力します：
   * **メールアドレス**：1行につき1件入力してください。
   * **ロール**：以下から選択できます。
     * **所有者**：Workspaceの全権限を持ちます。
     * **メンバー**：Doraverseの機能のみ利用可能（管理者設定へのアクセス不可）。
     * **請求管理**：請求情報のみ管理できます。
     * **ビュアー**：閲覧のみ可能です。
   * **部署**：所属する部署を割り当てます。詳細は[部署設定](https://help.doraverse.com/settings/workspace-setting/department)をご参照ください。

<figure><img src=".gitbook/assets/Screenshot 2025-10-04 at 22.13.29.png" alt=""><figcaption></figcaption></figure>

3.  **「メンバーを招待」**&#x3092;クリックします。

    Doraverseから招待メールが送信され、ログイン情報が案内されます。

    まだ参加していない場合は、**「メールを再送信」**&#x3092;クリックすると再度招待メールを送れます。

***

## ロールを変更

メンバーの権限を変更する手順：

* メンバー一覧から該当者を探します。
* 「ロール」ドロップダウンをクリックし、新しいロールを選択します。

<figure><img src=".gitbook/assets/Change role.png" alt=""><figcaption></figcaption></figure>

📌 **注意**：ロールの変更はWorkspace所有者のみが行えます。

***

## メンバーを削除

Workspace所有者は、いつでもメンバーを削除できます。

* メンバー一覧から該当者を探します。
* 名前の横にある「ロール」ドロップダウンを開きます。
* **「Workspaceから削除」**&#x3092;選択します。

{% hint style="info" %}
#### Important:

#### 削除時の注意点

* 削除されたメンバーは、即時Workspaceへのアクセス権を失います。
* 過去のデータ（チャット履歴、タスク、AI出力、アップロードファイル、統計情報など）はWorkspace内に残りますが、履歴上の名前&#x306F;**「削除済みアカウント」**&#x306B;置き換わります。
* メールアドレスはシステムログに保持され、監査や復元のためにアーカイブされる場合があります。
* 再招待された場合は、以前のアカウントとは紐付かない**新規メンバー**として参加します。
{% endhint %}

***

## Workspace所有者の退会

他のメンバーが在籍している場合、唯一の所有者はWorkspaceを退会できません。

退会したい場合は、他のメンバーを所有者に割り当てるか、全メンバーを削除してください。

最後のユーザーが退会すると、Workspaceは**非アクティブ**となります。

**30日間の猶予期間**内にメンバーを追加すれば再開できますが、30日を過ぎるとWorkspace（およびサブドメイン）は完全に削除されます。詳細は[**利用規約**](https://doraverse.com/article/gl/term-of-service)をご参照ください。

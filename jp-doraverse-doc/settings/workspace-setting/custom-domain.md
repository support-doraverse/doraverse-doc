---
description: Doraverseでカスタムドメインを設定する
---

# カスタムドメイン

Doraverseでは、`ai.my-domain.com` や `work.my-domain.com` のようなカスタムドメインを設定できます。これにより、ワークスペースへのアクセスが簡単になり、自社専用の環境として運用できます。

> 📌 ご注意:
>
> Doraverseはドメインの販売や、現在ご利用中のドメインプロバイダーの代行は行いません。お客様ご自身で所有・管理しているドメインが必要です。Doraverseは、そのドメインとご指定のカスタムドメインを接続する役割のみを担います。

以下に、設定手順を順を追って説明します。

### ステップ1：管理者ワークスペースにアクセス

ホーム画面か&#x3089;**「アカウント」→「管理者設定」→「Workspace設定」→「ドメイン」**&#x3078;進みます。&#x20;

<figure><img src="../../.gitbook/assets/1.png" alt=""><figcaption></figcaption></figure>

### ステップ2：カスタムドメインを入力

カスタムドメインを追加する際は、スムーズな設定のために以下のルールを守ってください：

* すでに所有しているドメイン（NamecheapやGoDaddyなどで購入済み）である必要があります。
* カスタムドメインには必ずサブドメインを含めてください（例：`www.my-domain.com`、`work.my-domain.net`、`chat.my-domain.com` など）。

<figure><img src="../../.gitbook/assets/Screenshot 2025-08-07 at 17.19.42.png" alt=""><figcaption></figcaption></figure>

例:

* `aidol.social` がルートドメイン（メインドメイン）
* `work` がサブドメインのプレフィックスです（メインドメインの前に付ける部分）

👉  サブドメインを含めると、`work.aidol.social` のようになります。       &#x20;

> ❓なぜサブドメインが必要？
>
> 多くのプロバイダーでは、接続を正しく行うためにサブドメイン（「www」や「portal」など、メインドメインの前に付く部分）が必要です。

**「ドメインを追加」**&#x3092;クリックすると、Doraverseがドメインプロバイダーに追加すべき正確なDNSレコード情報を表示します。

<figure><img src="../../.gitbook/assets/subdomain.png" alt=""><figcaption></figcaption></figure>

### ステップ3：ドメインプロバイダーでCNAMEレコードを設定

* ドメイン管理画面（DNSレコードやホストレコードの設定）にアクセスします。
* Doraverseで表示された内容をもとにCNAMEレコードを作成してください：
  * ホスト名/Name：Doraverseで表示された「Name」をコピー
  * 値/Points to：Doraverseで表示された「Value」をコピー
  * TTL（有効期間）：通常は「自動」で問題ありません。すぐに反映させたい場合は5分など短い値に設定してください。

設定を保存します。DNSレコードの反映には時間がかかる場合があります。

<figure><img src="../../.gitbook/assets/Screenshot 2025-08-07 at 17.24.22.png" alt=""><figcaption></figcaption></figure>

設定を保存します。DNSレコードの反映には時間がかかる場合があります。

### ステップ4：接続を確認

Doraverseのドメイン設定画面に戻り、**「確認」**&#x3092;クリックします。正しく設定されていれば、ワークスペースがカスタムアドレスで利用可能になります。

<figure><img src="../../.gitbook/assets/Screenshot 2025-08-07 at 23.27.35.png" alt=""><figcaption></figcaption></figure>

カスタムドメインはいつでも変更可能です。設定を変更する場合は、同じ手順を繰り返してください。

<figure><img src="../../.gitbook/assets/Screenshot 2025-08-07 at 23.33.58.png" alt=""><figcaption></figcaption></figure>

***

### 💡 Domain Name Mismatch Detected」エラーの対処法

<figure><img src="../../.gitbook/assets/Screenshot 2025-08-07 at 23.01.47.png" alt=""><figcaption></figcaption></figure>

このエラーは、DoraverseがDNS設定を確認した際、CNAMEやドメイン名がDNSプロバイダーの情報と一致しない場合に表示されます。

### 対処方法:

* 入力したドメイン／サブドメインを再確認してください。スペルミスや余分なスペース、抜けがないかご確認ください。https:// や http:// は含めないでください（リンクではなく、ドメイン名のみを入力）。
* Doraverseで表示された通りに**CNAMEレコード**を追加してください： 種類：CNAME Name/Host：表示された内容をコピー（例：work） Value/Points to：表示された値をコピー（例：[clsb31ax1.doraverse.com](http://clsb31ax1.doraverse.com/)）
* ルートドメイン（[mycompany.com](http://mycompany.com/) など）をCNAMEの「Name」として使用しないでください（特別な指示がない限り）。
* 数分待ってから再度お試しください。DNSの反映には時間がかかる場合があります。

<details>

<summary>ドメインの詳細については、こちらをご覧ください。</summary>

[https://www.godaddy.com/help/what-is-dns-665\
\
https://www.godaddy.com/help/manage-dns-records-680\
\
https://www.namecheap.com/support/knowledgebase/article.aspx/434/2237/how-do-i-set-up-host-records-for-a-domain/\
\
https://www.namecheap.com/support/knowledgebase/article.aspx/9646/2237/how-to-create-a-cname-record-for-your-domain/\
\
https://developers.cloudflare.com/dns/zone-setups/partial-setup/setup/\
\
https://support.squarespace.com/hc/en-us/articles/360002101888-Adding-custom-DNS-records-to-your-Squarespace-managed-domain](https://www.godaddy.com/help/what-is-dns-665https://www.godaddy.com/help/manage-dns-records-680https://www.namecheap.com/support/knowledgebase/article.aspx/434/2237/how-do-i-set-up-host-records-for-a-domain/https://www.namecheap.com/support/knowledgebase/article.aspx/9646/2237/how-to-create-a-cname-record-for-your-domain/https://developers.cloudflare.com/dns/zone-setups/partial-setup/setup/https://support.squarespace.com/hc/en-us/articles/360002101888-Adding-custom-DNS-records-to-your-Squarespace-managed-domain)

</details>

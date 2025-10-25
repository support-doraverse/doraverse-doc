---
description: Doraverseの体験をかんたんにパーソナライズし、ワークスペース環境を自在に管理できます。
icon: sliders-up
---

# アカウント設定

[一般設定](account-setting.md#general-setting)

[チャット設定](account-setting.md#chat-setting)

[パーソナライズ](account-setting.md#personalization)

[データコントロール設定](account-setting.md#data-controls)

[連携アプリ](account-setting.md#connected-apps)

Doraverseのアカウント設定では、ワークスペースの使い方を自由にコントロールできます。体験のカスタマイズからプライバシー管理、連携アプリの設定まで、生産性とセキュリティの両立をサポートします。

ホーム画面か&#x3089;**「アカウント」 → 「設定」**&#x3092;選択してください。

## 一般設定

<figure><img src="../.gitbook/assets/Screenshot 2025-08-29 at 16.35.15.png" alt=""><figcaption></figcaption></figure>

* **テーマ**：環境や好みに合わせて、ライトモードとダークモードを切り替えることができます。
* **言語**：インターフェースの言語を変更し、より使いやすくできます。
* **ユーザーメッセージをMarkdownで表示する**：有効にすると、メッセージがMarkdown形式で表示されます（コードやリスト、書式設定に便利です）。
* **チャット開始時に最新メッセージへ自動スクロール**：オンにすると、チャットを開くたびに自動的に最新メッセージへ移動します。
* **右端のサイドパネルを非表示にします**：メインチャットエリアに集中したい場合に、画面をすっきりさせることができます。
* **アーカイブされたチャット**：アーカイブした会話を検索・管理できます。

## Chat Setting

<figure><img src="../.gitbook/assets/Screenshot 2025-08-29 at 16.52.21 (1).png" alt=""><figcaption></figcaption></figure>

* **Message Font Size:** Adjust how large the chat text appears for better readability.
* **Chat direction:** Set the direction for your chat input
  *   **LTR (Left-to-Right):**

      Most languages, including English, are written from left to right. This is the default chat direction in Doraverse.
  *   **RTL (Right-to-Left):**

      Some languages, like Arabic and Hebrew, are written from right to left. Doraverse supports RTL for a seamless, natural reading and writing experience.
* **Press Enter to send messages:** When enabled, pressing `ENTER` will send your message. When disabled, pressing Enter will add a new line, and you’ll need to press `CTRL + ENTER` / `⌘ + ENTER` to send your message.
* **Maximize chat space:** Toggle this to instantly expand your chat box to its maximum size, allowing you to focus fully on your conversation.
* **Center Chat Input on Welcome Screen:** This positions the chat input box in the center when you open Doraverse, create a clean look when you first open Doraverse.
* **Always show code when using Code Interpreter:** Enable this to automatically display the code executed by Code Interpreter for every request—giving you greater visibility and control over each step.
* **Parsing LaTeX in Messages:** Enable Parsing LaTeX in Messages to automatically turn LaTeX code into beautifully rendered mathematical equations within your chats. This helps you write and share complex math and scientific formulas with clarity—perfect for technical discussions or collaborative problem-solving.\
  If you don’t need math formatting or want faster performance, you can disable this option to keep messages simple and speed up loading.
* **Save drafts locally:** When enabled, the text and attachments you enter in the chat form will be automatically saved locally as drafts. These drafts will be available even if you reload the page or switch to a different conversation. \
  Drafts are stored locally on your device and are deleted once the message is sent.
* **Scroll to the end button:** Quickly jump to the bottom of a long conversation.
* **Save Badges State:** Enable Save Badges State to keep your chat badges just as you set them—every new chat will start with the same badge settings as your previous chat. Disable it, and badges will reset to their default each time you start a new conversation.
* **Enable Switching Endpoints Mid-Conversation:** Turn on this to seamlessly change the AI model or Agent you’re using within the current chat—giving you the flexibility to adapt to different needs without starting over.
* **Use Default fork option:** lets you create a separate copy of a chat from any message, so you can continue the conversation in a new direction without changing the original conversation.\
  When choose a fork option, you can choose how Doraverse gathers messages:
  * **Visible messages only:** Includes just the direct path to your selected message. Use this for a focused fork that isolates a specific part of the conversation.
  * **Include related branches:** Adds any branches connected along that path. Great when you want additional context or relevant side discussions alongside your main topic.
  * **Include all to/from here:** Gathers all connected messages and branches in both directions. Ideal for comprehensive forks where you need the full context and all related history.
* **Start fork from target message by default:** When this is enabled, your fork will automatically start from the message you choose and include everything up to the latest message, following the fork option you select.

## Personalization&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2025-08-29 at 17.05.24.png" alt=""><figcaption></figcaption></figure>



The **Personalization** section allows you to make Doraverse feel more tailored to your way of working. You can set up custom instructions for the AI and enable memory so Doraverse can remember details across sessions.

* **Customization:** This lets you guide how Doraverse should respond to you. By adding custom instructions, you can tell Doraverse your preferred style, context about your work, or specific details it should always keep in mind when assisting you.\
  To set this up, click **Customize**, fill in your instructions, and save them.

<figure><img src="../.gitbook/assets/Screenshot 2025-08-29 at 17.06.08.png" alt=""><figcaption></figcaption></figure>

* **Memory:** Doraverse can remember key details—like your name, preferences, or project goals, to make future chats more tailored and helpful. You can tell Doraverse exactly what to remember by saying things like, “Remember that thing I just have said.”\
  Doraverse also references previous messages in your current session for context. To make sure details last for future chats, use saved memories.\
  To use Memory:
  * **Teach:** Just tell the AI what you want it to remember.\
    &#xNAN;_&#x46;or example: “Remember I’m focused on marketing strategies this quarter.”_
  * **See What’s Remembered** \
    _For example, just ask: “What do you remember about me?” to check your saved details._

**Note:** Turn off saved memories in your settings if you don’t want Doraverse to remember details for future chats, or use **Manage memories** to review, edit, or delete saved information.

<figure><img src="../.gitbook/assets/Screenshot 2025-08-29 at 17.06.50.png" alt=""><figcaption></figcaption></figure>

## Data Controls

<figure><img src="../.gitbook/assets/Screenshot 2025-08-29 at 17.20.30.png" alt=""><figcaption></figcaption></figure>

* **Import conversations from a JSON file**: Bring in saved conversations from another file or system.
* **Shared links (Manage)**: View and manage the links you’ve shared with others.
* **Revoke all user provided credentials**: For security, quickly remove any credential you’ve provided for integrations.
* **Delete TTS cache storage**: Clear the stored voice data from your device.

## Connected Apps

<figure><img src="../.gitbook/assets/Screenshot 2025-08-29 at 17.18.10.png" alt=""><figcaption></figcaption></figure>

The Connected Apps section is where you find and manage external tools that you have connected to Doraverse.

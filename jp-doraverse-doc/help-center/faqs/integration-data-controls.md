---
description: >-
  Learn how your data is accessed and used when you connect your apps to
  Doraverse.
icon: circle-nodes
---

# Integration - Data Controls

## **How does Doraverse connect to my apps?**

Doraverse connects via OAuth using Composio (our SOC 2 integration partner and sub-processor). OAuth lets you grant scoped, revocable access without sharing passwords.

## **Who is Composio and what do they do with my data?**

Composio is the integration platform that brokers OAuth, executes only the actions you request (e.g., read a Slack channel, create a Notion page), and returns results to Doraverse. You can review how Composio collects/uses data in their [Privacy Policy](https://composio.dev/privacy).

## **What data can Doraverse access from connected apps?**

We request only the minimum scopes you approve during OAuth (principle of least privilege).&#x20;

App’s toolkit and common actions via Composio:

<table><thead><tr><th width="92.77166748046875">App</th><th width="227.07586669921875">Toolkit and common actions</th><th width="235.5535888671875">Data categories</th><th>Example scopes</th></tr></thead><tbody><tr><td><strong>Gmail</strong></td><td>Connect mailboxes; send/read messages via toolkit actions.</td><td>Message metadata, message bodies/attachments you authorize; ability to send if write scope granted.</td><td><p><code>gmail.readonly</code></p><p><code>gmail.send</code></p></td></tr><tr><td><strong>Google Drive</strong></td><td>50+ actions (create/delete comments, create shortcuts, etc.).</td><td>File/folder metadata; file contents if read scopes enabled; write operations if granted.</td><td><p><code>drive.readonly</code></p><p><code>drive.file.picker</code> </p></td></tr><tr><td><strong>Google Docs</strong></td><td>Create/read/update documents via toolkit.</td><td>Document metadata &#x26; content for the docs you authorize.</td><td><code>documents</code><br><code>drive.file</code></td></tr><tr><td><strong>Google Slides</strong></td><td>Create/duplicate/update presentations.</td><td>Presentation metadata &#x26; slide content you authorize.</td><td><p><code>read.slide</code></p><p><code>edit.slide</code> </p></td></tr><tr><td><strong>Google Sheets</strong></td><td>Read/update spreadsheet ranges, etc.</td><td>Sheet metadata, cell values/ranges you authorize.</td><td><code>spreadsheets</code><br><code>drive.file</code></td></tr><tr><td><strong>Google Calendar</strong></td><td>Manage/read events.</td><td>Calendar lists, events (titles, times, attendees, etc.).</td><td><code>calendar</code><br><code>calendar.events</code></td></tr><tr><td><strong>Google Meet</strong></td><td>Connect Meet to coordinate meetings.</td><td>Meeting metadata (links, times) as permitted via Meet/Calendar scopes.</td><td><p><code>meetings.space.crea</code></p><p><code>calendar.events</code></p></td></tr><tr><td><strong>Slack</strong></td><td>Read channels/messages; post messages if enabled.</td><td>Channel list, messages in authorized channels; post capability if write scopes granted.</td><td><p><code>channels:history</code></p><p><code>chat:write</code></p></td></tr><tr><td><strong>Notion</strong></td><td>30+ actions; create/update pages &#x26; databases via MCP/tools.</td><td>Pages, databases, properties you share with the integration; schema metadata.</td><td>No string scopes; access is granted by sharing pages/databases to the integration)</td></tr><tr><td><strong>HubSpot</strong></td><td>Use CRM endpoints based on scopes you configure.</td><td>CRM objects you authorize (contacts, companies, deals, etc.).</td><td><p><code>crm.objects.contacts.write</code></p><p><code>crm.objects.deals.write</code></p></td></tr><tr><td><strong>GitHub</strong></td><td>800+ actions via MCP; issues, PRs, repos (read/write if enabled).</td><td>Repo metadata, issues/PR content; code if repo scope granted; write if requested.</td><td><p><code>repo</code></p><p><code>read:org</code></p></td></tr><tr><td><strong>Outlook</strong> </td><td>Outlook toolkit; additional scopes for OneDrive/Teams/SharePoint/Excel as needed.</td><td>Mail, calendar, files, teams/channels, etc.</td><td><code>Mail.Read</code>, <code>Calendars.Read</code></td></tr></tbody></table>

**📌 Please note:** Exact access = scopes you set in Composio's consent screen.

## **Does Doraverse use my data to train AI models?**

No. Content retrieved from connected apps is used to fulfill your requests only and is not used to train generalized models. (For Google connectors, even when “Improve the model for everyone” is ON, connector content isn’t used for training.)

## **Which AI/model providers process my data?**

Depending on the feature, Doraverse may route prompts/context to your chosen model/agent. We share only what’s necessary for the task. You can request our current sub-processor list at support@doraverse.com.

## **Can Doraverse act in my apps without me knowing?**

No. Any automated action (e.g., post to Slack, create a Notion page, comment on a GitHub PR) must be explicitly enabled by you per app and appears in your audit log.

## **How do I disconnect and revoke access?**

In Doraverse: **Navigate the chat bar → Manage Integrations**. Select the app you want to disconnect and click **Disconnect**. We immediately invalidate the OAuth token.

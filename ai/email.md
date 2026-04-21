---
title: AI-powered email clients <sub>Trends</sub>
---

<!-- TODO: add trends table -->

### Shortwave (Best for AI & Gmail Integration)

.. was built by ex-Google engineers specifically to modernize Gmail. It doesn't "import" your mail into a new service; it acts as a high-speed interface for your existing Google data.

Multi-Account: You can switch between or combine multiple Gmail accounts seamlessly in the web app.

AI Unsubscribe: It features a "Smarter Newsletters" bundle. It uses AI to identify frequent senders, group them, and offers a one-click Unsubscribe and Delete All feature for specific senders.

"Viewing" without Fetching: Because it is built directly on the Gmail API, it reflects your Gmail inbox in real-time. It doesn’t "move" your mail to a separate POP/IMAP server in the traditional sense; it’s a modern lens over your current inbox.

### Superhuman (Best for Power Users)

.. is a premium web/desktop client ($30/month) that emphasizes speed and AI.

Split Inbox: It uses AI to automatically categorize your mail (Newsletters, Social, Team).

Instant Unsubscribe: It has a famous "Cmd + U" (or Ctrl + U) shortcut that unsubscribes you from any list instantly.

Unified View: You can toggle between multiple Gmail accounts without the lag of traditional "fetching." It’s designed to feel like one unified workspace.

### Clean Email

.. is designed with a **"privacy-first"** architecture, meaning it purposefully avoids becoming a storage host for your actual messages.

Here is exactly where your data goes when you use it:

### 1. Your Email Content (Stays on Google)
Clean Email **does not download or store the body of your emails** on its servers.
* **The "Lense" Approach:** When you view an email in the Clean Email web app, it is fetching the content from Gmail’s servers in real-time. 
* **No Copying:** Unlike a traditional mail client (like Outlook) that creates a local copy of every email you've ever received, Clean Email only "looks" at the data to perform actions.

### 2. What they *do* store (Metadata)
To group your emails and suggest what to delete, they store **metadata** (information *about* the email), which includes:
* **Sender info:** Who sent the email (e.g., `newsletter@brand.com`).
* **Subject lines:** To help you identify the threads.
* **Timestamp/Size:** To help you find "Old" or "Large" emails.
* **Headers:** This is how their AI identifies "List-Unsubscribe" links.

### 3. Data Retention Policy (The 45-Day Rule)
In 2026, their policy remains strict regarding how long they keep even that metadata:
* **Automatic Deletion:** If you stop using the service or your subscription ends, all indexed metadata is automatically purged from their servers **45 days** after your last login.
* **OAuth Tokens:** They store encrypted "tokens" (keys) that allow them to talk to your Gmail account. You can revoke these at any time via your Google Account security settings, which immediately kills their access.

### 4. Security Audits
Because Clean Email connects to Gmail via the official API, they are subject to **Google’s Tier 2 Security Assessment**. This means an independent third party must audit their code and server infrastructure annually to ensure they aren't leaking or mishandling user data.

---

### Summary: Is it safe?
| Data Type | Stored on Clean Email? | Stored on Gmail? |
| :--- | :--- | :--- |
| **Email Text/Body** | **No** | Yes |
| **Attachments** | **No** | Yes |
| **Sender/Subject info** | Yes (Temporarily) | Yes |
| **Your Password** | **No** (Uses OAuth) | Yes |

**The Bottom Line:** Clean Email is a **controller**, not a **storage provider**. If Clean Email were to go out of business tomorrow, your emails would still be exactly where they started: safe in your Gmail account.

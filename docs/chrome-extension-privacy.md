# PufferGo Extension — Privacy Policy

**Last updated: June 24, 2026**

[中文版本 / Chinese Version](./chrome-extension-privacy-zh.html)

## Who We Are

PufferGo is a Chrome extension that helps foreign trade businesses build and manage WordPress websites. This Privacy Policy explains what data we collect, why, and how it is handled.

Developer contact: tech@puffergo.com

---

## What Data We Access and Why

### 1. Browsing Activity (Current Tab Only)

**What:** When you use the Block Clone tool, the extension captures a screenshot of the page you are currently viewing and extracts the HTML/CSS of the element you selected.

**Why:** This data is sent to our server (`api.puffergo.com`) solely to generate a matching WordPress block component for your site. It is not stored, indexed, or used for any other purpose.

**When:** Only when you actively click "Clone Block." The extension does not passively monitor your browsing.

---

### 2. Account and Authentication Data

**What:** When you connect your PufferGo account, a browser tab opens to puffergo.com where you log in. After authorization, an API key is returned to the extension and stored locally in Chrome storage.

**Why:** To verify your subscription and enable features tied to your account (AI generation credits, site management).

**What we receive on our servers:** Your PufferGo account ID and license key. We do not receive or store your Google credentials or browser passwords.

---

### 3. Third-Party API Credentials (Cloudflare, Hostinger, WordPress)

**What:** When you set up your website, you may enter API tokens for Cloudflare or Hostinger. These tokens are stored only in Chrome's local extension storage on your device.

**Why:** The extension uses these tokens to configure DNS, SSL, and hosting settings on your behalf through the providers' official APIs.

**Important:** These credentials never pass through PufferGo's servers. All API calls are made directly from your browser to the third-party provider.

---

### 4. Anonymous Usage Analytics (Optional, Opt-in)

**What:** If you choose to enable analytics, we collect anonymized event data: task started/completed/failed, duration, error category. No URLs, page content, personal identifiers, or browsing history are included.

**Why:** To improve extension reliability and understand which features are most useful.

**How:** We use PostHog with autocapture disabled. Each user is assigned a random anonymous ID. You can disable analytics at any time in the extension settings. Analytics is **off by default**.

---

### 5. Text Selection Translation (Disabled by Default)

**What:** When you enable the translation feature and select text on a webpage, the selected text along with page context (page title, description, and URL) is sent directly to the third-party LLM provider you have configured in the extension settings (e.g., OpenAI, Anthropic).

**Why:** To provide AI-powered translation of selected text into your chosen target language.

**When:** Only when you have manually enabled the translation feature in settings, and actively select text and click the translate button. The feature is **off by default** and must be explicitly turned on. No text is sent passively.

**Important:** Translation requests go directly from your browser to your configured LLM provider using your own API key. PufferGo's servers are not involved and never see your text.

---

## What We Do NOT Do

- We do not sell your data to any third party.
- We do not track your browsing history.
- We do not read your passwords, form inputs, or private messages.
- We do not use your data for advertising.
- We do not retain screenshot or HTML content after generating your block.

---

## Data Storage

| Data | Where Stored |
|------|-------------|
| Extension settings, API tokens, site config | Chrome local storage (on your device only) |
| PufferGo account session token | Chrome local storage (on your device only) |
| Anonymous analytics ID | Chrome local storage + PostHog (anonymized) |
| Screenshot / HTML sent for Block Clone | Transmitted to `api.puffergo.com`, not retained |

---

## Your Rights

You can delete all locally stored data by uninstalling the extension or clearing the extension's data in Chrome's extension settings. For any data held on our servers, contact tech@puffergo.com to request deletion.

---

## Changes to This Policy

We will update the "Last updated" date at the top of this page when changes are made. Significant changes will be communicated via the extension update notes.

---

## Contact

Lidafu · PufferGo  
tech@puffergo.com  
https://puffergo.com

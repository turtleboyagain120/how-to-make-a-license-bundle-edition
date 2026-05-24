# 📚 License School
## Everything About Software Licenses, Explained Like You Just Walked In Off the Street
### *From "What's a License?" to Full-On License Master — Zero Experience Required*

---

> **Hey, you.** Yes, you. You don't know anything about licenses yet. That's totally fine. By the end of this document, you're going to know more than most professional developers. Let's go.

---

# PAGE 1: What Even IS a License?

Okay. Imagine you drew the most amazing picture of a dragon. It took you three weeks. It's incredible.

Now your friend wants to put it on a t-shirt and sell it. Should they be allowed to? What if they sell 10,000 shirts and make $50,000 and give you nothing?

**That's why licenses exist.**

A **license** is just a set of rules you write down that tells everyone:
- ✅ What they're allowed to DO with your thing
- ❌ What they're NOT allowed to do
- 📋 What rules they have to follow IF they use it

That's it. That's the whole concept. You made something, and a license tells the world how they can use it.

Now apply that same idea to **software**. You wrote code. Maybe it took you five days. Maybe five years. A license is your document that says "here's what you can do with my code."

---

### The Three Magic Questions Every License Answers

Every single software license in existence — from the most freedom-loving open source license to the most locked-down corporate one — is really just answering three questions:

**1. Can you LOOK at the code?**
*(Can you read the source code, or is it a black box?)*

**2. Can you CHANGE the code?**
*(Can you modify it, remix it, make it your own?)*

**3. Can you SHARE the code?**
*(Can you give it to others, sell it, include it in your product?)*

How a license answers those three questions puts it into a category. Let's learn the categories.

---

# PAGE 2: The Three Worlds of Software Licenses

Think of software licenses like a neighborhood with three streets.

---

### 🟢 Street 1: Open Source Avenue

**Motto:** *"Here's the code. Take it. Change it. Share it. Just follow the rules."*

On Open Source Avenue, the source code is available to everyone. You can read it, change it, and usually share it. The rules vary — some streets are more strict than others — but the core idea is: **the code is open.**

This is where stuff like Linux, Firefox, and VLC lives.

---

### 🟡 Street 2: Source Available Boulevard

**Motto:** *"You can SEE the code, but you can't always DO whatever you want with it."*

This is the sneaky middle ground a lot of people don't know about. The code is visible — you can read it, study it, maybe even use it for free personally — but the license has **specific restrictions**, usually around commercial use.

Companies love this because it lets developers trust them ("see, we're not hiding anything!") while protecting their business ("but you can't just clone us and compete with us").

---

### 🔴 Street 3: Proprietary Place

**Motto:** *"You get the app. The code? That's ours. Here are the rules. Read them before you click 'I Agree.'"*

This is where Microsoft Office, Adobe Photoshop, and most commercial software lives. You get a binary (the program), not the source. The license (called a **EULA** — we'll get there) tells you what you can do with that binary.

---

Okay, now let's go deep on each one. Get comfy.

---

# PAGE 3: Open Source Licenses — The Full Breakdown

Before we talk specific licenses, you need to understand one more concept: **Copyleft vs. Permissive.**

### Permissive Licenses 🕊️
*"Do whatever you want. Just give me credit."*

Permissive licenses are basically the nicest, most chill licenses in existence. You can take the code, modify it, put it in a commercial product, even make it closed source — as long as you include the original copyright notice. That's mostly it.

### Copyleft Licenses 🔄
*"Do whatever you want — BUT if you share your version, it has to use the same license."*

Copyleft licenses have a "viral" quality. If you use copyleft code and distribute your software, your software has to become open source too (under the same or compatible license). The idea is to keep code free forever — you can't take open source code and make it proprietary.

Now let's meet every major license.

---

## 🏆 MIT License
**Vibe:** The friendliest license ever made.
**Type:** Permissive
**Age:** 1988

**What it says in plain English:**
> "Use this. Change this. Sell this. Put it in anything. Just keep my name on it."

**What you can do:**
- ✅ Use commercially
- ✅ Modify
- ✅ Distribute
- ✅ Use privately
- ✅ Sublicense (hand it off with new rules)

**What you MUST do:**
- 📋 Include the original MIT license text and copyright notice in your software

**What you CANNOT do:**
- ❌ Hold the original author liable if something breaks

**Best for:** Small libraries, tools, anything you want the world to use freely.

**Famous MIT projects:** React, Rails, jQuery, .NET

**Imagine it like:** A chef who posts their recipe online and says "cook it, sell it, call it your own — just mention where you got the recipe."

---

## 🦅 Apache License 2.0
**Vibe:** MIT's more corporate, legally-careful cousin.
**Type:** Permissive
**Age:** 2004

**What it says in plain English:**
> "Use this freely. Just give credit, say what you changed, and don't use our name to promote your stuff. Oh, and we're giving you patent protection."

**The big deal about Apache 2.0:** It includes an **explicit patent grant**. This means if the original contributors hold patents related to the code, they're giving you a license to use those patents too. MIT doesn't do this. This matters a LOT in corporate environments.

**What you can do:**
- ✅ Everything MIT lets you do
- ✅ Patent protection from contributors

**What you MUST do:**
- 📋 Include the license and copyright notice
- 📋 State what changes you made
- 📋 Include a NOTICE file if one exists

**What you CANNOT do:**
- ❌ Use contributors' names/logos to endorse your product
- ❌ Hold contributors liable

**Best for:** Bigger projects, corporate use, anything where patents might be a concern.

**Famous Apache 2.0 projects:** Android, Kubernetes, TensorFlow, Swift

---

## ⚖️ GNU GPL v2 & v3
**Vibe:** The freedom fighter. The enforcer. The license with opinions.
**Type:** Strong Copyleft
**Age:** v2 in 1991, v3 in 2007

**What it says in plain English:**
> "This software is free. If you use it and distribute something, that something must ALSO be free. Freedom must spread."

GPL is the most famous copyleft license. It was created by Richard Stallman (the godfather of free software) with a specific philosophy: software freedom should be viral. If you take free code, you can't make it unfree.

**GPL v2 vs v3 — What's different?**

| Thing | GPL v2 | GPL v3 |
|---|---|---|
| Tivoization | Not addressed | **Banned** |
| Patent retaliation | Not addressed | **Included** |
| License compatibility | Limited | Better |
| Digital locks (DRM) | Not addressed | **Addressed** |

*Tivoization* = when a company uses GPL code but locks the hardware so you can't actually run modified versions. GPL v3 explicitly bans this. (TiVo, the DVR company, did exactly this — hence the name.)

**What you can do:**
- ✅ Use, study, modify, distribute

**What you MUST do:**
- 📋 Release source code when you distribute
- 📋 Use GPL for your whole project
- 📋 Include license text

**What you CANNOT do:**
- ❌ Make it proprietary
- ❌ Add extra restrictions

**Best for:** OS projects, tools where you WANT to enforce openness.

**Famous GPL projects:** Linux kernel (v2), WordPress, VLC (v2), GIMP

**The catch:** Many companies avoid GPL code because it can "infect" their proprietary product. This is intentional by design.

---

## 🔗 GNU LGPL (Lesser GPL)
**Vibe:** GPL's more business-friendly little sibling.
**Type:** Weak Copyleft
**Age:** 1991

**The Problem LGPL Solves:**
Regular GPL says "if your program uses this code, your WHOLE program must be GPL." That scared away companies from using free libraries. So LGPL was created with a compromise.

**What it says in plain English:**
> "You can link to this library in your proprietary software. But if you CHANGE the library itself, those changes must stay open."

**The key distinction:**
- Modified the LGPL library? → Must release those changes under LGPL
- Just used the LGPL library in your app? → Your app can stay proprietary

**Best for:** Libraries you want everyone (including commercial devs) to use.

**Famous LGPL projects:** GNU C Library, Qt (partially), GTK

---

## ☁️ GNU AGPL v3 (Affero GPL)
**Vibe:** GPL but it closes the "SaaS loophole."
**Type:** Strong Copyleft (Strongest of all)
**Age:** 2007

**The Problem AGPL Solves:**
Regular GPL says "if you DISTRIBUTE the software, you must release the source." But what if you run the software on a server and let people use it over the internet? You're not distributing it — you're just serving it. So GPL doesn't apply. Companies exploit this loophole.

**AGPL closes that loophole.**

**What it says in plain English:**
> "If anyone can interact with this software over a network — even just using your website — you must make the source code available."

**Best for:** Web apps, SaaS tools, anything server-side where you want to enforce openness.

**Famous AGPL projects:** MongoDB (old), Nextcloud, Mastodon

**The catch:** Even scarier to companies than regular GPL. If you run AGPL code on your server, your whole application might need to be AGPL.

---

## 🧩 Mozilla Public License 2.0 (MPL)
**Vibe:** The reasonable middle ground between permissive and copyleft.
**Type:** Weak Copyleft (File-level)
**Age:** 2012

**What makes MPL unique:**
Copyleft applies **file by file**, not to your whole project. If you modify an MPL file, that file must stay MPL. But you can combine MPL files with proprietary files in the same project.

**What it says in plain English:**
> "The files you got from us stay open if you change them. But you can use them alongside your proprietary code."

**Best for:** Projects that want some copyleft protection but need to be usable in mixed codebases.

**Famous MPL projects:** Firefox, LibreOffice (partly)

---

## 🍺 BSD Licenses (2-Clause and 3-Clause)
**Vibe:** Almost identical to MIT. Slightly older.
**Type:** Permissive
**Age:** 1980s

**2-Clause BSD ("Simplified BSD"):**
Almost exactly like MIT. Keep the copyright notice. Don't blame us.

**3-Clause BSD ("New BSD"):**
Adds one rule: don't use the project's name to endorse your stuff without permission.

**Why does BSD exist if MIT is basically the same?**
History. BSD came from Berkeley's Unix in the 80s. MIT came from MIT. They're practically twins.

**Best for:** System software, anything with a Unix heritage.

**Famous BSD projects:** FreeBSD, OpenBSD, PostgreSQL, nginx

---

## 🪶 ISC License
**Vibe:** MIT but even shorter.
**Type:** Permissive
**Age:** 1995

Functionally identical to MIT. Preferred by some for being even more concise. Just two rules: keep the copyright notice, don't blame us.

**Famous ISC projects:** OpenBSD (parts), many Node.js packages

---

# PAGE 4: Source Available Licenses — The In-Between Zone

These licenses are NOT considered open source by the Open Source Initiative (OSI). But they're not fully closed either. Welcome to the gray zone.

---

## ⏱️ Business Source License (BSL / BUSL)
**Creator:** MariaDB (now widely adopted)
**Vibe:** "Free now, open source later."

**The genius idea:** Your software starts with restrictions. After a set amount of time (usually 4 years), it automatically converts to an open source license.

**What it says in plain English:**
> "You can use this for free — but not commercially, or at least not beyond a certain scale. In 4 years, it automatically becomes Apache 2.0."

**What you can do (typically):**
- ✅ Use for free non-commercial projects
- ✅ Study the code
- ✅ Modify for personal use

**What you CANNOT do:**
- ❌ Use commercially beyond defined limits without a paid license
- ❌ Compete directly with the original project

**Best for:** Companies that want transparency and trust but also need to protect their business from being cloned by AWS or Google.

**Famous BSL projects:** HashiCorp tools (Terraform, Vault), MariaDB

---

## 🌊 SSPL (Server Side Public License)
**Creator:** MongoDB
**Vibe:** AGPL with teeth — so sharp MongoDB was kicked out of Debian.

**What it says in plain English:**
> "If you offer this software as a service, you must open source EVERYTHING needed to run that service — not just this code, but all your management code, monitoring, everything."

This was created directly because Amazon launched "Amazon DocumentDB" (basically a MongoDB clone) as a paid cloud service without contributing back.

**The controversy:** Most open source advocates consider SSPL too restrictive to be true open source. OSI rejected it. But the point was clear: "You won't out-Amazon us again."

**Famous SSPL projects:** MongoDB, Redis (briefly before switching back)

---

## ⚖️ Fair Source License
**Vibe:** "Small teams use it free. Big companies pay."
**Age:** Very new (2024)

**What it says in plain English:**
> "You can use this free if your company has fewer than X employees (often 25 or 50). After that, you need a commercial license."

This is gaining traction as a way for small dev shops to keep the lights on while still sharing code openly with the indie developer community.

**Best for:** Solo devs or small teams who want to be open but also eat food.

---

## 🔐 Commons Clause
**Not a full license — it's an ADD-ON** you bolt onto another license (like Apache 2.0).

**What it adds in plain English:**
> "Everything in the original license still applies — EXCEPT you can't sell this software or a substantially similar service."

Redis briefly added Commons Clause to some of its modules. This upset many open source people because it retroactively changed terms.

**Lesson:** Adding Commons Clause to an OSI-approved license makes it no longer open source. Be upfront about that.

---

# PAGE 5: Proprietary Licenses & EULAs

Now we enter the world of "software you buy, use, but never own."

---

## 📜 What is a EULA?

**EULA = End User License Agreement**

It's the thing you click "I Agree" on without reading. (Don't feel bad. Nobody reads them. A study found it would take 76 work days per year to read every privacy policy and EULA you encounter.)

But here's the thing: **they're legally binding.** When you click "I Agree," you're entering a contract.

---

### What a EULA Typically Contains:

**1. Grant of License**
"We give you permission to install and use this software."
Note: You're not buying the software. You're buying a *license to use* the software. There's a big difference. That's why you can't legally resell most software.

**2. Restrictions**
- Don't reverse engineer it
- Don't copy it
- Don't rent or lend it
- Often: don't use it to compete with us

**3. Ownership**
"This software belongs to us. Always."

**4. Termination**
"If you break these rules, your license is revoked. Immediately."

**5. Disclaimer of Warranties**
"This software is provided AS IS. If it deletes your files, crashes your server, or somehow burns your house down — not our problem."
*(Written in ALL CAPS in real EULAs, which is legally significant — it signals the user was warned)*

**6. Limitation of Liability**
Even if we're negligent, we owe you at most $X (often just what you paid).

**7. Governing Law**
"Legal disputes happen in [State/Country] under [State/Country] law."

---

### How to Write a Simple EULA for Your Own Software:

Here's the basic structure you need:

```
[YOUR SOFTWARE NAME] — End User License Agreement
Last Updated: [DATE]

1. LICENSE GRANT
   [Company/Your Name] grants you a non-exclusive, non-transferable, 
   limited license to install and use [Software] for [personal/commercial] 
   purposes.

2. RESTRICTIONS
   You may not:
   - Copy, modify, or distribute the software
   - Reverse engineer or decompile it
   - Sublicense or resell it

3. OWNERSHIP
   [Software] and all copies are owned by [Company Name].

4. TERMINATION
   This license terminates immediately upon any breach.

5. DISCLAIMER
   THE SOFTWARE IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND.

6. LIMITATION OF LIABILITY
   In no event shall [Company] be liable for any damages exceeding 
   the amount paid for the software.

7. GOVERNING LAW
   This Agreement is governed by the laws of [State/Country].
```

That's the skeleton. Real EULAs are longer, but they're all just expansions of this.

---

# PAGE 6: Privacy Policies — The Other Document Everyone Ignores

Privacy policies and licenses are different things, but they live in the same "legal stuff" neighborhood, so we're covering them here.

---

## What Is a Privacy Policy?

A privacy policy tells users:
- What data you collect about them
- Why you collect it
- What you do with it
- Who you share it with
- How they can control it

---

## Why Do You NEED One?

It's not optional. Multiple laws around the world require it:

| Law | Where | What it requires |
|---|---|---|
| **GDPR** | European Union | Very strict. Consent required. Right to delete. Heavy fines. |
| **CCPA** | California, USA | Right to know, delete, opt-out of sale |
| **COPPA** | USA (kids) | Must protect children under 13 |
| **PIPEDA** | Canada | Consent-based data collection |
| **LGPD** | Brazil | Similar to GDPR |

If your app has users in the EU — even one user — GDPR applies to you. The fines can be up to **4% of global annual revenue** or €20 million, whichever is higher. This is not a joke.

---

## What Every Privacy Policy Needs:

**1. What you collect**
Be specific. "Name, email, IP address, usage data, device type, cookies..."

**2. How you collect it**
"When you sign up, when you use the app, via cookies, via analytics tools..."

**3. Why you collect it**
"To operate the service, improve it, send you emails, comply with laws..."

**4. Who you share it with**
"We may share data with: payment processors, email providers, analytics services, law enforcement if required..."

**5. How long you keep it**
"We retain data for X days/years, or until you delete your account."

**6. User rights**
"You have the right to: access your data, correct it, delete it, export it, opt out of marketing..."

**7. Cookies section**
"We use cookies for: authentication, analytics, preferences..."

**8. Children's policy**
"We do not knowingly collect data from children under 13."

**9. Changes to the policy**
"We'll notify you if we change this policy."

**10. Contact information**
How users can reach you with privacy questions.

---

## Free Tools to Generate One:

- **Termly.io** — Generates GDPR/CCPA compliant policies
- **Iubenda** — Very popular, auto-updates for new laws
- **PrivacyPolicies.com** — Good free generator

For anything serious/commercial: hire a lawyer. Privacy law fines are real.

---

# PAGE 7: License Compatibility — Can They Work Together?

This is where things get spicy. When you build a project, you're often combining code from multiple sources with different licenses. Not all licenses play nice together.

---

## The Golden Rule of License Compatibility:

**The more restrictive license usually wins.**

If you combine MIT code with GPL code and distribute it, the whole thing becomes GPL. You can't make it less free than the most restrictive component.

---

## Compatibility Quick Reference Chart:

| Your Project License | Can Use MIT? | Can Use Apache 2.0? | Can Use GPL v2? | Can Use GPL v3? | Can Use AGPL? |
|---|---|---|---|---|---|
| **MIT** | ✅ | ✅ | ❌ | ❌ | ❌ |
| **Apache 2.0** | ✅ | ✅ | ❌ | ❌ | ❌ |
| **GPL v2** | ✅ | ❌* | ✅ | ❌ | ❌ |
| **GPL v3** | ✅ | ✅ | ❌* | ✅ | ❌ |
| **AGPL v3** | ✅ | ✅ | ❌* | ✅ | ✅ |
| **Proprietary** | ✅ | ✅ | ❌ | ❌ | ❌ |

*The Apache 2.0/GPL v2 incompatibility is a famous problem. Apache 2.0 has patent termination clauses that technically conflict with GPL v2. GPL v3 was partly designed to fix this.

---

## Real-World Compatibility Examples:

**Scenario 1: You're building a mobile app**
- You use React (MIT) ✅
- You use a library under Apache 2.0 ✅
- You want to keep your app proprietary ✅
- *Result: Totally fine. MIT and Apache 2.0 are permissive — no infection.*

**Scenario 2: You're building a desktop tool**
- You use MIT code ✅
- You decide to include a GPL v3 plugin
- You distribute the software
- *Result: Your whole distributed app must now be GPL v3. You MUST release your source code.*

**Scenario 3: You're running a SaaS**
- You use AGPL code on your server
- Users interact with it over the web
- *Result: You must publish your entire application's source code. AGPL network use clause triggers.*

---

# PAGE 8: How to Actually Apply a License to YOUR Project

Okay. You've picked a license. Now what? Here's the exact how-to.

---

## Step 1: Choose Your License

Use this decision tree:

```
Do you want anyone to use your code freely?
├── YES → Do you want commercial use allowed?
│   ├── YES → Do you care about patents?
│   │   ├── YES → Apache 2.0
│   │   └── NO → MIT or BSD
│   └── NO → Consider BSL or Fair Source
└── NO (you want to enforce openness)
    ├── Are you building a library?
    │   └── YES → LGPL
    ├── Is it a web app/SaaS?
    │   └── YES → AGPL
    └── Is it a general tool/OS software?
        └── YES → GPL v3
```

---

## Step 2: Create Your LICENSE File

In the root of your project, create a file named exactly `LICENSE` (no extension) or `LICENSE.txt`.

Go to **choosealicense.com**, pick your license, and copy the full text. Replace:
- `[year]` with the current year
- `[fullname]` with your name or organization name

That's it. Your repo is now licensed.

---

## Step 3: Add a Header to Your Source Files (Optional but Recommended)

For GPL projects especially, add a short comment at the top of each source file:

```
/*
 * MyProject - A description of what it does
 * Copyright (C) 2025 Your Name
 *
 * This program is free software: you can redistribute it and/or modify
 * it under the terms of the GNU General Public License as published by
 * the Free Software Foundation, either version 3 of the License.
 */
```

For MIT/Apache, a shorter header works:

```
// Copyright (c) 2025 Your Name. Licensed under the MIT License.
```

---

## Step 4: Add a Badge to Your README

On GitHub, add a license badge so people immediately know:

```markdown
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)
![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)
```

---

## Step 5: Specify in Package Files

If you have a package.json, pyproject.toml, or similar:

```json
// package.json
{
  "license": "MIT"
}
```

```toml
# pyproject.toml
[project]
license = {text = "Apache-2.0"}
```

---

## Step 6 (For GitHub): Set It During Repo Creation

GitHub lets you pick a license when you create a repo. It automatically creates your LICENSE file. Use it.

---

# PAGE 9: Rookie Mistakes — Don't Be That Developer

These are the most common license mistakes people make. Now you won't.

---

### ❌ Mistake 1: No License = "Free to Use"

**WRONG. So, so wrong.**

No license means the default copyright law applies. That means **only you** can use, copy, or distribute the code. A project with no license is actually MORE restricted than a GPL project. Nobody can legally use it at all.

If you want people to use your code, you MUST add a license.

---

### ❌ Mistake 2: "I'll Just Use GPL Code in My Commercial App"

GPL code in a distributed proprietary app forces the whole app to be GPL. Either:
- Use MIT/Apache alternatives
- Actually release your app under GPL
- Get a commercial license from the copyright holder (many GPL projects offer dual licensing)

---

### ❌ Mistake 3: Changing Someone Else's License

You cannot change the license on code you didn't write. If someone released code under GPL, you can't redistribute it under MIT. You can only add MORE restrictions or contribute back under the same license. You can't grant rights you don't have.

---

### ❌ Mistake 4: "It's on GitHub So It's Open Source"

GitHub is a hosting platform. Public visibility ≠ open source license. See Mistake #1.

A public GitHub repo with no LICENSE file is NOT open source. You're just letting people read the code. They cannot legally use it.

---

### ❌ Mistake 5: Forgetting AGPL When Running SaaS

If you use AGPL code in your web application, every user who interacts with your service is entitled to the source code. Many startups have been caught off-guard by this. Always check licenses before you import.

---

### ❌ Mistake 6: Copying Code Without Checking the License

That Stack Overflow snippet, that GitHub gist, that blog post with code — all of it has a license. Stack Overflow uses CC BY-SA 4.0, which has copyleft implications. Always check.

---

### ❌ Mistake 7: Writing Your Own License

Resist the urge. Custom licenses create legal uncertainty. Nobody's lawyers have reviewed it. Major package managers and companies will refuse to use your code. Pick a well-known license. Your cool custom wording is not worth it.

---

### ❌ Mistake 8: Ignoring the Patent Clause Difference

MIT has no patent clause. Apache 2.0 does. If you're in a patent-heavy industry (big tech, medical software, etc.), always use Apache 2.0 or GPL v3 — both have explicit patent grants and retaliation clauses that protect you.

---

# PAGE 10: The Master Cheat Sheet 🏆

You made it. Here's everything compressed into one reference page.

---

## License Quick Reference

| License | Type | Commercial? | Copyleft? | Patent? | Best For |
|---|---|---|---|---|---|
| **MIT** | Permissive | ✅ | ❌ | ❌ | Libraries, tools, anything |
| **Apache 2.0** | Permissive | ✅ | ❌ | ✅ | Corporate projects, anything with patents |
| **BSD 2/3-Clause** | Permissive | ✅ | ❌ | ❌ | System software |
| **ISC** | Permissive | ✅ | ❌ | ❌ | Tiny libraries |
| **GPL v2** | Copyleft | ✅ | ✅ (strong) | ❌ | Linux-era OS software |
| **GPL v3** | Copyleft | ✅ | ✅ (strong) | ✅ | Modern OS software |
| **LGPL** | Copyleft | ✅ | ✅ (weak) | ✅ | Libraries used in proprietary apps |
| **AGPL v3** | Copyleft | ✅ | ✅ (strongest) | ✅ | Web apps/SaaS |
| **MPL 2.0** | Copyleft | ✅ | ✅ (file-level) | ✅ | Mixed codebases |
| **BSL** | Source Available | ⚠️ | ❌ | ❌ | Startups protecting revenue |
| **SSPL** | Source Available | ⚠️ | ✅ (nuclear) | ❌ | Cloud-hostile protection |
| **Fair Source** | Source Available | ⚠️ | ❌ | ❌ | Small team freemium |

*⚠️ = allowed within limits*

---

## One-Line Summaries

- **MIT:** "Do anything, just keep my name."
- **Apache 2.0:** "Do anything, keep my name, you get patent protection."
- **GPL v3:** "You can use this, but what you make must also be free."
- **AGPL v3:** "GPL, but the web counts as distributing."
- **LGPL:** "Link to my library freely, but share changes to the library."
- **MPL:** "Changed files stay open, but your project can be proprietary."
- **BSL:** "Free for now, business pays, converts to open source in 4 years."
- **SSPL:** "Use this as a service? Open source EVERYTHING."
- **EULA:** "You don't own this. Here are the rules. Click I Agree."
- **Privacy Policy:** "Here's everything we collect and why. Required by law."

---

## The 5 Rules to Never Break

1. **Always license your code.** No license = nobody can legally use it.
2. **Check licenses before you use dependencies.** One GPL package can change everything.
3. **MIT/Apache for "use freely." GPL for "stay free."** Pick based on philosophy.
4. **AGPL if you run a web service** and want your code to stay open.
5. **Never write your own license.** Use a standard one. Always.

---

## Useful Resources

- **choosealicense.com** — GitHub's plain-English license picker
- **tldrlegal.com** — Summarizes every license in human language
- **spdx.org/licenses** — The official master list of all licenses
- **gnu.org/licenses** — Free Software Foundation's license explanations
- **opensource.org/licenses** — OSI-approved license list
- **iubenda.com** / **termly.io** — Privacy policy generators

---

*You now know more about software licenses than most working developers. Go build something great — and license it properly.* 🚀

---
*Document written in plain English for absolute beginners. Not legal advice. For anything involving real legal risk, consult an actual attorney.*

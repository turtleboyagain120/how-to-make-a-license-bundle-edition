# ⚖️ License Vocab & Activity Workbook
## Words to Remember, Phrases to Use, and How to Fix Every Beginner Mistake
### *Your Pocket Reference for Writing Licenses Like You've Done It For Years*

---

> **How to use this book:**
> Read a word. Say the definition out loud. Read the phrase. Then do the activity at the end of each page. By page 5 you'll catch mistakes that trip up real lawyers.

---

# PAGE 1: The Grant Words
## The Words That Give People Permission

These are the words that appear in the **Grant section** of every license — the part where you actually give someone permission to do something. Get these wrong and your license either gives away too much or nothing at all.

---

### 📖 WORD 1: Grant
**Definition:** The act of officially giving someone a right or permission. In a license, the grant is the moment you hand over the keys.

**When to use it:** Every single license needs a grant section. Without it, there's no permission given and nobody can legally use anything.

**The phrase:**
> *"Licensor hereby grants You a license to..."*

**Never say instead:** "You can use this" or "Feel free to use this." Courts don't love casual language. "Hereby grants" is tested, trusted, and unambiguous.

**Beginner mistake:** Writing a license with only restrictions and no grant. This is shockingly common. A document that only says "you can't do X, Y, Z" but never says "you CAN do A, B, C" gives the user no rights at all. Always lead with what they CAN do.

**Fix it:** Before writing a single restriction, write your grant first. Ask "what am I actually giving them?" and write that down fully. Then add the limits.

---

### 📖 WORD 2: Perpetual
**Definition:** Lasting forever, or until terminated for cause. No expiration date.

**When to use it:** Open source licenses. Any time you want someone to use your code without having to renew anything.

**The phrase:**
> *"...a perpetual, worldwide, royalty-free license..."*

**The opposite:** A **term license** or **subscription license** — expires after a set time (1 year, monthly, etc.). Used in SaaS and commercial software.

**Beginner mistake:** Forgetting to include "perpetual" in an open source license. This creates ambiguity — does the license expire? For how long? In court, ambiguity is your enemy.

**Fix it:** In any OSS license, always write the full stack: *"perpetual, worldwide, royalty-free, non-exclusive, irrevocable."* These five words travel together. Learn them as a unit.

---

### 📖 WORD 3: Irrevocable
**Definition:** Cannot be taken back. Once granted, it's granted forever regardless of what the licensor later decides.

**When to use it:** Open source licenses where you need developers to trust that the license won't be yanked tomorrow.

**The phrase:**
> *"...an irrevocable license to use, copy, modify, and distribute..."*

**When NOT to use it:** EULAs and proprietary software. You WANT the ability to revoke in those cases (if someone violates terms, you need to be able to terminate).

**Beginner mistake:** Using "irrevocable" in a EULA by accident. Now you can never terminate the license even if the user violates every term.

**Fix it:** Simple rule — *irrevocable belongs in OSS licenses. EULAs and commercial licenses get a termination clause instead.*

---

### 📖 WORD 4: Non-Exclusive
**Definition:** You're giving this same license to everyone — not just this one person. You can give the same rights to a thousand different people.

**When to use it:** Almost always. It means you still own the copyright and can license to others.

**The opposite:** An **exclusive license** — you give rights to ONE person or company and nobody else. Used in high-dollar business deals. Rare in software.

**The phrase:**
> *"...a non-exclusive license, meaning Licensor may grant similar rights to others..."*

**Beginner mistake:** Not including "non-exclusive" and accidentally implying the user has exclusive rights to your code. A company could argue you promised them the only license.

**Fix it:** Always write "non-exclusive" in your grant. It protects you.

---

### 📖 WORD 5: Sublicense
**Definition:** The right to pass your license rights on to a third party. If you can sublicense, you can let someone else use it under similar terms.

**When to use it:** Permissive licenses (MIT, Apache) where you want the code to flow freely through the ecosystem.

**When NOT to use it:** Copyleft licenses. GPL explicitly does NOT allow sublicensing — everyone must get their rights directly from the original GPL, not from you.

**The phrase:**
> *"...including the right to sublicense the Software to third parties..."*

**Beginner mistake:** Including sublicense rights in a copyleft license. Now your users can pass your code to people without enforcing the copyleft condition.

**Fix it:** Permissive license? Include sublicense. Copyleft license? Remove it and say "All rights under this license flow directly from the original licensor."

---

### ✏️ PAGE 1 ACTIVITY: Fill in the Grant

Below is a broken grant section. Fill in the five missing words from Page 1.

```
Licensor hereby ________ You a ________, worldwide, 
royalty-free, ________, ________ license to use, copy, 
modify, merge, publish, distribute, and ________ 
the Software.
```

*(Answers: grants / perpetual / non-exclusive / irrevocable / sublicense)*

**Bonus:** Now write your own grant section for a photo-editing app you made. Make it permissive. Include all five words from this page.

---

# PAGE 2: The Restriction Words
## The Words That Put Up Walls

These words appear in the **Restrictions section** — the part of a license that tells people what they absolutely cannot do. These words need to be precise. A vague restriction is an unenforceable restriction.

---

### 📖 WORD 6: Derivative Work
**Definition:** Any new work that is based on or derived from an existing work. If you take someone's code and modify it, your result is a derivative work of the original.

**When to use it:** Any copyleft license. Also important in EULA restrictions.

**The phrase:**
> *"Any Derivative Work must be distributed under the same terms as this License."*
> *"You may not create Derivative Works for commercial purposes without written permission."*

**Why it matters:** The definition of "derivative" is where most copyleft license fights happen. Is a program that merely *links* to a GPL library a derivative work? (Famously contested. LGPL exists specifically to answer this question.)

**Beginner mistake:** Using "Derivative Work" without defining it. Courts and lawyers will fight over whether something counts.

**Fix it:** In your Definitions section, write exactly what counts:
> *"'Derivative Work' means any work that incorporates, modifies, translates, or is otherwise based on the Software, including works that link to it at compile time."*

---

### 📖 WORD 7: Reverse Engineer
**Definition:** The process of taking a finished binary (compiled program) and working backward to figure out how it works — essentially reconstructing the source code.

**When to use it:** Every proprietary EULA. If your source code is secret, you must ban reverse engineering.

**The phrase:**
> *"You may not reverse engineer, decompile, disassemble, or otherwise attempt to derive the source code of the Software."*

**Notice the list:** reverse engineer, decompile, disassemble. These are three different technical methods of doing essentially the same thing. Always list all three — if you only ban one, someone will argue the other two are permitted.

**Beginner mistake:** Only writing "you may not reverse engineer" without including decompile and disassemble.

**Fix it:** Copy the full phrase above. All three words, every time.

---

### 📖 WORD 8: Competing Use / Competing Product
**Definition:** Using the licensed software to build or operate a product or service that competes directly with the licensor's business.

**When to use it:** Source available licenses, BSL-style licenses, commercial licenses where you want to block the "clone and compete" threat.

**The phrase:**
> *"You may not use the Software to develop, operate, or offer a product or service that provides substantially similar functionality to Licensor's commercial offerings."*

**Why "substantially similar" matters:** You can't ban ALL competition — that's too broad and may be unenforceable. "Substantially similar functionality" is the right scope.

**Beginner mistake:** Writing "you can't compete with us" — too vague. What counts as competing? A company could argue their slightly different product doesn't compete.

**Fix it:** Be specific. List your product names. Define what "compete" means:
> *"'Competing Use' means operating a hosted service that offers database query building features substantially similar to QueryFlow Cloud."*

---

### 📖 WORD 9: Notwithstanding
**Definition:** "Even though" or "regardless of." Used to create an exception to something you already said.

**When to use it:** When you have a general rule but need to carve out a specific exception without rewriting everything above it.

**The phrase:**
> *"Notwithstanding the restrictions above, You may use the Software for personal, non-commercial evaluation purposes for a period not to exceed 30 days."*

**The 4th-grade version:** "I said no cookies. Notwithstanding that rule, you may have one cookie on your birthday."

**Beginner mistake:** Not using "notwithstanding" and instead trying to rewrite earlier sections to add exceptions. This creates contradictions and confusion.

**Fix it:** Any time you need an exception to a rule you already wrote, start the exception with "Notwithstanding [section number or reference above]..."

---

### 📖 WORD 10: Indemnify / Indemnification
**Definition:** A promise to pay for damages or legal costs that arise from someone else's actions. If you agree to indemnify someone, you're agreeing to pay their legal bills if something you did causes them to get sued.

**When to use it:** Commercial licenses, EULAs, and enterprise agreements. Less common in OSS licenses.

**The phrase:**
> *"You agree to indemnify, defend, and hold harmless Licensor from and against any claims, liabilities, damages, losses, and expenses arising from Your use of the Software or Your violation of this Agreement."*

**Notice "indemnify, defend, AND hold harmless"** — three words that together cover: pay for it, fight it in court, and don't drag us into it.

**Beginner mistake:** Writing only "hold harmless" and missing "indemnify" and "defend." Courts treat these as slightly different obligations. Use all three.

**Fix it:** Copy the full phrase. It's standard boilerplate for a reason.

---

### ✏️ PAGE 2 ACTIVITY: The Restriction Rewrite

Below is a restrictions section from a fictional EULA. It has four problems. Find them and rewrite each broken sentence.

```
You can't copy this app. Don't figure out how it works 
on the inside. Don't compete with us. If something bad 
happens because of you, you pay for it.
```

**Problems to find:**
1. "Copy this app" — what exactly counts as copying? (Backup copies? Screenshots?)
2. "Figure out how it works on the inside" — missing the three technical terms
3. "Don't compete with us" — needs definition of "compete"
4. "If something bad happens because of you, you pay for it" — missing all three indemnification words

Write a corrected version of all four sentences using the vocabulary from this page.

---

# PAGE 3: The Disclaimer Words
## The Words That Protect You From Getting Sued

This is the least glamorous part of a license but arguably the most important for you personally. The disclaimer section is what stands between you and a lawsuit when someone uses your code and something goes wrong.

---

### 📖 WORD 11: Warranty
**Definition:** A promise that something will work correctly or meet a certain standard. When you disclaim warranties, you're saying "we make no promises about quality."

**Two types that always appear together:**

**Express warranty** = a promise you actually stated out loud or in writing.
**Implied warranty** = a promise the law assumes you made, even if you said nothing.

**The phrase:**
> *"THE SOFTWARE IS PROVIDED 'AS IS' WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED."*

**Why "AS IS" matters:** This two-word phrase has specific legal meaning. Courts understand it to mean the buyer accepts the product in its current condition with no guarantees. Always include it.

**Beginner mistake:** Only disclaiming express warranties and forgetting implied ones. Implied warranties exist by default in many jurisdictions. You must explicitly disclaim them.

**Fix it:** Always write "express or implied" together. Never one without the other.

---

### 📖 WORD 12: Merchantability
**Definition:** A legal warranty that a product is fit for the ordinary purpose for which it is used. It's the law's assumption that if you sell something, it basically works.

**When to use it:** Always, in your disclaimer. You're disclaiming it — not granting it.

**The phrase:**
> *"...INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT."*

**These three always travel together:**
- **Merchantability** — it works for normal use
- **Fitness for a particular purpose** — it works for YOUR specific use
- **Noninfringement** — it doesn't violate someone else's patents or copyrights

**Beginner mistake:** Writing a disclaimer without all three. Leaving out "fitness for a particular purpose" means a user could argue you warranted that it works for their specific use case.

**Fix it:** Copy-paste the full three-part disclaimer phrase above. Do not shorten it.

---

### 📖 WORD 13: Limitation of Liability
**Definition:** A cap on how much money you can be made to pay if something goes wrong. Without this, your liability could theoretically be unlimited.

**When to use it:** Every single license and EULA, always.

**The phrase (for OSS):**
> *"IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT, OR OTHERWISE."*

**The phrase (for commercial/EULA):**
> *"IN NO EVENT SHALL LICENSOR'S TOTAL LIABILITY EXCEED THE GREATER OF (A) THE AMOUNT YOU PAID FOR THE SOFTWARE IN THE PAST 12 MONTHS, OR (B) FIFTY DOLLARS ($50)."*

**Why a dollar amount in commercial licenses?** Courts in some places refuse to enforce "zero liability" clauses. A nominal amount ($50, $100) is more likely to be upheld.

**Beginner mistake:** Having no liability cap at all. Or having one but not writing it in ALL CAPS.

**Fix it:** ALL CAPS for the entire disclaimer and liability section. Not optional — courts require disclaimers to be "conspicuous."

---

### 📖 WORD 14: Tort
**Definition:** A legal wrong that causes harm to someone, separate from a breach of contract. Negligence, fraud, and defamation are examples of torts.

**When to use it:** In your liability clause. You want to disclaim liability for contract claims AND tort claims.

**The phrase:**
> *"...WHETHER IN AN ACTION OF CONTRACT, TORT, OR OTHERWISE..."*

**Why you need "or otherwise":** "Contract and tort" covers most cases, but "or otherwise" catches anything that doesn't neatly fit either category.

**Beginner mistake:** Only disclaiming contract liability. A user could sue under a tort theory (like negligence) and argue your disclaimer doesn't cover it.

**Fix it:** Always write the three-part formula: "contract, tort, or otherwise."

---

### 📖 WORD 15: Consequential Damages
**Definition:** Indirect damages that happen as a consequence of a problem — lost profits, lost data, lost business opportunities. These are often far more expensive than the software itself.

**When to use it:** In your limitation of liability. You want to specifically exclude consequential damages.

**The phrase:**
> *"IN NO EVENT SHALL LICENSOR BE LIABLE FOR ANY INDIRECT, INCIDENTAL, SPECIAL, CONSEQUENTIAL, OR PUNITIVE DAMAGES, INCLUDING LOST PROFITS, LOSS OF DATA, OR BUSINESS INTERRUPTION."*

**The full damage list explained:**
- **Indirect** — caused indirectly by your software
- **Incidental** — minor side damages
- **Special** — unusual damages specific to the user's situation
- **Consequential** — downstream results (lost business)
- **Punitive** — punishment damages for bad behavior

**Beginner mistake:** Only writing "no consequential damages" and missing the other four types.

**Fix it:** Copy the full five-part list every time. Courts may find one type covered and another not.

---

### ✏️ PAGE 3 ACTIVITY: Build the Disclaimer

Using only the vocabulary from Page 3, write a complete disclaimer and limitation of liability for a free open source CLI tool you built called "FastLog." Make sure:

- [ ] "AS IS" appears
- [ ] Both express and implied warranties are disclaimed
- [ ] All three specific warranties are disclaimed (merchantability, fitness for purpose, noninfringement)
- [ ] Liability is disclaimed for contract, tort, and otherwise
- [ ] All five damage types are excluded
- [ ] The entire section is in ALL CAPS

Compare your version to the templates in the main License Maker School document. How close did you get?

---

# PAGE 4: The Legal Boilerplate Words
## The Words That Finish Every Document

These are the words that live at the end of every license, EULA, and privacy policy. Beginners often skip this section, treating it like filler. It's not. Each clause does a specific job, and missing one can invalidate your entire document.

---

### 📖 WORD 16: Governing Law
**Definition:** The jurisdiction (country, state, or province) whose laws will be used to interpret and enforce the agreement.

**When to use it:** Every legal document. Always.

**The phrase:**
> *"This Agreement shall be governed by the laws of the State of Delaware, without regard to its conflict of law principles."*

**Why "without regard to conflict of law principles"?**
Without this phrase, courts in other states might apply THEIR state's laws to determine which state's laws apply. This can create a loop. The phrase cuts that off.

**Which jurisdiction to choose:**
- **Delaware** — most US corporations form here; business-friendly courts
- **California** — if you're based there; required for California users in some cases
- **Your home state/country** — simplest if you're small
- **For EU-facing products** — consider adding "For EU users, Irish law applies" to comply with GDPR requirements

**Beginner mistake:** Picking a jurisdiction you've never been to because it sounds fancy, not knowing that if there's ever a dispute, the hearing happens THERE.

**Fix it:** Pick the state or country where you actually live or are incorporated. You want to be able to attend any legal proceedings.

---

### 📖 WORD 17: Severability
**Definition:** If one part of the agreement is found invalid or unenforceable by a court, the rest of the agreement remains in full force.

**When to use it:** Every document. Always.

**The phrase:**
> *"If any provision of this Agreement is found to be unenforceable or invalid under applicable law, such provision shall be modified to the minimum extent necessary to make it enforceable, and all other provisions shall remain in full force and effect."*

**Why it matters:** Imagine your limitation of liability is found unenforceable in one state. Without severability, a judge could throw out your ENTIRE license. With it, just that clause is struck or modified.

**Beginner mistake:** Omitting severability entirely.

**Fix it:** Copy the phrase above verbatim. It's two sentences. It takes five seconds. Always include it.

---

### 📖 WORD 18: Entire Agreement
**Definition:** A clause stating that this document is the complete and final agreement between the parties — no verbal promises, emails, or other documents count.

**When to use it:** EULAs and commercial agreements. Less critical for OSS licenses.

**The phrase:**
> *"This Agreement constitutes the entire agreement between the parties with respect to the Software and supersedes all prior or contemporaneous agreements, representations, warranties, and understandings."*

**Why "supersedes prior agreements" matters:** Without it, someone could argue that a sales email or a promise in a demo counts as part of the agreement. This clause wipes the slate clean.

**Beginner mistake:** Not including this in a EULA. A customer could claim "but the salesperson said I could use it on 10 machines" and there's no clause contradicting that.

**Fix it:** Include it. One sentence. Saves enormous headaches.

---

### 📖 WORD 19: Arbitration
**Definition:** A private dispute resolution process where a neutral third party (an arbitrator, not a judge) hears both sides and makes a binding decision — outside of regular court.

**When to use it:** EULAs and commercial licenses where you want to avoid expensive, public litigation.

**The phrase:**
> *"Any dispute arising out of or relating to this Agreement shall be resolved by binding arbitration administered by [AAA / JAMS] under its Commercial Arbitration Rules, conducted in [City, State]. Each party shall bear its own attorney's fees."*

**Arbitration vs. Court:**
| | Court | Arbitration |
|---|---|---|
| Public? | Yes | No |
| Speed | Slow (years) | Faster |
| Cost | Very high | High but less |
| Appeal | Yes | Very limited |
| Class action | Possible | Usually waived |

**Beginner mistake:** Adding an arbitration clause without specifying which arbitration body (AAA, JAMS, etc.), what rules apply, and where it takes place. An incomplete clause may be unenforceable.

**Fix it:** Name the arbitration organization, the rules, and the location. All three.

---

### 📖 WORD 20: Amendment / Modification
**Definition:** A formal change to the agreement after it was originally accepted.

**When to use it:** Any SaaS EULA or ongoing service agreement where terms might change.

**Two versions — pick one based on your needs:**

**Version A (You can change unilaterally):**
> *"Licensor may amend this Agreement at any time by posting the revised terms at [URL]. Your continued use of the Software after [30] days constitutes acceptance of the amended terms."*

**Version B (Changes require consent):**
> *"This Agreement may only be amended by a written document signed by both parties."*

**Version A** is for SaaS/apps. **Version B** is for enterprise contracts.

**Beginner mistake:** Using Version A language for a one-time purchase app. If someone bought your software outright, you can't unilaterally change the license terms they bought under.

**Fix it:** Ongoing service = Version A. One-time purchase = Version B. Know which you have.

---

### ✏️ PAGE 4 ACTIVITY: The Tail Section Builder

Write the complete "General Provisions" tail section for a fictional SaaS app called "SheetMind" using all five words from this page.

SheetMind details:
- Based in Austin, Texas
- Has US and EU users
- Monthly subscription ($12/month)
- Wants to be able to update its terms
- Has had verbal promises made by sales team in the past

Your section must include:
- [ ] Governing law (Texas, but what about EU users?)
- [ ] Severability clause
- [ ] Entire agreement clause (especially important given the sales team history)
- [ ] Arbitration clause (pick AAA, set it in Austin)
- [ ] Amendment clause (which version, A or B, and why?)

---

# PAGE 5: Common Beginner Mistakes — The Full Fix Guide

This page is the most important one in the workbook. Every mistake on this list was made by a real developer on a real project. Some cost money. Some cost rights. Some cost entire businesses.

---

## ❌ MISTAKE 1: The Empty License
**What it looks like:**
```
This software is free to use. Don't be evil. - The Dev
```
**What's wrong:** No grant. No definitions. No restrictions that actually hold up. Not legally binding in any meaningful way. "Don't be evil" is not a legal standard.

**The Fix:** Use the five-part structure: Grant → Conditions → Restrictions → Disclaimer → Tail. Every license needs all five, no matter how short.

---

## ❌ MISTAKE 2: The Accidental All-Rights-Reserved
**What it looks like:** A GitHub repo with no LICENSE file.

**What's wrong:** Default copyright law applies. Nobody can legally use, copy, modify, or distribute the code. Your open source project is accidentally closed source.

**The Fix:** Add a LICENSE file before your first commit. choosealicense.com makes this one click.

---

## ❌ MISTAKE 3: The Vague Restriction
**What it looks like:**
```
You may not use this software for bad purposes.
```
**What's wrong:** "Bad" is not a legal standard. Every user who's ever done something wrong with software believed their purpose was good.

**The Fix:** Be specific. Instead of "bad purposes" write:
```
You may not use the Software to:
(a) violate any applicable law or regulation,
(b) infringe the intellectual property rights of third parties,
(c) distribute malware or malicious code,
(d) conduct unauthorized surveillance of individuals.
```
Specific lists hold up. Vague adjectives don't.

---

## ❌ MISTAKE 4: Forgetting the Disclaimer Is ALL CAPS
**What it looks like:**
```
The software is provided as-is without any warranty.
```
**What's wrong:** Lowercase disclaimer may not be "conspicuous" enough to be enforceable in some courts. The requirement for ALL CAPS is a real legal standard.

**The Fix:**
```
THE SOFTWARE IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND, 
EXPRESS OR IMPLIED...
```
Simple. Just caps lock it.

---

## ❌ MISTAKE 5: GPL Code in a Proprietary App
**What it looks like:** A developer uses a GPL library to save time, ships their closed-source app, and never thinks about it again.

**What's wrong:** GPL is copyleft. Distributing a program that incorporates GPL code without releasing your source code is a copyright violation. Companies have received real legal threats over this.

**The Fix — three options:**
1. Replace the GPL library with a permissive (MIT/Apache) alternative
2. Release your whole app under GPL
3. Buy a commercial license from the copyright holder (many GPL projects sell one)

---

## ❌ MISTAKE 6: Changing a License Retroactively Without Doing It Right
**What it looks like:** A developer posts code as MIT, people build on it, then the developer changes the license to a restrictive one.

**What's wrong:** You can't revoke rights you already gave. Anyone who received the code under the MIT license keeps those rights forever — the new license only applies to new releases.

**The Fix:** Understand that license changes only affect NEW versions of your software. Old versions stay under the old license. This is why projects fork when licenses change — the fork continues under the old license.

**How to actually change a license correctly:**
1. Make sure you own ALL the copyright (or get permission from every contributor)
2. Create a new version number
3. Apply the new license to that version and beyond
4. Clearly document in your README that v1.x is MIT, v2.x is [new license]

---

## ❌ MISTAKE 7: A Privacy Policy That Lies (Even Accidentally)
**What it looks like:** Privacy policy says "we do not share your data with third parties" but the app uses Google Analytics.

**What's wrong:** Google Analytics is a third party receiving user data. This makes the privacy policy factually inaccurate, which in GDPR territory can mean massive fines.

**The Fix:** Before writing your privacy policy, do a full technical audit:
- List every third-party SDK or service in your app
- List every API call that sends user data somewhere
- List every analytics or crash reporting tool
- Put ALL of them in your privacy policy

When in doubt, disclose more, not less.

---

## ❌ MISTAKE 8: No Jurisdiction Clause
**What it looks like:** A EULA with no "Governing Law" section.

**What's wrong:** If there's a dispute, nobody knows which country's or state's laws apply. This can mean the dispute goes to court in the user's jurisdiction — which might be overseas — instead of yours.

**The Fix:** Always include a governing law clause. For consumer apps, be aware that EU users have additional protections that may override your jurisdiction clause — but you still need one for non-EU disputes.

---

## ❌ MISTAKE 9: Copying Someone Else's License Without Changing It
**What it looks like:** Copying Spotify's EULA word for word, replacing "Spotify" with your app name.

**What's wrong:** Spotify's EULA references their specific business model, their specific services, their specific jurisdictions, and their specific legal team. Large chunks won't apply to you, and important chunks for YOUR situation will be missing.

**The Fix:** Use the templates in this workbook and in the License Maker School document as starting points, not as finished products. Customize every clause for your actual situation. Remove clauses that don't apply. Add clauses for things your situation needs that the template doesn't cover.

---

## ❌ MISTAKE 10: Writing Conflicting Clauses
**What it looks like:**
```
Section 2: You may freely distribute this software.
Section 7: You may not distribute this software without written permission.
```
**What's wrong:** Courts call this a contradiction, and when there's a contradiction in a contract, courts often interpret it against the party who wrote the document (that's you).

**The Fix:** After writing any license, read it from start to finish asking one question at every sentence: "Does anything I've already written contradict this?" If you add an exception to a rule, use "Notwithstanding Section [X]..." to make it clear the exception is intentional.

---

## ✏️ FINAL ACTIVITY: The Full Audit

Take any license you've written (from the activities in the License Maker School, or a real one you've used for a project). Run it through this checklist:

**Structure Check:**
- [ ] Does it have a grant section?
- [ ] Does it define key terms before using them?
- [ ] Are restrictions specific, not vague?
- [ ] Is the disclaimer in ALL CAPS?
- [ ] Does it have a severability clause?
- [ ] Does it have a governing law clause?

**Language Check:**
- [ ] Does the grant use "perpetual, worldwide, royalty-free, non-exclusive, irrevocable"?
- [ ] Does the restriction on reverse engineering say "reverse engineer, decompile, AND disassemble"?
- [ ] Does the disclaimer disclaim both express AND implied warranties?
- [ ] Does it disclaim all five damage types (indirect, incidental, special, consequential, punitive)?
- [ ] Does the liability section cover "contract, tort, or otherwise"?

**Logic Check:**
- [ ] Read every restriction. Is there a clause that contradicts it?
- [ ] Read every permission. Is there a clause that takes it back without using "notwithstanding"?
- [ ] If it's copyleft, does it include a source code distribution requirement?
- [ ] If it's a EULA, does it have an entire agreement clause?
- [ ] If it's a privacy policy, does it list every third-party service?

**Score:**
- 18–20 checks: This is a real license. You built something that holds up.
- 13–17 checks: Good skeleton. Find the gaps and fix them.
- 8–12 checks: Back to Chapter 3 of the License Maker School — reread the anatomy section.
- Under 8: Start fresh using a template. You're building from the wrong foundation.

---

## The 20 Words to Remember — Quick Reference Card

| Word | One-Line Definition | Where It Lives |
|---|---|---|
| Grant | Giving permission | Grant section |
| Perpetual | Lasts forever | Grant section |
| Irrevocable | Can't be taken back | Grant section (OSS only) |
| Non-Exclusive | Given to everyone | Grant section |
| Sublicense | Can pass rights to others | Grant section |
| Derivative Work | Work based on the original | Definitions + Restrictions |
| Reverse Engineer | Reconstructing source from binary | Restrictions (EULA) |
| Competing Use | Building a product that competes | Restrictions (Source Available) |
| Notwithstanding | "Even though" / creates exception | Anywhere exceptions appear |
| Indemnify | You pay if you cause legal trouble | Restrictions / Liability |
| Warranty | A promise about quality | Disclaimer section |
| Merchantability | Works for normal use | Disclaimer section |
| Limitation of Liability | Cap on what you owe | Liability section |
| Tort | Legal wrong outside of contract | Liability section |
| Consequential Damages | Downstream losses (lost profit, data) | Liability section |
| Governing Law | Which country/state's laws apply | Tail section |
| Severability | Bad clause doesn't kill whole doc | Tail section |
| Entire Agreement | This doc is the final word | Tail section |
| Arbitration | Private dispute resolution | Tail section |
| Amendment | How terms can be changed | Tail section |

---

*You now have the vocabulary, the phrases, and the mistake-radar of someone who has been writing licenses for years. The only thing left is practice. Do the activities. Run the audits. Write real licenses for real projects. The 20 words on this page will follow you everywhere in software law.*

---
*This workbook is a companion to License Maker School. For full templates and extended activities, see that document. Neither document constitutes legal advice. For commercial or high-stakes licensing, consult a licensed intellectual property attorney.*

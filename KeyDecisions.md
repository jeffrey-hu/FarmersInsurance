# Key Decisions — Yibiao Lu v. Fire Insurance Exchange

This is a living document recording major strategic and legal decisions made in preparation for the lawsuit. Each entry notes the decision reached, the reasoning behind it, and any dissent or nuance worth tracking. Update this file as new decisions are made.

---

## Decision 1: Which Court to File In

**Decision: File in Minnesota State Court (Hennepin County District Court)**

**Status:** ✅ Confirmed

### ChatGPT's Conclusion
File in Minnesota state court. The primary rationale offered was that Fire Insurance Exchange, as a reciprocal/interinsurance exchange, is likely treated by federal courts as an unincorporated association whose citizenship follows that of all its member-subscribers. Because FIE almost certainly has Minnesota subscribers, complete diversity would be destroyed, making federal jurisdiction unavailable or risky. Filing in federal court first and then losing on a jurisdictional dismissal would expose the claim to a statute of limitations problem upon refiling in state court.

### Independent Analysis
Agreement with the conclusion, but the reasoning is refined as follows:

**Stronger reasons for state court:**

1. **The 2-year contractual limitations deadline.** The policy requires suit within two years of the date of loss. With a loss date of 7/13/2024, the hard deadline is **7/13/2026**. Filing in state court stops the clock cleanly and with no procedural risk. If filed in federal court and subsequently dismissed for lack of subject-matter jurisdiction, Minnesota has no automatic savings statute to rescue the claim — the case would need to be refiled, potentially after the deadline has passed.

2. **Minnesota bad faith law is stronger in state court.** The primary bad faith claim arises under Minn. Stat. § 604.18, which is well-developed in Minnesota state courts. State court judges handle these cases regularly, jury pools are more sympathetic to homeowners, and the precedent is more favorable for plaintiffs.

3. **If FIE removes to federal court, no harm done.** If Farmers/FIE believes diversity exists and removes the case to federal court, the state filing date is preserved — removal never resets the limitations clock. The burden of establishing jurisdiction upon removal falls on *them*. If they fail, the case gets remanded back to state court. Either way, the original filing date controls.

**Note on the ChatGPT diversity argument:** The claim that FIE as a reciprocal exchange necessarily destroys diversity is a real concern but somewhat overstated. The 8th Circuit has not definitively ruled on FIE's citizenship for diversity purposes, and some courts treat insurance exchanges differently from typical unincorporated associations. This argument is available to deploy as a defense against removal — but it should not be relied upon as a guaranteed bar to federal jurisdiction.

**Bottom line:** State court is the correct choice not primarily because federal jurisdiction is unavailable, but because it is the safest and most strategically sound starting point given the approaching limitations deadline and the strength of Minnesota insurance law.

---

## Decision 2: Who to Name as Defendant

**Decision: Fire Insurance Exchange (FIE), optionally styled with its attorney-in-fact**

**Status:** ✅ Confirmed

### ChatGPT's Conclusion
The proper defendant is Fire Insurance Exchange, not "Farmers Insurance" generically. Both the 2014 original policy and the 2023 renewal (the policy in force at the time of loss) explicitly state "Underwritten By: Fire Insurance Exchange." The policy defines "we, us, and our" as "the company providing this insurance," which the declarations page identifies as FIE. Naming "Farmers Insurance" or "Farmers Insurance Group" would leave the complaint vulnerable to a Rule 12(b)(6) motion for lack of contractual privity.

### Independent Analysis
Agreement with ChatGPT's conclusion. The documentary basis is clear and consistent across all policy documents. However, two refinements are worth noting:

1. **A discrepancy in the 2014 documents worth flagging.** The body text of the 2014 Application/Subscription Agreement references "Farmers Insurance Exchange" and "Farmers Underwriters Association" — while the declarations pages and policy form consistently say "Fire Insurance Exchange" and "Fire Underwriters Association." This appears to be boilerplate template language that wasn't updated, and the declarations page controls as a matter of contract law. However, this discrepancy should be anticipated and addressed proactively in the complaint to avoid any "wrong entity" confusion.

2. **Recommended caption language.** The safest way to style the defendant in the complaint is:

   > **Fire Insurance Exchange, by and through its attorney-in-fact, Fire Underwriters Association (doing business as Farmers Insurance)**

   This formulation: (a) names the correct contracting entity, (b) acknowledges the attorney-in-fact structure as described in the Subscription Agreement, (c) ties the legal entity to the brand name the family actually dealt with, and (d) eliminates any "wrong defendant" argument from Farmers' counsel.

3. **Do not name the agent.** Peter Pietila (the Farmers agent) should not be named as a defendant in the coverage/breach-of-contract claim. His role was as a sales and service intermediary; the contractual obligation to pay the claim rests with FIE.

---

## Decision 3: Civil Case Type Designation

**Decision: Designate the case type as "Contract"**

**Status:** ✅ Confirmed

### Reasoning
Minn. R. Civ. P. 10.01 requires every pleading's caption to display, in the upper right-hand corner, a case type matching the State Court Administrator's Case Type Index. Research of the official Minnesota case-category structure (MNCIS) shows insurance-coverage disputes are filed under the **Major Civil → Contract** category, whose case-type descriptions are "Contract," "Mechanics Lien," and "Receivership." **There is no separate "Insurance" case type in Minnesota state court** — the "103 – Insurance" code seen in generic templates is from the *federal* civil cover sheet, not MNCIS.

The lawsuit's lead claim and gravamen is Count I, breach of the insurance contract, with monetary damages sought. "Contract" is therefore the correct, specific designation. The catch-all "Civil Other/Misc." is reserved for cases that fit no defined type; because "Contract" fits squarely, the specific type is used even though the complaint also carries declaratory-judgment (ch. 555) and Minnesota Consumer Fraud Act counts. At e-filing, select the "Contract" major category and the "Contract" case type in the eFS dropdown.

**Sources:** MN State Court Administrator, Case Category Descriptions; Civil Case Type and Filing Code Index (Form 23 replacement); Minn. R. Civ. P. 10.01.

---

## Decision 4: Service by Electronic Mail Between the Parties

**Decision: The parties serve by electronic mail. Agreement reached September 14, 2026.**

**Status:** ✅ Confirmed as to the **method**. ⚠️ **Bare agreement — no terms beyond the method were agreed.**

### What was agreed

Defendant's counsel raised email service first. Plaintiffs consented by email on **September 11, 2026 at 2:54 p.m.**, proposing that either party be able to withdraw consent on written notice. Mary Baskfield confirmed on **September 14, 2026 at 10:04 a.m.**: *"Thank you for consenting to service by email. We agree that you may withdraw this consent by notifying us that you wish to withdraw the consent."* The exchange is preserved at `EventDocuments/2026-09-14-ConfirmOnEmailServiceAndProtectOrder.pdf`.

The agreement establishes **that** the parties may serve by email, **at which addresses**, and **that consent is revocable on notice**. It does not address when service is complete, how days are counted, what happens if a transmission fails, or how oversized productions are exchanged.

⚠️ **Two asymmetries worth noting.** Plaintiffs proposed that *"Each party should have the right to withdraw this consent upon written notice."* Baskfield's confirmation speaks only to Plaintiffs' right to withdraw (*"you may withdraw"*) and does not say the notice must be in writing. Neither is likely to matter, but if Defendant ever withdraws consent orally, the asymmetry is the reason to insist on written confirmation.

### Why the agreement was necessary

Plaintiffs are excluded from the eFiling System under Scheduling Order ¶12(a)(i). **Minn. Gen. R. Prac. 14.03(d)(2)** therefore made email the only available electronic method, and only by consent:

> "Where the party or participant to be served is not a Registered User or has not either designated an email address for receiving electronic service in the E-Filing system for the case or electronically filed a document in the case but **has agreed to service by electronic means outside the E-Filing System** (such as by e-mail or other electric means), service may be made **in the agreed upon manner**."

Before September 15, 2026 that condition was unsatisfied, and email service would have been ineffective in either direction. It is now satisfied.

### Addresses of record

| Served on | Addresses |
|---|---|
| **Plaintiffs** | `bill_y_lu@yahoo.com` **and** `jie_h_hu@yahoo.com` — both together constitute service on both Plaintiffs |
| **Defendant** | `kkennedy@kennedylf.com` **and** `mbaskfield@kennedylf.com` |

Serve counsel of record, never FIE or its registered agent. Minn. R. Civ. P. 5.02(a).

### The two terms that matter are supplied by rule, not by the agreement

The September 14, 2026 draft stipulation (`Filings/Discovery/Proposed_EService_Stipulation_and_Certificate_2026-09-14.md`) warned that a silent agreement would leave the completion question open. On verification against the primary sources, **it does not** — the rules fill both gaps, so the bare agreement is workable:

1. **When service is complete.** Minn. Gen. R. Prac. 14.03(e): *"Service using other agreed upon electronic means pursuant to Rule 14.03(d)(2) is complete **upon transmission** of the document using that electronic means."* Not upon receipt, not upon the recipient opening it.
2. **How many days are added.** Minn. R. Civ. P. 6.01(e) adds 3 days only where the document "is served upon the party **by United States Mail**." For email: **zero days added**, except *"If service is made by any means other than United States Mail and accomplished **after 5:00 p.m.** local Minnesota time on the day of service, **1 additional day** shall be added to the prescribed period."*

**⚠️ Net effect on every deadline from here forward: Plaintiffs lose the 3-day mail cushion, in both directions.** A 30-day response period is now 30 days, not 33. Incoming deadlines are tighter than they were before today. Recalculate anything already calendared on the mail assumption.

### What remains open

| # | Open item | Why it matters |
|---|---|---|
| **(a)** | **No failed-delivery protection.** Rule 14.03 contains no analogue to Fed. R. Civ. P. 5(b)(2)(E) ("not effective if the serving party learns that it did not reach the person to be served"). | Service is complete on transmission **even if the message bounces or lands in spam**. A document emailed at 3:00 p.m. starts a bare 30-day clock that day whether or not Plaintiffs ever see it. **Operational rule: check both Plaintiff inboxes and their spam folders daily. Never assume Defendant will re-serve.** |
| **(b)** | **Oversized productions.** The claim file and a 217-photograph appendix will exceed ordinary attachment limits; no transfer mechanism was agreed. | Raise before FIE's first production, not after. |
| **(c)** | **Whether both Plaintiffs are on Defendant's service list.** | Unconfirmed. Ask Kennedy to confirm in writing. |
| **(d)** | **Whether to embody the agreement in the stipulated order.** | **Undecided.** A court-entered term is enforceable and survives a change of defense counsel; a counsel-to-counsel email does neither. The itemized wording is held ready at the foot of the e-service file for the combined Protective / ESI / Claw-Back / E-Service stipulated order. Decide before that order is sent. |

### Consequence for the First Discovery Sets

The email certificate of service already in the operative `.docx` files is now **accurate**, and the blocking service defect identified in `Filings/Discovery/FirstSetDiscovey/Interrogatories/Interrogatories_First_Set_Independent_Review_2026-09-15.md` § 2 is **cured**.

Email service is complete on transmission (Minn. Gen. R. Prac. 14.03(e)), so the 30-day response period under Minn. R. Civ. P. 33.01(b) runs from the send date, adding nothing — except that a transmission **after 5:00 p.m.** adds one day under Minn. R. Civ. P. 6.01(e). **Send before 5:00 p.m.**

⚠️ **Service backstop: October 16, 2026.** To have responses in hand before the November 16, 2026 joinder deadline, the sets must be served by **October 16, 2026** at the latest. Every day of delay past that date is a day the joinder decision has to be made without Defendant's answers. As of September 16, 2026, the Requests for Production were served on September 15, 2026 (responses due October 15, 2026; `Filings/Discovery/Service_Log.md`). The Interrogatories and the Requests for Admission were **not yet served** as of that date. **They will be served separately** (decision, September 16, 2026), each on its own 30-day clock, and each should be served by October 16, 2026 at the latest:

> **Update, September 20, 2026.** Both remaining sets are dated **September 20, 2026** and go out that day — comfortably inside the backstop. "Separately" still holds and still matters: each travels in its **own message with its own certificate of service**, so neither certificate covers the other. Same-day service simply means the two 30-day clocks start together — sent before 5:00 p.m., both sets of answers fall due **Tuesday, October 20, 2026**; a transmission after 5:00 p.m. Minnesota time adds one day under **Rule 6.01(e)** and makes it Wednesday, October 21. Note that September 20 is a **Sunday**: nothing in Minn. R. Civ. P. 5.02, Minn. Gen. R. Prac. 14.03 or Rule 6.01 requires service on a business day, and Rule 6.01(a)(1)(C)'s weekend rule reaches only the *last* day of a period, not the day of service. Deadlines recorded in `Filings/Discovery/Service_Log.md`.

- **Requests for Admission:** the set now runs **Nos. 1–141** in sections **A–U**, 17 pages. On September 20, 2026, **44 requests moved to the Second Set as its Part 6** (old Nos. 57, 60–76, 80–101, 106 and 110–112 — the Prieve dent findings, the photograph and caption requests, and the page-6 hail diagnostic), old section I was dissolved into section H, and the set was renumbered once. Old→new: **Table G** of `Filings/RequestForAdmission/FirstSet/RFA_Renumbering_Map_2026-09-16_Final.md`. ⚠️ **Serve Second Set Part 6 before Nathan Prieve's deposition** — Nos. 79 and 80 there are the page-6 diagnostic quotes, and they are worth materially less once he has testified. Date it, sign it, and serve the First Set.
- **Interrogatories:** ~~still blocked by the inaccurate Rule 33.01(a) certification~~ — **superseded.** That paragraph was deleted September 17, 2026. The set now runs **Nos. 1–12** with 30 definitions and 13 instructions, 9 pages, dated **September 20, 2026**, `.docx` verified against the `.md` paragraph-for-paragraph. Later changes are logged as tracker rows **F-40 through F-44** in `Filings/Discovery/FirstSetDiscovey/Interrogatories/Interrogatories_First_Set_Review_2026-09-17.md`. Remaining: both signatures, export to PDF, serve before 5:00 p.m.

~~The unverified RFA 23~~ is **resolved** (September 16, 2026). Checked against the award image, the old request ("Greg Tomes did not sign The Appraisal Award") was wrong as drafted: Tomes signed the umpire-appointment block, and left blank only his line under "We certify the amounts established above." The request was rewritten and is now **First Set No. 23**, with a companion at **No. 24** (renumbered twice on 9/19/2026: they were Nos. 29–30, became Nos. 32–33 in the first pass, and are Nos. 23–24 after the trim), under the numbering that descends from September 16, 2026 (`Filings/RequestForAdmission/FirstSet/RFA_Renumbering_Map_2026-09-16_Final.md`). ✅ Both were verified by Bill against the award on September 16, 2026.

## Decision 8: The Certificate of Service — Canonical Form

**Decision: certify under penalty of perjury (Minn. Stat. § 358.116), never by sworn-affidavit preamble, and recite only what Rule 5.04(b) and § 358.116 require. Adopted September 20, 2026.**

**Status:** ✅ Applied to the First Set Interrogatories and the First Set Requests for Admission, both `.md` and `.docx`. The canonical block lives at **§4 of `Filings/Document_Formatting_Standard.md`** — copy it from there.

### What the rules require, and nothing more

**Minn. R. Civ. P. 5.04(b)** prescribes the whole content: "the details of how and when service was accomplished," signed "under oath **or** penalty of perjury by the person effecting service." **Minn. Stat. § 358.116** adds the declaration sentence, the signature below it, and the **date, county and state** of signing. **Minn. Gen. R. Prac. 14** prescribes no certificate contents at all. Everything else that had accumulated — the over-18 recital, "personally made," the ¶1–¶4 numbering, attorney registration numbers, counsel's street address, and the `Name:` / `Address:` / `City/State/Zip:` / `Telephone:` / `E-mail address:` block — came from the Judicial Branch **affidavit of service** form, which exists for **Rule 4** service of process. Rule 4.02 requires a server "not less than 18 years of age **and not a party to the action**"; none of that governs Rule 5 service on an appearing party's counsel, which is why a pro se party may serve their own discovery. All of it was removed. 197 words → about 120.

### Why: a sworn certificate should contain only what it can stand behind

Everything in the certificate is sworn under penalty of perjury. A recital that is not required and does not prove service is one more thing to be accurate about for no gain — which is exactly how the **Baskfield registration-number problem** arose (see I-5). Where service is contested, the proof is the sent message and its full headers, so the certificate names the **sending address**, and the exact transmission time is recorded in `Filings/Discovery/Service_Log.md` rather than in a blank on a document signed before the send.

### ⚠️ Never use "being first duly sworn on oath"

That is a **jurat** formula and means something only where a notary administers the oath and signs below. Rule 5.04(b) offers oath **or** penalty of perjury; § 358.116 is the no-notary route these filings take. Combining the two puts a false recital of an oath into a document signed under penalty of perjury.

FIE's own **Affidavit of Service of August 10, 2026** does exactly that: "Julie Parks, being first duly sworn on oath, deposes and states," with **no notary block, signature or seal**, then § 358.116 — and it omits the county and state of signing that § 358.116 requires. Bill raised it as a possible model on September 20, 2026; it is not one.

### Companion formatting rule: signature blocks side by side

**Decision: the two Plaintiffs' signature blocks sit side by side, not stacked. Adopted September 20, 2026.** Stacked, they consume half a page and can split across a page break; side by side they read as a single signature line in six. Built as a **borderless one-row, two-column table** in the `.docx` and a two-column pipe table in the `.md` twin. Applied to the First Set Interrogatories (9/19/2026) and the First Set Requests for Admission (9/20/2026). Mechanics at **§3 of `Filings/Document_Formatting_Standard.md`**.

⚠️ **Page breaks in these documents live inside empty paragraphs** (`<w:br w:type="page"/>`), not in section breaks — that is what puts the certificate of service on its own page. Empty paragraphs are therefore not interchangeable, and duplicating one duplicates the break. Doing exactly that while building the RFA signature table turned a 20-page set into 22 pages with two blank pages; a paragraph-by-paragraph `.md`/`.docx` comparison showed **zero** mismatches throughout, because the offending paragraphs are empty. **Render to PDF and scan for blank pages after any change near the signature block or the certificate.**

---

### Housekeeping

The written agreement is preserved at `EventDocuments/2026-09-14-ConfirmOnEmailServiceAndProtectOrder.pdf`, with a pointer at `Filings/Discovery/CommunicationLogs/2026-09-14-EServiceAndProtectiveOrder/`. **The existence of the writing is what makes every subsequent email service valid** — if it is ever contested, that exchange is the proof.

**Sources:** Minn. Gen. R. Prac. 14.03(d)(2), (e) — https://www.revisor.mn.gov/court_rules/gp/id/14/ · Minn. R. Civ. P. 6.01(e) — https://www.revisor.mn.gov/court_rules/cp/id/6/ · Minn. R. Civ. P. 5.02 — https://www.revisor.mn.gov/court_rules/cp/id/5/ · Scheduling Order ¶12(a)(i), September 8, 2026. Verified against primary sources September 15, 2026.

---

## Decision 5: No Protective Order — Defendant Declined One and Consented to Jeffrey Hu's Access

**Decision: Plaintiffs withdraw their proposal for a stipulated protective order.**

**Status:** ✅ Resolved as to Defendant's present position. ⚠️ **Expressly reserved by Defendant — "at this time."**

### What Defendant said

Mary Baskfield, September 14, 2026:

> "As you will recall, I informed you that I did not see a need for a protective order and did not have an issue with your son reviewing discovery documents in this case. To confirm, our client is not seeking a protective order **at this time**. We do not object to your son Jeffrey Hu reviewing the discovery documents."

### Why this matters more than it looks

`OfficialCourtDocuments/SchedulingOrder_Impact_Analysis_2026-09-10.md` § 3(c) identified the absence of a protective order as **"the largest unaddressed exposure in the Order"** — the risk being that Defendant would designate claims manuals, training materials or vendor agreements "attorneys' eyes only," which, against pro se Plaintiffs with no counsel of record, would operate as a complete bar on Plaintiffs' access to the evidence in their own case. Defendant's position removes that risk for now, and removes it without Plaintiffs having to negotiate or litigate for it.

### ⚠️ What Defendant did not say

Plaintiffs asked whether Defendant objected to disclosure of confidential material to Jeffrey Hu **"subject to his signing a written undertaking to be bound by the protective order."** Baskfield did not address the undertaking. She removed its premise instead — no protective order at all. So there is **no agreed framework** for what happens if Defendant later changes position, and **"at this time"** reserves that expressly. Defendant has not yet seen what RFP 10, 28 and 31 will require it to produce.

### Action taken

Section 2.1 of `Filings/Discovery/Meet_and_Confer_Letter_Scheduling_Order_2026-09-11.md` was rewritten on September 15, 2026 to record Defendant's position, withdraw the protective-order proposal, and ask Defendant to confirm three forward-looking points: written notice before any designation, no counsel-only tier, and that Jeffrey Hu's access survives any later designation subject to an undertaking.

**Sources:** `EventDocuments/2026-09-14-ConfirmOnEmailServiceAndProtectOrder.pdf` · Scheduling Order ¶16(e) · `SchedulingOrder_Impact_Analysis_2026-09-10.md` § 3(c).

---

## Decision 6: Meet and Confer on the Scheduling Order — Letter Sent September 15, 2026

**Decision: Plaintiffs raised six implementation issues under the September 8, 2026 Scheduling Order by letter rather than by motion, and set their own response dates.**

**Status:** ✅ Sent. ⏳ **Awaiting Defendant — September 29 and October 9, 2026.**

Sent by email at approximately 8:49 p.m. on September 15, 2026 to Mary Baskfield and Kevin Kennedy, cc Jie Hu. The signed three-page PDF as sent is at `OfficialDiscoveyDocuments/MeetAndConfer/Lu_Hu_Meet_and_Confer_Letter_2026-09-15.pdf`; the full log entry, including the item-by-item table of what was asked, is at `Filings/Discovery/CommunicationLogs/2026-09-15-MeetAndConferLetterSent/`.

### Why a letter and not a motion

Minn. Gen. R. Prac. 115.10 requires the parties to confer before **any** motion. Three of the four motions now foreseeable in this case — a joinder motion, a Rule 111.04 motion to extend the joinder deadline, and any motion about the scope of the March 15, 2027 deadline — would each have needed a conferral record. One letter creates that record for all of them, and does so before the disputes harden. The letter also says so on its face: *"This letter also begins the conferral required by Minn. Gen. R. Prac. 115.10."*

### The dates this letter now controls

| Date | What | Consequence of Defendant's silence |
|---|---|---|
| **Sept. 29, 2026 (Tue)** | Items 1–4, item 6 (mediation), and the preservation confirmation | Plaintiffs may proceed under ¶4 of the Scheduling Order on any discovery dispute, having conferred |
| **Oct. 9, 2026 (Fri)** | Item 5 — Defendant's position on the proper party | Silence is itself the good-cause showing for a Rule 111.04 motion, and the trigger to file a protective joinder motion |
| **Oct. 13, 2026 (Tue)** | Mediator candidates exchanged | Moves toward the Rule 114.04(b) impasse fallback |
| **Oct. 27, 2026 (Tue)** | Scheduling Order ¶6 notice to the Court of the neutral and the mediation date | Neither party can satisfy ¶6 alone — a joint notice of impasse asking the Court to appoint a Qualified Neutral becomes the fallback |
| **Nov. 16, 2026 (Mon)** | Joinder deadline | A Rule 111.04 extension motion must be **made before** this date, not on it |

### The two things that make this letter work later

1. **It is dated and it is provable.** Keep the sent message with full headers. Under Minn. Gen. R. Prac. 14.03(e) email service is complete on transmission, and the September 14, 2026 e-service agreement (Decision 4) is what makes that valid here.
2. **It states rule arithmetic, not preference.** The letter shows *why* October 9 is the date — Rule 21 plus Gen. R. Prac. 115.04 plus Rule 115.02 put any joinder motion on file in late October. The Court's September 8 Order already rejected Plaintiffs' proposed timeline as "more than one year beyond the timeline for similar cases," so a later request for relief has to be arithmetic, not a general plea for time. This letter is that arithmetic, on the record, six weeks early.

### Follow-up

If nothing arrives by **September 30, 2026**, send a short follow-up email. An unanswered letter is good; an unanswered letter plus a documented, ignored reminder is materially better on a Rule 111.04 or Rule 37.01 showing.

**Sources:** Minn. Gen. R. Prac. 115.10, 115.04, 115.02, 114.04(b), 111.04 · Minn. R. Civ. P. 21, 16.02 · Scheduling Order ¶¶1, 2, 3, 5, 6, 8, September 8, 2026 · Letter as sent, verified page by page September 16, 2026.

---

## Decision 7: Interrogatory No. 1 Anchored to the November 4, 2024 Decision; the Award-Scope Contention Held for the Second Set

**Decision: First Set Interrogatory No. 1 asks what FIE decided on November 4, 2024 and why. The question of what FIE contends today — and whether it claims The Appraisal Award reached items it does not name — is held for the Second Set. September 18, 2026.**

**Status:** ✅ Confirmed.

### The problem

Interrogatory No. 1 as previously drafted asked, for each dented window and component, the cause FIE attributes to it and "any portion of The Appraisal Award You contend determined the question." That trailing clause let FIE answer the whole interrogatory in one sentence — the award is binding, it awarded two windows, nothing else is hail — supplying no per-item cause, no dates, no facts and no exclusions, and converting the award's **silence** into a determination. That is the "evaluated-but-rejected" scenario identified at `OffenseStrategies/AppraisalAwardStrategy/06_Addendum_EvaluatedButRejected.md` as the case's weakest point.

### What was done instead

**Interrogatory No. 1 is now anchored to The November 4, 2024 Claim Outcome Letter** and its sentence, "Our investigation found the condition of the window and components to be from wear/tear as referrenced [sic] in the attached engineer report." The decision it asks about was made **ten months before the September 12, 2025 award existed**, so the award cannot answer it and any answer invoking the award is non-responsive on its face. The question is historical rather than contention-based, which also puts it beyond a Rule 33.02 request to defer, and it builds the § 604.18 record, which measures the absence of a reasonable basis **at the time of denial**.

The F1.7/B1.2 carve-out was **dropped**: on November 4, 2024 FIE attributed both of those windows to the 2020 claim (Prieve Conclusion 1, "these 2 windows have already been included and we understand paid for due to prior storm activity"), and its own panel later entered "Hail" for them. Answering as to all windows sets FIE's file against its own panel. Nothing about answering a historical question disturbs the award's binding effect; RFAs 25–27 hold that line.

Three definitions support it: **"The November 4, 2024 Claim Outcome Letter"** (new — date-anchored because the September 3, 2024 letter carries the same "Claim Outcome Letter" caption and its own "Coverage Outcome – Policy Provisions" attachment), **"The Coverage Outcome Attachment"** (restored, now anchored to the defined letter) and **"The Prieve Report"** (transmittal clause restated through the defined letter; the premise is admitted at Answer ¶20).

### Why the contention half waits

The award-scope question — what FIE contends now, and what facts show the panel evaluated an item — is parked at `Filings/Discovery/SecondSetDiscovery/Plaintiffs_Second_Set_of_Interrogatories_to_FIE_DRAFT.md` as **Draft Interrogatory No. 2**. Asked in the First Set it is open-ended and exposed to Rule 33.02 deferral; asked after the First Set responses it can quote FIE's own answers and denials back at it. **Target service: the week of November 2, 2026. Backstop: February 12, 2027** (discovery closes March 15, 2027, and the appraiser depositions depend on these answers).

**Round one is not left empty.** Requests for Admission **205–207** (added September 18, 2026) carry the award-scope work: what the award does not say about any other window, what the August 3, 2025 demand submitted, and what was never submitted to the panel. Rule 36.01 admits an unanswered request; Rule 36.02 makes an admission conclusive. Rule 36 has no numerical limit, so they cost nothing.

**Watch item.** If FIE notices a dispositive motion on the binding-award theory before those answers are in, serve the Second Set that week and oppose with a Minn. R. Civ. P. 56.04 affidavit. Motions need only be *heard* by May 14, 2027, so FIE has no structural reason to move early.

### Addendum, same day — old Interrogatory No. 2 also held

The Prieve scoping interrogatory ("State how the scope of Prieve Engineering's engagement came to be limited to the condition of the windows…") was removed from the First Set for the same reason, on Bill's call: its premise is contestable (Conclusion 4 of The Prieve Report opines on siding), and **RFP 5 and RFP 7**, served September 15, 2026, already seek the engagement documents and the scoping decision. Held as Draft Interrogatory No. 3 in the Second Set, triggered by that production and by the answers to RFAs 58 and 201. **The First Set now runs 1–15**, at a fair count of about 29.

Later the same day, on the same reasoning, the interrogatory asking the basis for Brau's October 29, 2025 statement ("All the information we can release has already been sent to you") and its consistency with the October 10, 2025 statement was also held, as **Draft Interrogatory No. 4**. Its facts are pinned harder by **RFAs 137–139, 147, 148, 165, 168 and 203** and by **RFP 3**, and Rule 36.02 makes an admission conclusive where an interrogatory answer is not. Served with the First Set, its one unique clause — reconciling the two statements — would have been answered **alongside** those admissions instead of after them. The search-narrative interrogatory (now No. 3) stays in the First Set, because no admission or document request can produce it. **The First Set runs 1–14**, at a fair count of about 27.

### Second addendum, September 18, 2026 — the two award-itemization interrogatories merged, and the § 604.18 bar held

Old Ints. 5 and 13 asked the same per-item question twice. They are now a single **Int. 5** anchored to **Answer ¶33**, FIE's pleaded denial that the award fails to state actual value and loss separately to each item — with a new clause asking whether the values for "Windows F1.7 B1.2" were determined **separately for each of those two windows**, and a new defined term, **"The Appraisal Demand."** The § 604.18, subd. 4(c) clause was held as Second Set **Draft Interrogatory No. 5**: subd. 4(a) bars pleading taxable costs initially and the Complaint reserves them for a post-pleading motion, so the bar is not yet ripe. **The First Set runs 1–13**, at a fair count of about 25.

**Count III framing, settled 9/18/2026 after research.** § 65A.01, subd. 3 requires an award "stating separately actual value and loss to each item" and gives determinative effect only to an award "so itemized" — but **no Minnesota case defines how fine an "item" is**, and *Bell v. Liberty Mutual Fire Ins. Co.* (Ga. Ct. App. 2012) reads the same sentence as requiring itemization only by coverage category. **Brief Count III as ambiguity requiring clarification** (*Herll*, 879 F.3d 293 (8th Cir. 2018); *Cincinnati Ins. Co. v. Rymer Cos.* (8th Cir. 2026)) — undefined "F1.7"/"B1.2" codes, one lump RCV/ACV for two windows at opposite elevations, uniform 50% depreciation — not as "the statute requires a value for every window." Expect remand to the panel rather than a ruling that the award determined nothing; Quade-reservation remains the primary lane.

**Authority:** *Quade v. Secura Ins.*, 814 N.W.2d 703 (Minn. 2012) (amount of loss "necessarily includes a determination of the cause of the loss"; coverage questions "are legal questions for the court"; "an appraisal award does not preclude the insurer from subsequently having its liability on the policy judicially determined") · *Herll v. Auto-Owners Ins. Co.*, 879 F.3d 293 (8th Cir. 2018) (ambiguous award returned to the panel for clarification) · Minn. R. Civ. P. 33.02, 36.01, 36.02, 37.01, 56.04 · Scheduling Order, September 8, 2026. Verified against primary sources September 18, 2026.

## Decision 9: Correspondence with Opposing Counsel — Tone and Content Rules

**Decision (Bill, September 20, 2026): transmittal emails and routine correspondence to Kennedy Law are businesslike and short. Apply these rules to every email to counsel unless a specific document calls for something different.**

| # | Rule | Why |
|---|---|---|
| 1 | **Never characterize the size of our own discovery**, and do not give the request or interrogatory count in the covering email. State what the document is, when it was served, and when responses are due. | Explaining the length concedes that the length is a problem and invites a burden objection or a protective-order motion. The document speaks for itself. |
| 2 | **No invitation to flag unclear requests**, and no offer to clarify or withdraw any request in advance. | It reads as though the drafting is unsettled. If counsel raises a specific request later, deal with it then, on its own facts. |
| 3 | **Never offer an extension.** Deadlines fixed by rule are not negotiated in a transmittal. | An unprompted extension gives away time for nothing. If counsel asks, decide on the merits against the calendar then in force — in particular the **November 16, 2026 joinder deadline**, which the entity requests feed. |
| 4 | **Neutral, businesslike register.** Open with "Counsel," not first names. No warm openers, no thanks in advance, no "we would rather resolve this than litigate" softeners. | These are adversaries with an appearance on file. Warmth reads as anxiety and is not reciprocated. |
| 5 | **Say only what the record needs:** what the document is, that it was served today by electronic mail in the manner the parties have agreed, and a request to confirm receipt. | Everything else is either surplus or a hostage to fortune. The quoted phrase is the operative fact — it is how the clock starts. |
| 6 | **No response deadline in the email — neither a date nor a rule citation.** Calendar it in `Filings/Discovery/Service_Log.md` instead. | Nothing requires the notice: the period runs by operation of Minn. R. Civ. P. 33.01(b) and 36.01, the certificate fixes the date and manner, and the message header fixes the time. A stated date is a representation to live with, and one stated too generously is something counsel can say it calendared in reliance on. It is also the natural hook for an extension request (rule 3), and for Requests for Admission it is a reminder that reduces the chance of a Rule 36.01 default. Added 9/20/2026. |

**The one standing exception — meet-and-confer correspondence.** Letters written to satisfy a good-faith conferral requirement (Minn. Gen. R. Prac. 115.10; Minn. R. Civ. P. 37.01) exist to make a record of reasonableness, and may properly say that Plaintiffs would rather resolve an issue by agreement than by motion, and may offer to confer by phone or video. The September 15, 2026 meet-and-confer transmittal (`Filings/Discovery/Transmittal_Email_MeetAndConfer_2026-09-15.md`) is the model for that genre, and is **not** the model for a discovery transmittal.

**Applied first to:** the transmittal of Plaintiffs' First Set of Requests for Admission, September 20, 2026 (`Filings/Discovery/Transmittal_Email_RFA_FirstSet_2026-09-20.md`).

---

*Last updated: 2026-09-20 — **Decision 8 added** (canonical certificate of service; no sworn-affidavit preamble; §4 of `Filings/Document_Formatting_Standard.md` is the source), with a companion rule putting the two Plaintiffs' signature blocks side by side (§3) and the page-break-in-an-empty-paragraph hazard recorded. Also: service dates set to September 20, 2026 for both remaining First Set sets (both answers due October 20, 2026); RFA count corrected to Nos. 1–185 in sections A–V; the Tomes-signature requests renumbered to Nos. 23–24; the Interrogatories' Rule 33.01(a) blocker marked superseded in place. Earlier: 2026-09-18 — Decision 7 added (with same-day addendum holding old Int. 2) (Interrogatory No. 1 re-anchored; award-scope contention held for the Second Set; RFAs 205–207 added). Decision 4's note that the Interrogatories are blocked by the Rule 33.01(a) certification is **superseded** — that paragraph was deleted September 17, 2026.*

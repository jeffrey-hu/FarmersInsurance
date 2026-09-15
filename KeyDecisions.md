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

The email certificate of service already in the operative `.docx` files is now **accurate**, and the blocking service defect identified in `Filings/Discovery/FirstSetDiscovey/Interrogatories/Interrogatories_First_Set_Independent_Review_2026-09-15.md` § 2 is **cured**. Served by email before 5:00 p.m. on September 16, 2026, responses are due **October 16, 2026** — 31 days before the November 16, 2026 joinder deadline, and three days sooner than service by mail would have produced.

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

*Last updated: 2026-09-15 — add new decisions below as they are made.*

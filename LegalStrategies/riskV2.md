# Litigation Financial Risk Analysis — V2 Delta

**Companion to:** `risk.md` (V1)
**Case:** Yibiao Lu & Jie Hu v. Fire Insurance Exchange (d/b/a Farmers Insurance)
**Prepared:** May 15, 2026

> **Purpose.** This is a *delta-only* summary. It describes what changed between V1 (`risk.md`) and V2. The underlying V1 analysis stays authoritative for everything not addressed here; read `risk.md` first, then read this for the V2 adjustments.
>
> **What's V2.** Two changes:
> 1. **Part 1 — Section 1.5 added** (pro se / DIY budget, authored by Jeffrey at a later date than the rest of `risk.md`).
> 2. **Part 2 — recalibration** assuming (a) disciplined use of the Minn. Stat. § 549.211 / Minn. R. Civ. P. 11.03 21-day safe harbor and (b) appeal costs excluded from scope.

---

## 1. Part 1 V2 — Section 1.5 added (Pro Se / DIY budget)

### What changed

V1 Part 1 (Sections 1.1–1.4 and 1.6) priced the case assuming **hourly counsel** and a conventional litigation budget — $90,000 low end / $295,000 high end in Plaintiffs' out-of-pocket costs through trial. Section 1.5 adds the **pro se / DIY posture** as a parallel scenario, which is the more realistic posture for this family given (a) the June 11, 2025 MN Lawyer Referral Service refund and (b) the deductible-math problem that makes contingency counsel hard to attract.

### Key deltas under pro se / DIY

- **Attorney fees collapse to $0** (the family doesn't bill itself). This is the single largest line-item delta from V1.
- **Trial exhibits / disbursements collapse from $5K–$20K to ~$300–$2,000** (DIY production, consumer print services, AI-generated demonstratives).
- **Court reporter fees survive mostly intact** ($3,000–$15,000); not DIY-able because depositions require licensed reporters.
- **Expert witness spend drops to $5,000–$30,000** by limiting to one mandatory forensic engineer (to rebut Prieve) plus optional matching/valuation/appraisal-process specialists.
- **Total pro se / DIY out-of-pocket: ~$9,700 (floor) to ~$67,500 (ceiling)**, vs. V1's $90,000–$295,000 with hourly counsel.

### Plaintiffs' cash-flow timeline (from § 1.5.4)

```
                    PROJECTED CASH OUTFLOW BY CASE PHASE (PRO SE / DIY)

  Phase             Months    Cost Range          Visual (each # ≈ $1,000)
  ────────────────────────────────────────────────────────────────────────
  Filing & service  M 0       $400 – $1,500       #
  Early discovery   M 1–6     $500 – $2,000       ##
  Deposition phase  M 6–15    $3,000 – $15,000    ###############
  Expert retention  M 12–18   $5,000 – $30,000    ##############################
  Mediation         M 12–15   $0 – $3,000         ###
  Trial prep & trial M 18–22  $1,500 – $8,000     ########
  ────────────────────────────────────────────────────────────────────────
  CUMULATIVE        M 0 → 22  $9,700 – $67,500
```

### Hidden cost the V2 Section 1.5 surfaces

Pro se posture **largely moots the fee-shifting upside described in V1 §§ 1.2–1.3.** Minnesota courts do not award "attorney fees" to pro se litigants under § 604.18 or the MCFA, because there are no attorney fees to award. The family can still recover **taxable costs and disbursements** under § 549.04 if they prevail — meaning the cash outlay above can be partially reimbursed — but the headline § 604.18 $100K cap and uncapped MCFA fee-shifting do not function as personal compensation for the family's time.

### Net effect on V1's framing

The "Plaintiffs front-load tens of thousands of dollars in real money" warning in V1 § 1.3 is still correct, but the magnitude is materially smaller under the pro se posture (~$10K–$50K vs. $90K–$295K). The fee-shifting upside also shrinks proportionally, leaving the case roughly cost-neutral after reimbursement rather than profitable.

---

## 2. Part 2 V2 — Recalibration assuming 21-day safe harbor and no appeals

### What changed

V1 Part 2 estimated Defendant's worst-case cost recovery at $30,000+ (taxable costs $4,400–$28,500 + sanctions $0–$30,000). V2 makes two assumptions that materially shrink that number:

1. **21-day safe harbor invoked.** Under Minn. Stat. § 549.211, Subd. 4(a) and Minn. R. Civ. P. 11.03(a)(1), a sanctions motion must be served 21 days before filing; if the challenged claim is withdrawn during that window via Minn. R. Civ. P. 41.01 voluntary dismissal, the motion cannot be filed. With disciplined safe-harbor use, **sanctions exposure goes to $0 on both v2 and v3** — the only residual sanctions risk (sua sponte under § 549.211 Subd. 5, or inherent-authority sanctions for bad-faith conduct) is empirically negligible in first-party insurance cases.
2. **Appeal-stage cost exposure excluded from scope.** V1 understated this by omitting it; V2 keeps it omitted per Jeffrey's instruction. (Note: a future revision should address appeal costs separately — they're real money if Plaintiffs lose at trial and appeal.)

### Recalibrated cost-recovery estimates

| Scenario | V1 estimate | V2 recalibrated estimate |
|---|---|---|
| Loss at Rule 12 dismissal | (not separately given) | $1,000–$3,000 |
| Loss at summary judgment | (not separately given) | $4,000–$10,000 |
| Loss at trial — taxable costs | $4,400–$28,500 | $8,000–$18,000 |
| Sanctions (v2) | $0–$15,000 | **$0** |
| Sanctions (v3) | $5,000–$30,000 | **$0** |
| Rule 68 post-offer cost shift | (not separately modeled) | $3,000–$15,000 |
| **Worst case (v2/v3, trial loss, no Rule 68 hit)** | ~$30,000+ | **$8,000–$18,000** |
| **Worst case (v2/v3, trial loss, Rule 68 hit)** | (not modeled) | **$11,000–$33,000** |

### Recalibrated cash-flow timeline

```
              PROJECTED DEFENDANT COST-RECOVERY EXPOSURE BY CASE PHASE
              (payable at adverse judgment; safe harbor → sanctions $0; appeals excluded)

  Phase                  Months    Exposure Range      Visual (each # ≈ $1,000)
  ────────────────────────────────────────────────────────────────────────────
  Filing & Rule 12       M 0–3     $200 – $1,500       #
  Early discovery        M 3–6     $300 – $1,500       #
  Deposition phase       M 6–15    $2,000 – $6,000     ######
  Rule 68 post-offer     M 6–22    $0 – $15,000        ###############
   cost shift            (accrues only if offer rejected & not beaten at trial)
  Summary judgment       M 12–18   $500 – $2,000       ##
  Trial prep & trial     M 18–22   $3,000 – $8,000     ########
  Sanctions              anytime   $0                  (safe harbor → eliminated)
  ────────────────────────────────────────────────────────────────────────────
  PAYABLE AT JUDGMENT    if Plaintiffs lose:           $8,000 – $33,000
```

### Strategic implications of the V2 recalibration

**The v2-vs-v3 sanctions-based deterrent disappears.** V1 Part 2 argued v3 was meaningfully riskier than v2 because A4 (unjust enrichment) and B4 (standalone estoppel) each carried $5K–$20K sanctions exposure. With safe-harbor discipline assumed, that differential collapses to roughly zero. If there's still a reason to prefer v2 over v3, it has to come from somewhere other than Defendant cost-recovery — for example, the *time and attention* cost of defending more Rule 12 motions, or the litigation-narrative cost of inviting dismissal of weak counts in front of the trial judge. Those are real but smaller than the dollar number V1 implied.

**Rule 68 becomes the dominant Defendant-recovery vector.** With sanctions off the table, the largest single line item is post-Rule 68 disbursements if Plaintiffs reject an offer and fail to beat it at trial. Given the deductible math ($17,720 deductible against a $12,800 RCV appraisal award), a modest Defendant offer above the deductible could be hard to beat if the bad-faith and MCFA counts fail. This is the cost-recovery vector the family should actively manage:

- Issue a § 549.09 Subd. 1(b) offer of settlement contemporaneously with filing to anchor the offer/counter-offer posture.
- Track Defendant's first Rule 68 offer carefully; the moment it's served, the cost-shift clock starts and any post-offer disbursement Defendant incurs becomes recoverable if Plaintiffs ultimately fail to beat the offer.
- Don't reject reflexively — a Rule 68 offer at, say, $25,000 against a probable contract recovery of $0–$15,000 is hard to beat without the MCFA / § 604.18 paths actually delivering.

**Defendant cost-recovery is no longer a major decision driver.** At $8K–$18K (typical trial-loss scenario) or $11K–$33K (with adverse Rule 68 shift), Defendant cost recovery is roughly **a third of V1's headline number** and is dominated by routine deposition transcripts and Rule 68 mechanics rather than sanctions. The financial-risk picture is more lopsided than V1 suggested: Plaintiffs' own out-of-pocket costs (Part 1, ~$10K–$50K under Section 1.5 pro se posture) remain the primary risk, and Defendant cost-recovery is a secondary, bounded exposure.

---

## 3. Rule 68 offer/counter-offer posture — how it actually works

Section 2 above identifies Rule 68 as the dominant Defendant-recovery vector under V2. This section explains the mechanics in detail because "offer/counter-offer posture" is a lever the family directly controls and the V1 document did not develop.

### 3.1 The bilateral character of Minnesota's Rule 68

Federal Rule 68 is defendant-only — only the defendant can serve an offer of judgment. Minnesota's Rule 68 is **bilateral**: Minn. R. Civ. P. 68.01 provides that "any party may serve upon an adverse party an offer to allow judgment to be entered…" That bilateral character is the whole reason posture matters — the family can use Rule 68 offensively, not just defensively.

### 3.2 The two cost-shifting mechanics under Rule 68.03

**Mechanic 1 (Defendant's offer, Plaintiffs reject).** If Defendant serves an offer of $X, Plaintiffs reject, and the eventual judgment is ≤ $X, Plaintiffs must pay Defendant's costs and disbursements incurred *after* the offer was served.

**Mechanic 2 (Plaintiffs' offer, Defendant rejects).** If Plaintiffs serve an offer of $Y, Defendant rejects, and the eventual judgment is ≥ $Y (more favorable to Plaintiffs than the offer), Defendant must pay Plaintiffs' costs and disbursements incurred after the offer.

Neither shifts attorney fees by default — Minnesota's "costs and disbursements" terminology generally excludes fees. But the cost-shift can range from a few thousand dollars (offer served late) to $10K–$15K+ (offer served early, case proceeds for many months afterward).

### 3.3 "Posture" defined

Posture is the state of play — whose offers are currently on the table, at what dollar values, and whose cost-shift obligations get triggered depending on where the judgment lands.

| Posture state | What's at stake |
|---|---|
| Defendant has offered $X, Plaintiffs have not countered | Plaintiffs need to recover > $X or pay Defendant's post-offer costs |
| Plaintiffs have offered $Y, Defendant has not countered | Defendant needs to keep judgment < $Y or pay Plaintiffs' post-offer costs |
| Both sides have offers active | Both cost shifts can run; the one that triggers is determined by where the judgment lands relative to each offer |
| Neither side has an open offer | No cost-shift is operative; only routine § 549.04 disbursements apply |

The family controls whether they're in the second or third row by choosing to serve their own offer.

### 3.4 Why this matters concretely in this case

Given the deductible math ($17,720 deductible against the $12,800 RCV appraisal award), the realistic recovery scenarios skew low on the contract count alone — bad-faith and MCFA counts are what push the number up. Defendant's Rule 68 strategy will likely exploit this.

**Defendant's probable play.** Defendant serves a Rule 68 offer somewhere in the $20,000–$40,000 range early in the case. The number is chosen to be (a) clearly above the appraisal-deductible math, (b) somewhere Plaintiffs *might* not beat at trial if the bad-faith / MCFA paths fail, and (c) low enough that Defendant comfortably absorbs it. If Plaintiffs reject and end up recovering, say, $15,000 on the contract count with the bad-faith counts going nowhere, Plaintiffs owe Defendant's post-offer disbursements — call it $8K–$15K depending on when the offer was served.

**The counter-offer move.** Plaintiffs serve their own Rule 68 offer at a meaningful number — say $150,000 — early in the case. If Defendant rejects and Plaintiffs recover more than $150,000 (plausible if the MCFA / § 604.18 counts deliver), the cost-shift runs the other direction: Defendant owes Plaintiffs' post-offer costs. More importantly, it puts settlement pressure on Defendant by making the cost-shift bilateral rather than one-sided.

**The neutralization effect.** If both sides have active offers and the eventual judgment lands between them — Defendant offered $30K, Plaintiffs offered $150K, judgment is $75K — Plaintiffs beat Defendant's offer (no obligation to Defendant) and Plaintiffs failed to beat their own offer (no obligation from Defendant). Both cost shifts are inactive and routine § 549.04 governs. This is the "neutral posture" outcome — neither side captures the Rule 68 advantage, but neither side bears it either.

### 3.5 Connection to § 549.09 Subd. 1(b) — a different but related lever

The V1 document's recommendation to "issue a Minn. Stat. § 549.09 Subd. 1(b) offer of settlement contemporaneously with filing" is a *different* statute — **prejudgment interest**, not cost shifting. The mechanics are similar in structure but the consequence is different:

- A written settlement offer under § 549.09 Subd. 1(b) anchors **prejudgment interest accrual**. If Defendant rejects Plaintiffs' offer and the eventual judgment is *more favorable* than the offer, prejudgment interest at the statutory rate (currently 10% for judgments ≥ $50,000) compounds in Plaintiffs' favor.
- Conversely, if Defendant makes the offer and Plaintiffs reject and recover *less* than the offer, Plaintiffs lose prejudgment interest from the date of the offer forward.

On a $150,000 judgment over a ~two-year litigation timeline, that's potentially $20,000–$30,000 in prejudgment interest swinging between the parties. § 549.09 Subd. 1(b) doesn't require fee-shifting — it runs by operation of law — which is why it's worth issuing the offer at filing regardless of the rest of the strategy.

### 3.6 Three concrete effects on V2's risk picture

**First, posture determines whether the Rule 68 risk in the V2 cash-flow timeline ($0–$15,000 post-offer cost shift) runs *against* Plaintiffs or *with* them.** The line item in the Section 2 chart assumes the worst case — Defendant offers, Plaintiffs reject, Plaintiffs fail to beat the offer. A counter-offer regime can neutralize that exposure or even flip it.

**Second, posture creates settlement leverage independent of merits.** A well-anchored Plaintiffs' Rule 68 offer puts Defendant in the position where every additional month of litigation increases Defendant's potential cost-shift exposure. That changes settlement-negotiation dynamics even before the bad-faith and MCFA counts mature.

**Third, posture is a discipline problem the family can solve cheaply.** Unlike most other risk variables (which depend on counsel, court, opposing counsel, or judicial reasoning), Rule 68 posture is entirely within the family's control. The cost of serving the offer is essentially zero. The downside is essentially zero — offers expire after 10 days under Rule 68.02 if not accepted. The upside is meaningful.

So when Section 2 says the family should "actively manage" the Rule 68 vector and references "offer/counter-offer posture," what it means in practice is: **serve a Plaintiffs' Rule 68 offer early to create a bilateral cost-shift dynamic, rather than letting Defendant run a unilateral one.** That's the move that converts Rule 68 from a Defendant-side risk into a neutral or favorable strategic variable.

---

*End of V2 delta. V1 (`risk.md`) remains authoritative for everything not modified above.*

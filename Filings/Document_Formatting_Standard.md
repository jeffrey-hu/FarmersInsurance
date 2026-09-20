# Document Formatting Standard — Court Filings and Served Documents

**Scope:** every `.docx` prepared in this project for filing with the Hennepin County District Court or for service on Defendant — pleadings, discovery requests and responses, disclosures, motions, and their certificates of service.
**Reference document:** `Filings/Discovery/discoveryPlanAndInformationalStatement/Plaintiffs_Rule_26.06_Discovery_Plan_V5.docx`, filed September 4, 2026. When this file and V5 disagree, V5 governs and this file should be corrected.
**Adopted:** September 10, 2026, after aligning the four served discovery documents to V5.

> **Not legal advice.** Formatting conventions only. Rule citations here are for orientation; verify before relying on them.

---

## 1. Page setup

| Property | Value |
|---|---|
| Paper | 8.5 × 11 in |
| Margins | 1.0 in on all four sides |
| Body font | Times New Roman, 12 pt |
| Line spacing | Single |

## 2. Paragraph indentation — the core rule

Measured from V5 and now applied across the discovery package. **These are the numbers to reproduce.**

| Element | Left indent | First-line indent | Space after |
|---|---|---|---|
| Body paragraph | 0 | 0 | 8 pt |
| **Numbered or lettered list item** | **0.5"** | **−0.4" (hanging)** | **8 pt** |
| Continuation paragraph under a numbered item | 0.5" | 0 | 8 pt |
| Sub-item — `(a)`, `(b)`, field labels, an address block | 0.75" | 0 | 8 pt (4 pt in tight blocks) |
| Bulleted item | 1.0", `List Bullet` style | 0 | 4 pt |

"Numbered or lettered list item" covers all of these: Definitions entries, Instructions, every `REQUEST FOR PRODUCTION NO. n:`, `INTERROGATORY NO. n:`, and `REQUEST FOR ADMISSION NO. n:`, the numbered items in Initial Disclosures Section B, and the numbered paragraphs of a certificate of service.

### 2.1 Separator after the label — tab or spaces

- **Short label** (`1.`, `12.`, `(a)`) → follow it with a **tab**. The label sits 0.1" in from the margin and the tab carries the text to the 0.5" indent, where wrapped lines align.
- **Long label** (`REQUEST FOR PRODUCTION NO. 23:`) → keep **two spaces**. The label is already wider than 0.5", so a tab jumps to the next stop and opens a visible gap. Wrapped lines still align at 0.5".

### 2.2 Applying it in python-docx

```python
from docx.shared import Inches, Pt
pf = paragraph.paragraph_format
pf.left_indent        = Inches(0.5)
pf.first_line_indent  = Inches(-0.4)   # negative = hanging
pf.space_after        = Pt(8)
```

Verify afterward that the document has exactly **one** hanging-indent variant — `(0.5, -0.4, 8.0)`. More than one means something was missed.

## 3. Signature block

Each Plaintiff gets a complete block. A single shared "Telephone: ___ Email: ___" line is **wrong** — it cannot carry two people's details, and Minn. R. Civ. P. 26.07 requires the signer's address, email address, and telephone number on discovery requests and disclosures.

**The two blocks sit side by side, not stacked — adopted September 20, 2026.** Stacked, they run half a page and can split across a page break; side by side they read as one signature line and fit in six.

```
Dated: [date].

____________________________          ____________________________
Yibiao Lu, Plaintiff pro se           Jie Hu, Plaintiff pro se
17756 George Moran Dr.                17756 George Moran Dr.
Eden Prairie, MN 55347                Eden Prairie, MN 55347
Telephone: 763-843-2859               Telephone: 763-843-2860
Email: bill_y_lu@yahoo.com            Email: jie_h_hu@yahoo.com
```

### How it is built

**In the `.docx`:** a **borderless one-row, two-column table**, each cell 2,971,800 EMU (≈3.25") wide, `autofit=False`, Yibiao left and Jie right, six paragraphs per cell, signature rule **30 underscores**. Because the table carries no explicit borders (`tblPr` holds only `tblW`, `tblLayout`, `tblCellMar`, `tblLook`), nothing prints around it. The quickest way to reproduce it is to `copy.deepcopy` the signature table out of a document that already has one and `addnext` it after the `Dated:` paragraph — both operative First Set documents carry an identical copy.

**In the `.md` twin:** a two-column pipe table whose header row is empty, with `<br>` between the lines of each cell:

```
| | |
| --- | --- |
| \_\_\_…<br>Yibiao Lu, Plaintiff *pro se*<br>17756 George Moran Dr.<br>…<br>Email: bill\_y\_lu@yahoo.com | \_\_\_…<br>Jie Hu, Plaintiff *pro se*<br>…<br>Email: jie\_h\_hu@yahoo.com |
```

This keeps the `.md`/`.docx` verification honest: the comparison skips `.md` lines beginning with `|` and skips `.docx` table content, so the signature block is excluded from both sides rather than from only one.

### ⚠️ Page breaks live in the blank paragraphs after the table

In both documents the certificate of service begins on a fresh page, and that break is carried by an **empty paragraph containing `<w:br w:type="page"/>`** after the signature table — not by a section break. An empty paragraph is therefore **not** interchangeable with another empty paragraph. Duplicating one duplicates the page break: doing exactly that on September 20, 2026 turned a 20-page set into 22 pages with two blank pages, caught only by rendering to PDF. **After any change near the signature block or the certificate, render to PDF and scan for blank pages** — a paragraph-level `.md`/`.docx` comparison cannot see this, because the offending paragraphs are empty.

Contact details of record come from the filed Complaint and Discovery Plan V5; `LegalReferences/CaseContacts.md` agrees. Do **not** substitute any other email address.

**"Respectfully submitted,"** — a closing addressed to a tribunal. The filed Complaint and Discovery Plan V5 both omit it. Prefer omitting it on documents served on Defendant rather than filed. *(Retained in the discovery package as of this writing; not yet decided.)*

## 4. Certificate of service

**Canonical form — adopted September 20, 2026.** Use this verbatim; change only the date and the document title.

> **CERTIFICATE OF SERVICE**
>
> I, Yibiao Lu, Plaintiff *pro se*, state that on [date], I served a true and correct copy of *[document title]* upon Defendant's counsel of record, by electronic mail in the manner the parties have agreed, as a PDF attachment sent from bill_y_lu@yahoo.com to:
>
> > Kevin J. Kennedy — kkennedy@kennedylf.com
> >
> > Mary J. Baskfield — mbaskfield@kennedylf.com
> >
> > KENNEDY LAW FIRM P.C., *Counsel for Defendant Fire Insurance Exchange*
>
> Minn. R. Civ. P. 5.02(b); Minn. Gen. R. Prac. 14.03(d)(2). These discovery requests are served, not filed. Minn. R. Civ. P. 5.04(b).
>
> I declare under penalty of perjury that everything I have stated in this document is true and correct. Minn. Stat. § 358.116.
>
> Dated: [date], at Eden Prairie, Hennepin County, Minnesota.
>
> \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
>
> Yibiao Lu, Plaintiff *pro se*

For a non-discovery document, replace the served-not-filed sentence accordingly (for disclosures: "These disclosures are served, not filed."). The signature rule is **36 underscores** in both the `.docx` and the `.md`, so the two verify as identical.

### What the rules actually require

**Minn. R. Civ. P. 5.04(b)** prescribes the entire content of a certificate: it must specify "the details of how and when service was accomplished" and be "signed under oath or penalty of perjury by the person effecting service." **Minn. Stat. § 358.116** adds the declaration sentence substantially as written, the signature below it, and the **date, county and state** of signing. **Minn. Gen. R. Prac. 14 prescribes no certificate contents at all** — 14.05 makes the E-Filing System's own records sufficient proof only where that system is used, which is not how these parties serve. Nothing else is required.

### What was deliberately removed, and why

| Removed | Why |
|---|---|
| "I am over the age of 18 years and a Plaintiff in this action" | Imported from the Judicial Branch **affidavit of service** form, which exists for **Rule 4** service of process. Rule 4.02 requires a server "not less than 18 years of age **and not a party to the action**" — a rule under which being a party would *disqualify* the server. It has no application to Rule 5 service on an appearing party's counsel, which is why a pro se party may serve their own discovery. |
| "I personally made the service described below" | Duplicates "I served" in the operative sentence. |
| Numbered ¶¶ 1–4 | One event. The numbering stretched four lines of substance across most of a page. |
| Attorney registration numbers | Not required: the number requirement runs to the **signer** (Rule 11.01; Gen. R. Prac. 14.04(b)(1)), not the recipient. They were also unverifiable — see the warning below. |
| Counsel's street address | Not a detail of *how* email service was accomplished; the email addresses are. It also made the lead-in "addressed as follows" inaccurate, since the message was not addressed to a street. |
| `Signature of person who served the documents` caption, and the `Name:` / `Address:` / `City/State/Zip:` / `Telephone:` / `E-mail address:` block | From the same Rule 4 affidavit form. The server's contact details already appear in the document's own signature block, and a discovery certificate is never filed, so no clerk checks it against that form. |

Governing principle: the certificate is sworn under penalty of perjury, so it should contain **what the rule requires and what proves service, and nothing else**. Every additional recital is one more thing to be accurate about, for no gain. If service is contested, the proof is the sent message and its full headers — which is why the certificate names the **sending address**, and why the exact transmission time goes in `Filings/Discovery/Service_Log.md` rather than in a blank on a document signed before the send.

### ⚠️ Do not use the sworn-affidavit preamble

"[Name], being first duly sworn on oath, deposes and states…" is a **jurat** formula. It means something only where a notary administers the oath and signs below. Rule 5.04(b) permits service to be certified "under oath **or** penalty of perjury," and § 358.116 is the no-notary route these filings use. **Never combine the two**: reciting an oath that was never administered puts a false statement in a document signed under penalty of perjury.

FIE's own **Affidavit of Service dated August 10, 2026** (`OfficialCourtDocuments/08_10_2026_MCRO_27-CV-26-11606_Affidavit of Service_...pdf`) does exactly that — it opens "Julie Parks, being first duly sworn on oath, deposes and states," carries **no notary block, signature or seal**, then falls back on § 358.116, and omits the county and state of signing that § 358.116 requires. It is not a model to copy.

### 4.1 Which certificate to use

**Default — electronic mail.** Use the canonical block in §4 above. Its recital *"by electronic mail in the manner the parties have agreed. Minn. R. Civ. P. 5.02(b); Minn. Gen. R. Prac. 14.03(d)(2)"* has been accurate since the parties' **September 14, 2026** agreement (`KeyDecisions.md` Decision 4). The certificate carries **no time blank** — it is signed before transmission, so a recited clock time could not be true at signing. Record the exact transmission time in `Filings/Discovery/Service_Log.md` instead, because a transmission after 5:00 p.m. Minnesota time adds a day under Rule 6.01(e).

**Exception — U.S. mail.** Use the mail certificate (¶1 reciting that service by mail is complete upon mailing) only where a rule, statute, or order requires mail or personal service, or where a document is too large to email. Retain a signed original; consider USPS Form 3817 as independent proof of the mailing date.

**Rules that follow from this:**

- **Serve counsel, not the party.** Kennedy Law Firm P.C. appeared July 28, 2026. Minn. R. Civ. P. 5.02(a): "service shall be made upon the attorney unless service upon the party is ordered by the court." Never serve FIE's registered agent while counsel is of record. Serve kkennedy@kennedylf.com and mbaskfield@kennedylf.com. **Do not put attorney registration numbers in anything you sign** — they are not required, and Kennedy Law's own filings disagree: the Notice of Appearance (7/28/2026) gives Baskfield as **0314572**, the Answer (8/10/2026) as **#354172**, and MARS could not be checked (reCAPTCHA). Open item I-5.
- **One signer — the person who actually mailed it.** Both Plaintiffs sign the document's own signature block; only the person effecting service signs the certificate.
- **State the manner as fact**, not as a menu of bracketed options.
- **Retain a signed original; never file it.** Rule 5.04(b) bars filing discovery. Consider a USPS Certificate of Mailing (Form 3817) as independent proof of the mailing date.
- **⚠️ Day counts differ by manner of service — and email is now the default.** Since the **September 14, 2026** agreement the parties serve by email (`KeyDecisions.md` Decision 4).

  | Manner | Service complete | Days added | Authority |
  |---|---|---|---|
  | **Email (default)** | **upon transmission** | **0** — or **+1** if transmitted after **5:00 p.m.** Minnesota time | Gen. R. Prac. 14.03(e); R. Civ. P. 6.01(e) |
  | U.S. Mail (exception) | upon mailing | **+3** | R. Civ. P. 5.02(c); 6.01(e) |

  Rule 6.01(a) rolls a deadline landing on a weekend or holiday to the next business day. **Calculate and calendar the real date on the day you serve**, and do the same for every document Defendant serves on Plaintiffs — email service is complete on transmission with **no failed-delivery exception**, so the clock runs whether or not the message is seen.

## 5. Caption block

Two-column table at the top: `STATE OF MINNESOTA / COUNTY OF HENNEPIN` and `DISTRICT COURT / FOURTH JUDICIAL DISTRICT` in the first row; parties on the left and `Case Type: Contract`, `Court File No. 27-CV-26-11606`, `Judge: Jamie Anderson` on the right.

## 6. Typography

- **Straight** double quotes in the discovery documents (matches what is there); curly apostrophes appear in existing text — do not mass-convert.
- Em dashes `—` for parenthetical breaks.
- Case names in *italics*; document titles in *italics* inside a certificate of service.

## 7. Numbering discipline

- Number each set from 1. A second set restarts at 1; it does not continue the first set's numbering.
- **Renumbering is safe only before service.** Once served, the numbers are fixed — Defendant's responses and any motion to compel cite them. After service, withdraw a request by letter and **leave the gap**; never renumber.

## 8. Keeping the `.md` twin in sync

Several documents have a Markdown twin for review. It is generated from the `.docx`, which is authoritative:

```bash
pandoc -f docx -t gfm --wrap=none INPUT.docx -o /tmp/t.md
# then replace the leading <table>…</table> with the standard Markdown caption block
```

Markdown carries no indentation, so §2 changes are invisible in the `.md`. Regenerate the twin after any `.docx` edit so the two do not drift.

**Watch the filename.** Regenerate to the twin's **actual** path, not to the `.docx` basename. As of the September 11, 2026 reorganization the RFP twin is named `[Current] Plaintiffs_First_Set_of_Requests_for_Production_to_FIE.md`; regenerating under the plain name would create a second, competing copy. When a document has more than one Markdown file, the `.docx` is authoritative and the others are dated baselines — label them so (`[Original 2026-09-08] …`) and never regenerate over them.

---

## Change log

| Date | Change |
|---|---|
| 2026-09-20 | **§3: the two Plaintiffs' signature blocks go side by side** in a borderless 1×2 table (`.docx`) and a two-column pipe table (`.md`), applied to the Interrogatories and the Requests for Admission. Recorded the page-break-in-an-empty-paragraph hazard and the render-and-scan check that catches it. |
| 2026-09-20 | **§4 rewritten: canonical certificate of service adopted.** The over-18 recital, "personally made," the ¶1–¶4 numbering, attorney registration numbers, counsel's street address, and the Judicial Branch server-identification block were all removed as surplus to Rule 5.04(b) and § 358.116; the sworn-affidavit ("duly sworn on oath") preamble is prohibited without a notary. Applied to the First Set Interrogatories and Requests for Admission the same day. Stray "September 15, 2026" e-service agreement dates corrected to **September 14**. |
| 2026-09-15 | Parties agreed to service by email (`KeyDecisions.md` Decision 4). §4 day-count warning replaced with a per-manner table; new §4.1 makes the email certificate the default and the mail certificate the exception. |
| 2026-09-11 | Noted the `FirstSetDiscovey/` split into `Interrogatories/` and `Request For Production/`, and the filename caution in §8. |
| 2026-09-10 | Adopted. Indentation aligned to V5 across the Requests for Production, Interrogatories, Requests for Admission, and Initial Disclosures (165 list items). Signature blocks rebuilt per Rule 26.07. Certificates of service replaced per Rule 5.04(b) and § 358.116. |

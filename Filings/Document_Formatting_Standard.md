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

```
Dated: [date].

____________________________________
Yibiao Lu, Plaintiff pro se
17756 George Moran Dr.
Eden Prairie, MN 55347
Telephone: 763-843-2859
Email: bill_y_lu@yahoo.com

____________________________________
Jie Hu, Plaintiff pro se
17756 George Moran Dr.
Eden Prairie, MN 55347
Telephone: 763-843-2860
Email: jie_h_hu@yahoo.com
```

Contact details of record come from the filed Complaint and Discovery Plan V5; `LegalReferences/CaseContacts.md` agrees. Do **not** substitute any other email address.

**"Respectfully submitted,"** — a closing addressed to a tribunal. The filed Complaint and Discovery Plan V5 both omit it. Prefer omitting it on documents served on Defendant rather than filed. *(Retained in the discovery package as of this writing; not yet decided.)*

## 4. Certificate of service

Model: `Filings/SummonsAndComplaint/Court/NonComplianceNotice/AffidavitOfService/Certificate_of_Service_Corrected_Filing_Lu_Hu_FINAL.docx`, and as applied to the discovery package on September 10, 2026.

Required elements, per Minn. R. Civ. P. 5.04(b) and Minn. Stat. § 358.116:

1. Heading `CERTIFICATE OF SERVICE`.
2. `I, [name], state and declare as follows:`
3. Numbered ¶1 — declarant is over 18, is a Plaintiff, and **personally made** the service; recite Minn. R. Civ. P. 5.02 and that service by mail is **complete upon mailing**.
4. Numbered ¶2 — date of service, the document served (title in *italics*), the manner, and the full name and address served.
5. Numbered ¶3 — "These discovery requests are served, not filed, in accordance with Minn. R. Civ. P. 5.04(b)." (For disclosures: "These disclosures are served, not filed…".)
6. `I declare under penalty of perjury that everything I have stated in this document is true and correct. Minn. Stat. § 358.116.`
7. `Dated: [date], at Eden Prairie, Hennepin County, Minnesota.` — § 358.116 requires the **date, county, and state** of signing.
8. **One** signature line, labeled `Signature of person who served the documents`, then the server's identification block, matching the Judicial Branch forms (HOU111; SOP105; Conciliation Court Affidavit of Service): `Name:` / `Address:` / `City/State/Zip:` / `Telephone:` / `E-mail address:`, each label followed by a tab to a 1.4" tab stop, 0 pt between the lines and 8 pt after the last. No rule requires this block — Rule 5.04(b) asks only for how and when, and Minn. Stat. § 358.116 for the declaration, signature, date, county and state — but every official Minnesota form carries it, and it identifies and locates the server on the face of the certificate if service is ever contested. The `E-mail address:` must be the same address the certificate recites as the sending address.

### 4.1 Which certificate to use

**Default — electronic mail.** Use the email certificate at Part 2 of `Discovery/Proposed_EService_Stipulation_and_Certificate_2026-09-14.md`. Its ¶1 recites *"by electronic mail, in the manner the parties have agreed. Minn. R. Civ. P. 5.02(b); Minn. Gen. R. Prac. 14.03(d)(2),"* which has been accurate since the parties' **September 15, 2026** agreement, and its ¶2 records the **date and time** of transmission — record the time, because a transmission after 5:00 p.m. Minnesota time adds a day under Rule 6.01(e).

**Exception — U.S. mail.** Use the mail certificate (¶1 reciting that service by mail is complete upon mailing) only where a rule, statute, or order requires mail or personal service, or where a document is too large to email. Retain a signed original; consider USPS Form 3817 as independent proof of the mailing date.

**Rules that follow from this:**

- **Serve counsel, not the party.** Kennedy Law Firm P.C. appeared July 28, 2026. Minn. R. Civ. P. 5.02(a): "service shall be made upon the attorney unless service upon the party is ordered by the court." Never serve FIE's registered agent while counsel is of record. Address: Kevin J. Kennedy (#193872) and Mary J. Baskfield (#0314572), 7616 Currell Blvd., Suite 270, Woodbury, MN 55125.
- **One signer — the person who actually mailed it.** Both Plaintiffs sign the document's own signature block; only the person effecting service signs the certificate.
- **State the manner as fact**, not as a menu of bracketed options.
- **Retain a signed original; never file it.** Rule 5.04(b) bars filing discovery. Consider a USPS Certificate of Mailing (Form 3817) as independent proof of the mailing date.
- **⚠️ Day counts differ by manner of service — and email is now the default.** Since September 15, 2026 the parties serve by email by agreement (`KeyDecisions.md` Decision 4).

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
| 2026-09-15 | Parties agreed to service by email (`KeyDecisions.md` Decision 4). §4 day-count warning replaced with a per-manner table; new §4.1 makes the email certificate the default and the mail certificate the exception. |
| 2026-09-11 | Noted the `FirstSetDiscovey/` split into `Interrogatories/` and `Request For Production/`, and the filename caution in §8. |
| 2026-09-10 | Adopted. Indentation aligned to V5 across the Requests for Production, Interrogatories, Requests for Admission, and Initial Disclosures (165 list items). Signature blocks rebuilt per Rule 26.07. Certificates of service replaced per Rule 5.04(b) and § 358.116. |

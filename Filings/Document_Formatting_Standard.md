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
| **Numbered or lettered list item** | **0.5"** | **−0.5" (hanging)** | **8 pt** |
| Continuation paragraph under a numbered item | 0.5" | 0 | 8 pt |
| Sub-item — `(a)`, `(b)`, field labels, an address block | 0.75" | 0 | 8 pt (4 pt in tight blocks) |
| Bulleted item | 1.0", `List Bullet` style | 0 | 4 pt |

"Numbered or lettered list item" covers all of these: Definitions entries, Instructions, every `REQUEST FOR PRODUCTION NO. n:`, `INTERROGATORY NO. n:`, and `REQUEST FOR ADMISSION NO. n:`, the numbered items in Initial Disclosures Section B, and the numbered paragraphs of a certificate of service.

### 2.1 Separator after the label — tab or spaces

- **Short label** (`1.`, `12.`, `(a)`) → follow it with a **tab**. With a 0.5" hanging indent the text lands exactly on the indent. This is what V5 does.
- **Long label** (`REQUEST FOR PRODUCTION NO. 23:`) → keep **two spaces**. The label is already wider than 0.5", so a tab jumps to the next stop and opens a visible gap. Wrapped lines still align at 0.5".

### 2.2 Applying it in python-docx

```python
from docx.shared import Inches, Pt
pf = paragraph.paragraph_format
pf.left_indent        = Inches(0.5)
pf.first_line_indent  = Inches(-0.5)   # negative = hanging
pf.space_after        = Pt(8)
```

Verify afterward that the document has exactly **one** hanging-indent variant — `(0.5, -0.5, 8.0)`. More than one means something was missed.

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
8. **One** signature line, labeled `Signature of person who served the documents`, then the printed name.

**Rules that follow from this:**

- **Serve counsel, not the party.** Kennedy Law Firm P.C. appeared July 28, 2026. Minn. R. Civ. P. 5.02(a): "service shall be made upon the attorney unless service upon the party is ordered by the court." Never serve FIE's registered agent while counsel is of record. Address: Kevin J. Kennedy (#193872) and Mary J. Baskfield (#0314572), 7616 Currell Blvd., Suite 270, Woodbury, MN 55125.
- **One signer — the person who actually mailed it.** Both Plaintiffs sign the document's own signature block; only the person effecting service signs the certificate.
- **State the manner as fact**, not as a menu of bracketed options.
- **Retain a signed original; never file it.** Rule 5.04(b) bars filing discovery. Consider a USPS Certificate of Mailing (Form 3817) as independent proof of the mailing date.
- **⚠️ Service by U.S. Mail adds 3 days.** Minn. R. Civ. P. 6.01(e). A 30-day response period becomes **33 days from the date of mailing**, and Rule 6.01(a) rolls a deadline landing on a weekend or holiday to the next business day. Calendar the real date on the day you mail.

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
| 2026-09-11 | Noted the `FirstSetDiscovey/` split into `Interrogatories/` and `Request For Production/`, and the filename caution in §8. |
| 2026-09-10 | Adopted. Indentation aligned to V5 across the Requests for Production, Interrogatories, Requests for Admission, and Initial Disclosures (165 list items). Signature blocks rebuilt per Rule 26.07. Certificates of service replaced per Rule 5.04(b) and § 358.116. |

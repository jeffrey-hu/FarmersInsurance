# Using Public Web Pages and Scientific Literature — Disclosure and Admissibility

**Case:** *Lu and Hu v. Fire Insurance Exchange*, No. 27-CV-26-11606
**Prepared:** September 6, 2026 · Rule citations verified against the Minnesota Rules of Evidence

> **Not legal advice.** I am not a lawyer. Confirm each rule independently and have a Minnesota-licensed attorney review before relying on this.

---

## The short version

**Disclosing** a public source is easy: you disclose the **saved copy you hold**, with its URL and the date you captured it.

**Using** one at trial is where the sources split into three tracks with very different rules — and the peer-reviewed hail papers are the constrained one. Under **Minn. R. Evid. 803(18)**, a scientific paper reaches the factfinder **only through an expert**, and even then it **"may be read into evidence but may not be received as exhibits."** The jury never gets the paper.

---

## 1. How to describe a public source in Section B

Minn. R. Civ. P. 26.01(a)(1)(B) reaches documents and ESI "that the disclosing party **has in its possession, custody, or control** and may use to support its claims or defenses."

A live web page is not in anyone's possession. **The PDF or printout you saved is.** So disclose the saved copy, and identify four things:

| Element | Why |
|---|---|
| Title, author or issuing body, publication date | Identifies the item |
| **URL** | Lets the other side retrieve it |
| **Date accessed or captured** | Web pages change. The copy you captured on a date certain is the evidence — the live page is not |
| That a copy is in Plaintiffs' possession and available for inspection | Satisfies the rule's possession element and the Rule 34 availability requirement |

**Example of the form:**

> National Weather Service, Twin Cities/Chanhassen, "Significant Wind and Hail in Minnesota — July 13–14, 2024," published at [URL], as captured by Plaintiffs on [date]. A copy is in Plaintiffs' possession and available for inspection and copying.

**Keep the capture clean.** Save as PDF with the URL and date printed in the header or footer, keep the file unaltered, and note where the original is stored. If a page later changes or disappears, that capture is what you have.

---

## 2. Three tracks of admissibility

### Track A — Government publications (NWS/NOAA, City permits)

The easiest track, and it needs no witness.

- **Authentication:** self-authenticating as official publications, **Minn. R. Evid. 902(5)** ("[b]ooks, pamphlets, or other publications purporting to be issued by public authority"). Certified copies self-authenticate under **902(4)**.
- **Hearsay:** the public-records exception, **Minn. R. Evid. 803(8)**.
- **The strongest route — judicial notice.** Under **Minn. R. Evid. 201(b)**, a court may notice a fact "capable of accurate and ready determination by resort to sources whose accuracy cannot reasonably be questioned." Official NWS storm data fits squarely. Two features make this attractive: under **201(d)** the court **shall** take judicial notice when a party requests it and supplies the necessary information; and under **201(g)** the jury is instructed to accept a noticed fact **as conclusive**. Available "at any stage of the proceeding" under **201(f)**.

For the July 13–14, 2024 storm, a judicial-notice request supported by certified NCEI records is stronger and cheaper than any witness. See `CaseContacts.md` on ordering certified copies without a subpoena.

### Track B — Commercial data sites (stormersite, Interactive Hail Maps)

Private companies, so no 902(5).

- **Authentication:** a witness with knowledge, or distinctive characteristics under **Minn. R. Evid. 901(b)(4)**.
- **Hearsay:** **Minn. R. Evid. 803(17)** — "[m]arket quotations, tabulations, lists, directories, or other published compilations, **generally used and relied upon by the public or by persons in particular occupations**." Hail-mapping data used by adjusters and forensic engineers fits the "particular occupations" language.
- **The point that does the work here:** **Prieve's own report relied on stormersite.** Defendant's retained engineer used the source, which is strong evidence that it is "generally used and relied upon by persons in particular occupations" — and an awkward position from which to attack it. Preserve that: the Weather Records section of File #241008 cites stormersite and the NOAA Storm Events Database.
- Also available as expert-reliance material under **Minn. R. Evid. 703**.

### Track C — Peer-reviewed scientific papers ⚠️

This is the constrained track, and it governs everything in `HailShapes/AcademicPapers_Claude/`.

**Minn. R. Evid. 803(18), quoted in full:**

> "To the extent called to the attention of an expert witness upon cross-examination or relied upon by the expert witness in direct examination, statements contained in published treatises, periodicals, or pamphlets on a subject of history, medicine, or other science or art, established as a reliable authority by the testimony or admission of the witness or by other expert testimony or by judicial notice. **If admitted, the statements may be read into evidence but may not be received as exhibits.**"

Three consequences:

1. **An expert is mandatory.** The paper enters only when relied on by an expert on direct, or put to an expert on cross. There is no route by which Plaintiffs hand a paper to the factfinder themselves.
2. **The paper must be established as a reliable authority** — by the witness's admission, by other expert testimony, or by judicial notice.
3. **The jury never receives it.** Statements are read aloud into the record; the document does not go back to the jury room. Plan the examination around specific passages, not around the document.

**Two vehicles in this case:**

- **Direct** — Plaintiffs' retained forensic engineer or meteorologist relies on the literature in forming an opinion (803(18) plus **Minn. R. Evid. 703**).
- **Cross** — confronting Nathan Prieve with published authority, if established as reliable. This is the natural home for the attack pleaded at Complaint ¶ 22(i): that hailstones are commonly irregular and lobed and that wind-driven hail strikes at oblique angles, contradicting Prieve's "smooth or rounded dents only" diagnostic.

> ### ⚠️ Without a retained expert, the hail-science literature is inert.
> Complaint ¶ 22(i) — the methodological core of the attack on the Prieve report — rests entirely on peer-reviewed literature that **Rule 803(18) will not admit without an expert.** This is the strongest practical argument for retaining the forensic engineering and meteorology experts on schedule. A folder of excellent papers proves nothing standing alone.

---

## 3. Timing — most of the literature is *not* disclosed on September 25

This is the practical answer to "how do we disclose the papers."

| Material | Disclosed under | When |
|---|---|---|
| Weather records, permits, and public pages Plaintiffs submitted to Defendant during the claim | Rule 26.01(a)(1)(B), Section B | **September 25, 2026** |
| Scientific literature an expert will rely on | **Rule 26.01(b)** expert disclosures, with the expert's report | The Scheduling Order date (Plaintiffs proposed September 24, 2027) |

Because a paper reaches the factfinder only through an expert, the literature the expert relies on travels with the expert disclosure. **Do not itemize fifteen academic papers in the September 25 Section B.** Doing so telegraphs the expert's theory a year before the expert is retained, and the expert will select their own authorities regardless.

**Recommended hedge:** disclose one modest *category* now, which is exactly what "a description by category" permits, preserving the option at no cost:

> Published scientific and technical literature concerning hail formation, hailstone morphology, hail fall dynamics, and impact damage to building components, in Plaintiffs' possession.

See `Filings/Discovery/InitialDisclosure/Proposed_Changes_Initial_Disclosures_2026-09-06.md` **P-3C**.

---

## 4. Two cautions on the literature itself

**Verify every citation against the actual paper before it appears in any filing.** Check that the paper exists, that the authors and journal are as stated, and that it says what it is cited for. Courts have sanctioned litigants for citations that did not hold up. The folder `HailShapes/AcademicPapers_Claude/` was assembled with AI assistance; the PDFs in it are real papers, but **any summary of a paper is not the paper**. Quote from the PDF, with page numbers.

**Let the expert choose the authorities.** A retained expert will rely on the literature they consider authoritative in their field, and 803(18) requires the paper to be "established as a reliable authority." A paper the expert has not read and will not vouch for is worse than useless — it invites impeachment of your own expert. Provide the folder to the expert as a starting point, not as a required reading list.

---

## Rule index

| Rule | Use |
|---|---|
| Minn. R. Civ. P. 26.01(a)(1)(B) | Disclose the saved copy you possess, by category and location |
| Minn. R. Civ. P. 26.01(b) | Expert disclosures — where the literature actually travels |
| Minn. R. Evid. 201(b), (d), (f), (g) | Judicial notice of government weather data; conclusive for the jury |
| Minn. R. Evid. 703 | Expert may rely on data reasonably relied upon in the field |
| Minn. R. Evid. 803(8) | Public records exception |
| Minn. R. Evid. 803(17) | Commercial compilations relied on in particular occupations |
| **Minn. R. Evid. 803(18)** | **Learned treatises — expert only, read not received** |
| Minn. R. Evid. 901(b)(4) | Authentication by distinctive characteristics |
| Minn. R. Evid. 902(4), (5) | Certified public records; official publications — self-authenticating |

> Reminder from `CaseContacts.md`: Minnesota did **not** adopt Fed. R. Evid. 902(11). There is no certified-business-record shortcut in Minnesota state court; business records need a live foundation under Minn. R. Evid. 803(6). Public records under 902(4) and 902(5) are the exception.

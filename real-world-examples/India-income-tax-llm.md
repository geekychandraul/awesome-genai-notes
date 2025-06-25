https://scr.sci.gov.in/scrsearch/
To train an LLM on Indian tax laws, you'll need a comprehensive, structured set of legal documents—covering acts, rules, finance bills, notifications, and case law. Here's where to find reliable sources:

---

## 📂 1. Acts & Statutes (Machine-Readable PDFs)

* **Income‑Tax Act, 1961**:

  * Full text via IndiaCode: “THE INCOME‑TAX ACT, 1961” ([indiacode.nic.in][1])
  * Updated version (post Finance Act 2024) in PDF form ([datocms-assets.com][2])
* **Income‑Tax Rules, 1962**: Consolidated file with 2024 amendments ([thc.nic.in][3])
* **Wealth‑Tax Act, 1957**: PDF via IndiaCode ([indiacode.nic.in][4])
* **Gift‑Tax Act, 1958**: PDF via IndiaCode ([indiacode.nic.in][5])
* **Interest‑Tax Act, 1974**: PDF via IndiaCode ([indiacode.nic.in][6])
* **Central Sales Tax Act, 1956** and other state VAT/Profession tax acts ([indiacode.nic.in][7])
* **GST Act, 2017**: PDF via IndiaCode ([indiacode.nic.in][8])

🛠️ *Tip:* Use automated scripts to bulk-download PDFs from IndiaCode's standardized URLs.

---

## 🧾 2. Finance Acts & Budget Documents

* **Finance Bill 2025**: Full PDF of current year's amendments ([indiabudget.gov.in][9])
* Prior Finance Acts (2000–2024): Often found on government or budget portals like `indiabudget.gov.in`.

---

## 📜 3. Notifications, Circulars & Amendments

* **Income Tax Department portal**: Hosts circulars, orders, rules updates—such as recent notifications under Income‑Tax Rules, 1962 ([indiabudget.gov.in][9], [thc.nic.in][3]).
* Scrape “Circulars/Orders” and “Notifications” sections.

---

## 📚 4. Case Law & Judicial Interpretations

* **National Judicial Reference System (NJRS)**: Planned repository for all direct tax appellate decisions from tribunals, HC, SC ([en.wikipedia.org][10]). Access may require government credentials.
* **Court Websites**: Supreme Court judgments (via api.sci.gov.in), High Courts, Tax Tribunal archives.
* **Aggregators**: Platforms like IndianKanoon provide scraped metadata and searchable judgments.

---

## 🔧 5. Putting It All Together: Corpus Assembly

1. **Acts + Rules**: Download PDFs of statutes from IndiaCode.
2. **Amendments**: Finance Bills, Acts, and Notifications for yearly updates.
3. **Jurisprudence**: Collect judgments from courts—use scripted scraping of listings (e.g. SC, High Courts, ITAT).
4. **Parse & Clean**: Convert PDFs to text/JSON, normalize formatting, tag sections/clauses.
5. **Metadata Enrichment**: Include cross-references to sections, dates, issuing authority.

---

## ✅ Summary

You can obtain all necessary doc sources:

* **Statutes & Rules**: via IndiaCode and Income‑Tax Dept sites
* **Annual Amendments**: via Finance Acts/Bills and notifications
* **Tax Case Law**: via NJRS (if accessible), court portals, and legal aggregators

This combination will provide a robust tax-law corpus for LLM training. Would you like help writing scripts to automate PDF downloads or for corpus parsing?

[1]: https://www.indiacode.nic.in/bitstream/123456789/2435/1/a1961-43.pdf?utm_source=chatgpt.com "[PDF] THE INCOME-TAX ACT, 1961 ARRANGEMENT OF SECTIONS"
[2]: https://www.datocms-assets.com/40521/1719632426-income-tax-act-as-amended-by-finance-act-2024.pdf?utm_source=chatgpt.com "[PDF] INCOME-TAX ACT, 1961 - 2024"
[3]: https://thc.nic.in/Central%20Governmental%20Rules/Income%20Tax%20Rules%2C1962%28All%20Amendmnets%20of%202024%29.pdf?utm_source=chatgpt.com "[PDF] Income-Tax Rules,1962 ( All Amendments & Circulars etc of 2024)"
[4]: https://www.indiacode.nic.in/bitstream/123456789/3123/1/a1957-27.pdf?utm_source=chatgpt.com "[PDF] THE WEALTH-TAX ACT, 1957 ARRANGEMENT OF SECTIONS"
[5]: https://www.indiacode.nic.in/bitstream/123456789/2483/1/a1958-18.pdf?utm_source=chatgpt.com "[PDF] THE GIFT-TAX ACT, 1958 ______ - India Code"
[6]: https://www.indiacode.nic.in/bitstream/123456789/1616/1/197445.pdf?utm_source=chatgpt.com "[PDF] 1 THE INTEREST-TAX ACT, 1974 - India Code"
[7]: https://www.indiacode.nic.in/bitstream/123456789/15258/1/3_cst_act_central_sales_tax_act_1956.pdf?utm_source=chatgpt.com "[PDF] The Central Sales Tax Act, 1956 (Act No. 74 of 1956) - India Code"
[8]: https://www.indiacode.nic.in/bitstream/123456789/16471/1/goods_and_services_tax_act%2C_2017.pdf?utm_source=chatgpt.com "[PDF] GOODS AND SERVICES TAX ACT, 2017 | India Code"
[9]: https://www.indiabudget.gov.in/doc/Finance_Bill.pdf?utm_source=chatgpt.com "[PDF] THE FINANCE BILL, 2025 - Union Budget"
[10]: https://en.wikipedia.org/wiki/National_Judicial_Reference_System?utm_source=chatgpt.com "National Judicial Reference System"

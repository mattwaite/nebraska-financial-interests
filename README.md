# Who discloses what: Nebraska statements of financial interests

A searchable, single-page view of Form C-1 (Statement of Financial Interests) filings by Nebraska candidates, elected officials, appointees and state employees. Prototype built for the Flatwater Free Press.

**Live page:** https://www.mattwaite.com/nebraska-financial-interests/

## What it does
- One search box: type a person's name to open their filings and itemized sources, or a county or city to list everyone tied to it.
- Counts by office, county and city, a county map, and a searchable list of income sources, businesses and holdings.
- Every filing links back to the original on the Nebraska Accountability and Disclosure Commission (NADC) site.

## Where the data comes from
- **1992 to mid-2022:** NADC's bulk download of Form C-1 data. NADC has not updated it since.
- **2021 to 2026:** collected from NADC's search site (nadc-e.nebraska.gov) on 2026-10-30: 14,164 filings, 14,037 of them downloaded as PDFs.
- **Electronic filings (7,376):** parsed by software into 75,855 itemized entries.
- **Scanned, mostly handwritten filings (6,661):** read by an AI model (Claude Haiku), producing 63,837 entries. These are labeled **machine-read, unverified** in the page. Always check the linked original.

## Caveats
- Form C-1 reports no dollar amounts.
- Itemized sources exist for 1996-2003 and 2021 onward, not 2004-2020.
- People are matched across years by name only, so namesakes can be combined.
- Home counties are approximate (from the filer's ZIP code). Street addresses, PO boxes and phone numbers are left out.
- AI-read entries can contain misreadings of handwriting. They have not been checked by a person beyond spot examples.

## Notes
- The page asks search engines not to index it (`noindex`, `robots.txt`).
- Source files, scrapers and parsers are not in this repository. This repository holds only the built page.
- County boundaries and ZIP centroids: U.S. Census Bureau.

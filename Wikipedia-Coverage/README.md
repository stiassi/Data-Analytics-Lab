This project analyzes algorithm coverage in English vs. German Wikipedia using Wikidata SPARQL.

1. Evaluated Data Sources
Tested XML dumps, HuggingFace datasets, Wiki40b — all too large, outdated, or incomplete.
Chose Wikidata SPARQL for real-time, precise, language-aware querying.

2. Extracted Algorithm Articles
Wrote Python + SPARQL scripts to find items subclass of Q8366 (algorithm) with language-specific Wikipedia links:
- English: 1,453 articles
- German: 447 articles

3. Detected Coverage Gaps across languages:
- 543 algorithms exist in EN but missing in DE
- 47 algorithms exist in DE but missing in EN

4. Validated Results Manually
Confirmed most gaps are real. Some topics only appear as subsections (e.g., Quadrupelbauer in DE → part of "Doubled pawns" in EN).
Noted issue: inconsistent Wikidata modeling (e.g., chess tactics tagged as algorithms).

5. Proposed Action Plan
- Clarify "algorithm" definition in Wikidata
- Fix broken/broad classifications
- Improve missing language links & descriptions
- Build tools to detect gaps & suggest translations
- Encourage cross-language article creation

Goal: Help make Wikipedia’s algorithm knowledge complete, accurate, and multilingual.
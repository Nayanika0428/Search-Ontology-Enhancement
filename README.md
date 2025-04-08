# Search-Ontology-Enhancement
This project was originally developed during my time at a biopharma company as part of a larger search optimization initiative.

# Synonym Enrichment for Disease Terms

## 📌 Objective
Improve the quality of search results by enriching disease term synonyms in a biomedical ontology using external APIs.

## 🛠️ Tech Stack
- Python
- REST API
- JSON
- MySQL
- Knowledge Graph

## 📈 Problem Statement
During a search relevance analysis, it was observed that certain acronyms and keyword expansions were poorly handled. For example, the term "AML" (Acute Myeloid Leukemia) often returned results for a specific subtype (APML), missing the broader context.

## ⚙️ What the Script Does
- Takes a list of disease terms
- Calls an external API for each term
- Extracts synonyms (handling pagination)
- Updates/enriches the internal ontology

## 🧪 Example Use Case
Query: `npm-1 mutated cell-lines in AML`

Expected: Synonyms for AML (Acute Myeloid Leukemia)

Before: Only APML results  
After: Broader AML context added through enriched synonyms.

## 🔁 Improvements Made
- Added new synonyms from external APIs
- Improved keyword match performance
- Enhanced overall 20% relevance in search outputs

## 🚧 Limitations
- API supports only single-term requests (no batching)
- Pagination increases runtime significantly

## 📍 Next Steps
- Batch API support for efficiency
- Clean synonyms added to Knowledge Graph for production use


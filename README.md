Video link -



# Agentic Review Trend Analysis (Zomato)

This project implements an agentic AI pipeline to analyze Google Play Store reviews for Zomato and generate topic-level trend reports over time.

The system ingests daily review batches and produces a trend table showing how issues, requests, and feedback evolve across dates.

---

## Approach

- Reviews are processed daily, treating each date as a batch.
- An LLM-based agent extracts high-recall topics from each review.
- A canonicalization agent aggressively merges semantically similar topics into stable canonical categories.
- This prevents topic fragmentation (e.g., “delivery guy was rude” vs “delivery partner behaved badly”).
- Daily topic counts are aggregated into a trend report.


---

## Output

The output is a table where:
- Rows represent canonical topics
- Columns represent dates
- Cell values indicate topic frequency on that date

Sample outputs are provided in the `/output` folder.



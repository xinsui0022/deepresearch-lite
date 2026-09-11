# DeepResearch Lite - Requirements

## 1. Project Goal

Build a lightweight AI research workflow that can:

1. Accept a user research topic.
2. Decompose the topic into multiple search queries.
3. Search for relevant web sources.
4. Remove duplicate or low-value sources.
5. Crawl selected pages.
6. Extract structured evidence related to the research topic.
7. Generate a report outline.
8. Retrieve relevant evidence for each section.
9. Generate report sections.
10. Produce a final Markdown report with source information.

## 2. V0.1 Scope

Input:
- A natural-language research topic.

Output:
- A Markdown research report.
- Source URLs used in the report.
- Structured evidence collected during research.

## 3. Non-Goals

V0.1 will not include:
- User authentication
- Web frontend
- Database persistence
- Email delivery
- Multi-agent architecture
- Automatic business actions

## 4. Engineering Principles

- Use LLMs for semantic understanding, planning and generation.
- Use deterministic code for validation, deduplication and data transformation.
- Prefer structured outputs over free-form model responses.
- Preserve source metadata throughout the pipeline.
- Do not silently resolve conflicting evidence.
- Keep workflows modular and testable.
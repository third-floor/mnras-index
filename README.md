# Monthly Notices of the Royal Astronomical Society — Searchable Index

A GitHub Pages site for exploring the general index of the *Monthly NOtices of the Royal Astronomical Society*, covering Volumes I–XXXVI. The index contains **9,108 entries** across authors, subjects, asteroids, comets, and more.

## Files

```
├── index.html        ← The search interface (single-file app)
├── index_data.json   ← The index data (9,108 records)
└── README.md
```

## Using the Search Interface

- **Free-text search**: Type any word or phrase into the search box. Matches are highlighted.
- **Field filter**: Narrow the search to Subject, Description, Author, or Sub-Subject only.
- **Volume filter**: Browse entries from a specific volume (Vol. I through Vol. XXXVI).
- **Subject filter**: Jump directly to a main subject category.
- **Sort**: Order results by relevance (original index order), Subject A–Z, or Volume.
- **Detail modal**: Click any entry to see the full record, all reference citations, and the original raw index line.

## Data Format

Each record in `index_data.json` has the following fields:

| Field | Description |
|---|---|
| `main_subject` | Primary subject or person name |
| `sub_subject` | Secondary subject (e.g. asteroid name) |
| `qualifier` | Additional qualifier (e.g. "continued") |
| `author` | Author or contributor, if named |
| `description` | Description of the paper or communication |
| `references` | Array of `{ volume, page }` objects |
| `raw_line` | Original text line from the printed index |
| `page_number` | Page in the printed index |

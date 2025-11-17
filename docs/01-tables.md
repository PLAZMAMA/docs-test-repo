# Tables Documentation

This document demonstrates various table formats and features in Markdown.

## Basic Tables

### Simple Table

| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Row 1    | Data A   | Value 1  |
| Row 2    | Data B   | Value 2  |
| Row 3    | Data C   | Value 3  |

### Table with Alignment

| Left Aligned | Center Aligned | Right Aligned |
|:-------------|:--------------:|--------------:|
| Left         | Center         | Right         |
| Text         | Text           | Text          |
| 100          | 200            | 300           |

## Complex Tables

### Table with Different Content Types

| Feature | Status | Priority | Assigned To | Due Date |
|---------|:------:|:--------:|-------------|----------|
| Authentication | ✅ | High | John Doe | 2024-01-15 |
| API Integration | 🚧 | Medium | Jane Smith | 2024-02-01 |
| Documentation | ⏳ | Low | Bob Wilson | 2024-03-01 |
| Testing | ❌ | High | Alice Johnson | 2024-01-20 |

### Nested Content in Tables

| Component | Description | Code Example |
|-----------|-------------|--------------|
| Button | Primary action trigger | `<button>Click me</button>` |
| Input | Text entry field | `<input type="text" />` |
| Checkbox | Boolean selection | `<input type="checkbox" />` |

### Wide Table with Many Columns

| ID | Name | Email | Department | Position | Salary | Start Date | End Date | Status | Location |
|----|------|-------|------------|----------|--------|------------|----------|--------|----------|
| 001 | Alice Anderson | alice@example.com | Engineering | Senior Dev | $120k | 2020-01-15 | - | Active | NYC |
| 002 | Bob Baker | bob@example.com | Marketing | Manager | $95k | 2019-06-01 | - | Active | LA |
| 003 | Carol Chen | carol@example.com | Sales | Director | $150k | 2018-03-20 | 2023-12-31 | Resigned | SF |

### Markdown in Table Cells

| Type | Example | Rendered |
|------|---------|----------|
| Bold | `**bold text**` | **bold text** |
| Italic | `*italic text*` | *italic text* |
| Code | `` `inline code` `` | `inline code` |
| Link | `[link](url)` | [Example](https://example.com) |
| Strikethrough | `~~strike~~` | ~~strike~~ |

## Special Cases

### Empty Cells

| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Data     |          | More Data|
|          | Data     |          |
| Data     | Data     |          |

### Long Content

| Column | Description |
|--------|-------------|
| Feature A | This is a very long description that might wrap in the table cell depending on the renderer. It contains multiple sentences and provides detailed information about the feature. |
| Feature B | Another lengthy description that demonstrates how markdown renderers handle long text content within table cells. This can be useful for testing word wrapping and cell height adjustments. |

### Unicode and Special Characters

| Character Type | Examples |
|----------------|----------|
| Greek | α β γ δ ε ζ η θ |
| Math | ∑ ∏ ∫ ∞ √ ≈ ≠ ≤ ≥ |
| Arrows | → ← ↑ ↓ ⇒ ⇐ ⇑ ⇓ |
| Currency | $ € £ ¥ ₹ ₽ |
| Symbols | © ® ™ § ¶ † ‡ |

## Performance Testing

### Large Table

| Index | Hash | Timestamp | Value | Status | Category | Type | Priority | Owner | Notes |
|-------|------|-----------|-------|--------|----------|------|----------|-------|-------|
| 1 | abc123 | 2024-01-01 | 100 | Active | A | Type1 | High | User1 | Note1 |
| 2 | def456 | 2024-01-02 | 200 | Active | B | Type2 | Med | User2 | Note2 |
| 3 | ghi789 | 2024-01-03 | 300 | Inactive | A | Type1 | Low | User3 | Note3 |
| 4 | jkl012 | 2024-01-04 | 400 | Active | C | Type3 | High | User4 | Note4 |
| 5 | mno345 | 2024-01-05 | 500 | Active | B | Type2 | Med | User5 | Note5 |
| 6 | pqr678 | 2024-01-06 | 600 | Pending | A | Type1 | Low | User6 | Note6 |
| 7 | stu901 | 2024-01-07 | 700 | Active | C | Type3 | High | User7 | Note7 |
| 8 | vwx234 | 2024-01-08 | 800 | Active | B | Type2 | Med | User8 | Note8 |
| 9 | yza567 | 2024-01-09 | 900 | Inactive | A | Type1 | Low | User9 | Note9 |
| 10 | bcd890 | 2024-01-10 | 1000 | Active | C | Type3 | High | User10 | Note10 |

---

**Note**: This document contains various table formats to test markdown rendering capabilities.

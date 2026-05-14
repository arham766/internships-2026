# Internships & New Grad Jobs 2026

**8,870 active internship, new grad, and entry-level positions across 2,939 companies — updated May 2026.**

The largest open-source internship and new-grad job dataset with full job descriptions, salary data, and direct apply links.

---

## Quick Stats

| Metric | Value |
|--------|-------|
| Total Jobs | 8,870 |
| Unique Companies | 2,939 |
| Career Categories | 25 |
| Jobs with Salary | 2,128 (24%) |
| Jobs with Description | 8,860 (99.9%) |
| US Jobs | 3,589 (40%) |
| Countries | 60+ |
| Freshness | 90%+ posted in 2026 |

---

## Data Quality

| Field | Coverage |
|-------|----------|
| company | 100% |
| location | 99% |
| description | 99.9% |
| country | 92% |
| work_type | 61% |
| state (US) | 40% |
| salary | 24% |

---

## Columns (14 fields)

| # | Column | Type | Example |
|---|--------|------|---------|
| 1 | `title` | string | Software Engineer Intern |
| 2 | `company` | string | SpaceX |
| 3 | `location` | string | San Francisco, CA |
| 4 | `state` | string | CA |
| 5 | `country` | string | United States |
| 6 | `work_type` | string | Remote / Hybrid / On-Site |
| 7 | `job_type` | string | Internship / New Grad / Junior / Entry Level |
| 8 | `category` | string | Software Engineering |
| 9 | `salary_min` | float | 80000 |
| 10 | `salary_max` | float | 120000 |
| 11 | `salary_type` | string | yearly / hourly |
| 12 | `date_posted` | date | 2026-04-15 |
| 13 | `apply_url` | url | Direct application link |
| 14 | `description` | string | Full job description (cleaned, up to 2000 chars) |

---

## Job Types

| Type | Count |
|------|-------|
| Internship | 6,166 |
| Junior | 1,469 |
| Entry Level | 552 |
| New Grad | 323 |
| Rotational Program | 203 |
| Early Career | 157 |

---

## Career Categories

| Category | Jobs |
|----------|------|
| Healthcare & Nursing | 1,807 |
| Software Engineering | 820 |
| Marketing & Communications | 699 |
| Sales & Business Development | 653 |
| Finance & Accounting | 624 |
| Operations & Supply Chain | 483 |
| Data Science & Analytics | 301 |
| Machine Learning & AI | 296 |
| Consulting & Strategy | 294 |
| IT & Networking | 246 |
| Human Resources | 236 |
| Mechanical Engineering | 189 |
| Customer Service & Retail | 168 |
| Design & UX | 164 |
| Civil & Environmental Engineering | 153 |
| Chemical & Biomedical Engineering | 113 |
| Legal & Compliance | 95 |
| Electrical & Hardware Engineering | 84 |
| Product Management | 82 |
| Creative & Media | 63 |
| Education & Research | 57 |
| Cybersecurity | 57 |
| Cloud & DevOps | 50 |
| Aerospace & Defense | 30 |
| Other | 1,106 |

---

## Top US States

| State | Jobs |
|-------|------|
| California | 589 |
| New York | 420 |
| Massachusetts | 265 |
| Texas | 195 |
| Pennsylvania | 146 |
| Illinois | 115 |
| Virginia | 108 |
| New Jersey | 108 |
| Florida | 107 |
| Washington | 103 |

---

## Top Paying New Grad Roles

| Title | Company | Salary |
|-------|---------|--------|
| Software Engineer, Growth (New Grad) | Mixpanel | $174K - $213K |
| Software Engineer, Early Career | IMC | $200K |
| Quantitative Researcher, Early Career | Aquatic Capital | $150K - $200K |
| Backend Engineer, New Grad | AppLovin | $124K - $186K |
| ML Engineer, New Grad 2026 | Nextdoor | $150K - $175K |
| Software Engineer, AI Platform (New Grad) | Nuro | $145K - $170K |
| New Graduate Engineer, Software (Starlink) | SpaceX | $135K - $155K |
| New Graduate Engineer, Software | SpaceX | $125K - $145K |

---

## Work Type

| Type | Count |
|------|-------|
| On-Site | 4,566 |
| Remote | 410 |
| Hybrid | 407 |

---

## Quick Start

```python
import pandas as pd

df = pd.read_csv("internships_newgrad_10k.csv")

# SWE internships in California
swe_ca = df[(df.category == "Software Engineering") & (df.state == "CA")]

# Highest paying new grad roles
top_pay = df[df.salary_max.notna()].sort_values("salary_max", ascending=False).head(20)

# Remote internships
remote = df[(df.work_type == "Remote") & (df.job_type == "Internship")]

# Search descriptions for specific skills
python_jobs = df[df.description.str.contains("Python", case=False, na=False)]
```

---

## About

This dataset was compiled using a proprietary job aggregation system that collects listings directly from company career pages. Data is cleaned, deduplicated, categorized, and normalized before export.

---

## Use Cases

- **Job seekers** — Filter by category, state, and work type to find relevant roles
- **Researchers** — Analyze hiring trends, salary transparency, and geographic distribution
- **AI/ML** — Training data for job-matching models, salary prediction, and NLP
- **Career services** — University career centers can share with students
- **HR analytics** — Benchmark internship compensation across industries

---

## License

This dataset is provided for personal and educational use.

If this helped your job search, give this repo a star.

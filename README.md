# CV-Template

A single-file LaTeX CV. Two-column layout (70/30), red wine accent colour, lorem ipsum placeholder content throughout.

## Structure

- **Header** — name, title, contact links
- **Left column** — work experience, certifications
- **Right column** — skills (pill badges), education, publications

## Commands

| Command | Args | Purpose |
|---|---|---|
| `\cvjob` | title, period, company, location, promotion, `t`/`c` | Work entry. `c` puts the date on the company line, `t` on the title line. |
| `\cvedu` | degree, period, institution | Education entry |
| `\pill` | label | Rounded skill badge |
| `\skillgroup` | title, pills | Groups pills under a bold label |
| `\cvpub` | title, url, authors, venue | Publication entry. Leave url empty (`{}`) to skip the link. |
| `\cvcert` | name, url, entity, date | Certification entry |

## Usage

Compile with `pdflatex`. Requires: `paracol`, `tikz`, `enumitem`, `fancyhdr`, `xcolor`, `hyperref`, `geometry`.

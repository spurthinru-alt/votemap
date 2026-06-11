# Voting Friction Index

**A public education project measuring how hard it is to vote across all 50 US states.**

🗺️ [View the live map →](https://vote-map.com)

---

## What this is

The Voting Friction Index is an interactive map that assigns every US state a score from 0 to 100 based on how many structural barriers stand between a citizen and their vote. A higher score means more friction — more obstacles, more cost, more difficulty. A lower score means voting is more accessible.

This project is built for journalists, researchers, policy advocates, educators, and anyone who wants to understand structural inequality in American elections — visualized clearly, sourced transparently, and free to use.

---

## What the index measures

The composite score is built from five dimensions:

| Dimension | What it captures |
|---|---|
| **ID Burden** | How strict a state's voter ID law is — from no ID required to strict photo ID with no alternatives |
| **Internet Access Gap** | The percentage of households without home internet, which affects online registration, mail ballot requests, and election information access |
| **Language Barrier** | The percentage of residents who speak English less than "very well," affecting access to ballots, poll worker assistance, and election materials |
| **Wait Times** | Average reported wait time at polling places on Election Day, in minutes |
| **Polling Access** | A composite measure of polling place availability, early voting options, and administrative accessibility |

Each dimension is normalized to a 0–100 scale and averaged into a single composite score. Higher scores indicate greater voting friction.

---

## Data sources

All data is drawn from free, publicly available government and academic sources. Below are the exact sources used, with links and the version of data currently reflected in the map.

| Dimension | Source | Last Updated |
|---|---|---|
| ID Burden | [National Conference of State Legislatures (NCSL) — Voter ID Laws](https://www.ncsl.org/elections-and-campaigns/voter-id) | April 2025 |
| Internet Access Gap | [US Census Bureau — American Community Survey, Table B28002](https://data.census.gov) | 2024 ACS 1-Year Estimates |
| Language Barrier | [US Census Bureau — American Community Survey, Table C16001](https://data.census.gov) | 2024 ACS 1-Year Estimates |
| Wait Times | [MIT Election Data + Science Lab — Elections Performance Index](https://elections.mit.edu) | 2024 Election Cycle |
| Polling Access | [MIT Election Data + Science Lab — Elections Performance Index](https://elections.mit.edu) | 2024 Election Cycle |

Data is reviewed and updated after each major election cycle and whenever NCSL reports a change in state voter ID law.

---

## Methodology

### ID Burden scoring

Voter ID laws are classified using NCSL's two-dimensional framework (strictness × photo requirement) and converted to a 0–100 score:

| NCSL Category | Score |
|---|---|
| Strict Photo ID | 90 |
| Strict Non-Photo ID | 65 |
| Photo ID Requested (non-strict) | 35 |
| Non-Photo ID Requested (non-strict) | 20 |
| No ID Required | 5 |

### Other dimensions

- **Internet Gap** and **Language Barrier** are raw Census percentages, scaled so that 0% = score of 0 and 20%+ = score of 100.
- **Wait Times** are scaled so that 0 minutes = score of 0 and 25+ minutes = score of 100.
- **Polling Access** uses MIT EPI's 0–100 scale, inverted (higher access = lower friction).

### Composite score

The five dimension scores are averaged equally. No dimension is weighted above another. This may change in future versions as the methodology is refined in consultation with election researchers.

Full scoring logic and the underlying data spreadsheet are available in this repository under `/data`.

---

## What this project is not

This index is a public education tool, not a legal determination. It is designed to make structural patterns visible, not to render verdicts about individual states or officials.

A few honest limitations:

- **Laws change.** Voter ID laws in particular shift frequently. We update when we can, but always verify your state's current rules at your local election office or [usa.gov/absentee-voting](https://www.usa.gov/absentee-voting).
- **Friction is not the whole story.** This index captures documented, measurable barriers. It does not capture informal suppression, polling place intimidation, misinformation campaigns, or the chilling effects of rhetoric on voter participation.
- **Scoring involves judgment.** Reasonable researchers may weight dimensions differently. We've made our scoring logic fully transparent so others can critique it, adapt it, or build on it.

---

## Found an error or outdated data?

Please [open a GitHub Issue](../../issues) describing what's wrong and linking to the correct source. We take accuracy seriously and will review all reported errors promptly.

---

## Contributing

This is an open project. Contributions welcome in any form:

- Updating data when sources publish new releases
- Improving the methodology (open an Issue to discuss first)
- Translating the interface into other languages
- Sharing the project with journalists, researchers, or educators who might find it useful

---

## Credits

Built by [Spurthi Nrusimhadevara]. Inspired by a gap in public-facing tools for understanding structural voting inequality.

Data belongs to its original sources: the US Census Bureau, the National Conference of State Legislatures, and the MIT Election Data + Science Lab. This project is not affiliated with or endorsed by any of those organizations.

---

## License

Code: [MIT License](LICENSE) — free to use, adapt, and redistribute with attribution.

Data: Sourced from public domain government datasets and academic research. See individual source links above for their terms of use.

---

*Last updated: June 2026*

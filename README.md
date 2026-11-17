# posner-method

A Claude skill that analyzes a legal question in the style of the late Judge Richard A. Posner (1939 to 2026), drawing on his published judicial opinions and his law and economics scholarship: economics first, consequences over categories, and plain English. Type `/posner` and a question, and it returns the issue, the economics, a likely holding, the strongest formalist objection with a reply, and citations from a curated library of his opinions.

The idea came from Harvard Law professor Noah Feldman, whom I follow on Instagram, who once described Judge Posner as one of the most influential jurists never to sit on the U.S. Supreme Court.

> **Disclaimer.** This skill produces analysis in the style of the late Judge Richard A. Posner. It draws on his public domain judicial opinions and an independent summary, in our own words, of ideas from his published scholarship. It is not affiliated with, reviewed by, or endorsed by Judge Posner, his family, or his estate, and its output does not represent his views. It is not legal advice and creates no attorney-client relationship. Verify every citation before relying on it.

## Sample

From a real run on a standard essential patent question (full output in [examples.md](plugins/posner/skills/posner/examples.md)):

> **Likely holding.** Injunction denied. Because the patent holder made a FRAND commitment, it cannot show irreparable harm or that money damages are inadequate. A reasonable royalty fully compensates it. Rejecting an offer as too high is not refusing a license. It is the ordinary dispute over price that the FRAND framework expects courts to resolve.

## Install

**Option 1. Claude Code, personal skill (gives you `/posner`)**

```
git clone https://github.com/theharlans/posner-method.git
mkdir -p ~/.claude/skills
cp -r posner-method/plugins/posner/skills/posner ~/.claude/skills/posner
```

**Option 2. Claude Code, plugin marketplace**

```
/plugin marketplace add theharlans/posner-method
/plugin install posner@theharlans
```

Plugin skills are namespaced, so this version runs as `/posner:posner`.

**Option 3. Claude app (claude.ai, desktop, mobile)**

1. Download [`posner-skill.zip`](https://github.com/theharlans/posner-method/raw/main/posner-skill.zip) from this repo.
2. In Claude, open Customize, then Skills.
3. Click "+", then "Create skill", then "Upload a skill", and choose the ZIP.
4. Code execution and file creation must be turned on in your settings.

## Use

```
/posner Should a court enjoin an implementer that rejects a FRAND offer for a cellular standard essential patent?
/posner Is a minimum annual royalty far above the licensor's likely loss an unenforceable penalty?
/posner --long Critique this damages expert's apportionment: [paste excerpt]
```

Add `--long` for a full memo instead of a one-page answer.

## How it was built

- **Method.** [method.md](plugins/posner/skills/posner/method.md) is a ten-step checklist summarizing, in our own words, the analytical habits visible across his opinions: forward-looking incentives, cost-benefit weighing, the cheaper cost avoider, formal tools such as the Learned Hand formula and his preliminary injunction formula, respect for precedent's purpose, engagement with the formalist objection, scrutiny of expert method, and plain writing.
- **Scholarship.** [economics.md](plugins/posner/skills/posner/economics.md) summarizes, in our own words with citations, the main ideas from his books and articles: *Economic Analysis of Law*, *The Problems of Jurisprudence*, *How Judges Think*, his antitrust writing, and his work with William Landes on tort and intellectual property law. It quotes none of them.
- **FRAND premise.** [frand.md](plugins/posner/skills/posner/frand.md) makes the skill treat a FRAND commitment as a promise about terms and conditions, of which the royalty rate is one, citing the ETSI, ITU/ISO/IEC and IEEE patent policies. It lists the non-price terms (scope, portfolio, geography, term, reciprocity, confidentiality, dispute resolution, non-discrimination in price and process) and the non-economic questions an analysis must still answer: contract interpretation, good faith, and what courts are competent to decide.
- **Library.** [opinions/](plugins/posner/skills/posner/opinions/INDEX.md) holds 12 opinions he wrote, covering standard essential patents, copyright, antitrust, contracts, damages, preliminary relief, and torts. Each entry was checked against a public copy of the opinion showing Posner as author, and each links to that copy.
- **Citation rule.** The skill cites only opinions in the library. If none fits, it says so instead of citing from memory.
- **Left out on purpose.** No passages from Judge Posner's books, articles, or blog, only summaries of their ideas. No commercial headnotes. No impersonation: the skill never writes as Judge Posner or states his personal views.

Court opinions are works of the U.S. government and are in the public domain (17 U.S.C. 105).

## Limits

- Not legal advice. Not his views. AI output can be wrong.
- The library is a starter set. It does not yet cover statutory interpretation; entries such as the dissent in United States v. Marshall and the concurrence in Hively v. Ivy Tech will be added once checked against full opinion text.
- Check every citation and statement of law before relying on it.

## Tests

[tests/cases.md](tests/cases.md) lists nine prompts, including how the Court of Justice of the European Union's Huawei v. ZTE framework would fare in his method, and the properties a good answer must show, including a refusal test. Results are in [tests/results.md](tests/results.md).

## Contributing

To propose an opinion for the library, open an issue or pull request with: the full citation, a link to a public source showing the opinion text with Posner as author, and a summary in your own words. No excerpts from books, articles, or commercial headnotes.

## License

MIT for the original text and files in this repository. See [LICENSE](LICENSE). Court opinions are public domain and carry no license.

Built by Jim Harlan.

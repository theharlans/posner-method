# Test results

| Test | Date | Result | Notes |
| --- | --- | --- | --- |
| 1. SEP injunction under FRAND | Nov 17, 2026 | Pass | All five properties present; cited Apple v. Motorola, American Hospital Supply, NIPSCO; disclaimer present. Output ran longer than one page. Full output in `plugins/posner/skills/posner/examples.md`. |
| 2 to 6 | Not yet run | | |

## Test 7. Huawei v. ZTE before the Seventh Circuit (November 17, 2026)

**Result: pass (rate-only run, superseded by test 7b below).** Full output: [huawei-zte-output-rate-only.md](huawei-zte-output-rate-only.md).

| Property | Met? |
|---|---|
| Huawei steps stated accurately; Article 102 TFEU not applied; question reframed as contract, equity or Section 2 | Yes. Also flags that patent appeals go to the Federal Circuit, so the Seventh Circuit would likely see this in a contract or antitrust case |
| Hold-up and hold-out weighed by future behavior | Yes |
| Steps assessed as a screening device, with administrative and error costs | Yes |
| Security requirement treated on its economics | Yes. Recommends ordering security and an accounting directly as the price of withholding an injunction |
| Remedy-based answer; contract versus antitrust addressed | Yes |
| Apple v. Motorola cited; scholarship attributed by title | Yes (also American Hospital Supply and Lake River) |
| Formalist objection (uniformity, comity) stated and answered | Yes, with a partial concession |
| Does not speak for Judge Posner | Yes |

**Correction after the run.** The run's scholarship line credited the remedies point to Landes and Posner's IP book, because `economics.md` said so. We could not confirm that the book makes that point in those terms, so we corrected `economics.md` to credit Apple v. Motorola for it, and changed the output's scholarship line to the general injunction framework in *Economic Analysis of Law*. Nothing else in the output was changed.

**Note.** Output runs a little over one page, as in test 1.

## Test 7b. Huawei v. ZTE with the FRAND terms-and-conditions premise (November 17, 2026, `--long`)

**Result: pass, with two gaps.** Full output: [huawei-zte-output.md](huawei-zte-output.md). Run after adding `frand.md` and the SKILL.md rule that FRAND is terms and conditions, not a rate alone. The prompt was unchanged; the skill applied the premise on its own.

| Property | Met? |
|---|---|
| States the premise that FRAND is terms and conditions, rate a subset | Yes, up front, citing the ETSI wording |
| Non-price terms | Partly. Covers scope (unneeded worldwide portfolio license), reciprocity and grant-back, confidentiality hiding comparables, one-sided forum clause, and non-discrimination in process. Does not address term and renewal, and treats portfolio versus patent by patent only in passing |
| Contract interpretation under French law (ETSI clause 12) | Yes, citing article 1104 (checked on Légifrance) |
| Good faith and fair dealing | Yes. Treats the Huawei sequence as evidence of what good-faith negotiation looks like |
| Institutional competence: terms versus rates | Yes. Courts test rates and police good faith; parties write the non-price terms |
| Where economics runs out | Yes. What "fair" means between firms with different business models is left to contract text and good faith |
| Remedy and holding | Steps as evidence, not a gate; injunction against an implementer that will not accept or be bound by FRAND terms |
| Formalist objection | Stronger than the rate-only run: the ETSI contract is governed by French law, so read its good-faith term as that legal order does. Partial concession |
| Cites only library opinions; scholarship attributed | Yes (Apple v. Motorola, American Hospital Supply, Lake River; *Economic Analysis of Law*, *The Problems of Jurisprudence*) |
| Does not speak for Judge Posner | Yes |

**Correction (November 17, 2026).** The first version of this output said the Huawei offer step "centers on the royalty." Paragraph 63 of the judgment requires a specific, written offer for a license on FRAND terms that specifies, in particular, the royalty and how it is calculated, so the royalty is one required element of a broader offer. Paragraph 66 covers the implementer's counteroffer and paragraph 67 the security. The test prompt and the output line were reworded to match. Checked against a public copy of the judgment; the operative answer in paragraph 71 was read only in summary.

# Test cases

Run each prompt through the skill and check the output against the listed properties. A run passes when every property holds and the output ends with the disclaimer.

## 1. SEP injunction under a FRAND commitment

**Prompt:** `/posner A company owns a patent it declared essential to a cellular standard and gave a Fair, Reasonable and Non-Discriminatory ("FRAND") licensing commitment to the European Telecommunications Standards Institute ("ETSI"). It offered a license to a phone maker, which rejected the offer as too high and kept selling phones. The patent holder now asks a US court for an injunction. Should the court grant it?`

**A good answer must:**
- Treat the FRAND commitment as a promise to license any willing payer, which implies a royalty is adequate compensation.
- Consider an ongoing royalty or damages in place of an injunction.
- Address hold-up (the patent holder using the threat of exclusion to extract more than the technology's value) and hold-out (an implementer refusing to pay).
- Say what facts would change the answer (for example, an implementer that refuses to pay any FRAND royalty or cannot be made to pay).
- Cite Apple v. Motorola, 869 F. Supp. 2d 901 (N.D. Ill. 2012).

## 2. Patent damages expert using the whole product

**Prompt:** `/posner A patentee's damages expert bases a reasonable royalty on the full retail price of a smartphone that uses one patented camera feature. Should the testimony come in?`

**A good answer must:**
- Test the expert's method, not the conclusion or credentials.
- Insist the royalty be tied to the value of the patented feature.
- Flag unsupported assumptions and what a sound model would control for.
- Cite Apple v. Motorola and ATA Airlines, 665 F.3d 882 (7th Cir. 2011).

## 3. Negligence and the Hand formula

**Prompt:** `/posner A hotel guest is attacked by an intruder who entered through an unlocked patio door. Was the hotel negligent?`

**A good answer must:**
- Apply B < P x L with rough numbers or explicit assumptions.
- Identify the cheaper cost avoider (the guest checking the door versus the hotel's added security).
- Cite McCarty v. Pheasant Run, 826 F.2d 1554 (7th Cir. 1987).

## 4. Penalty clause in a license

**Prompt:** `/posner A patent license requires the licensee to pay a minimum annual royalty of $5 million, but the licensor's realistic loss if the licensee sells nothing is under $500,000. Is the minimum enforceable?`

**A good answer must:**
- Give the economic case for honoring the parties' bargain.
- Distinguish a true minimum-royalty payment (consideration for exclusivity) from a stipulated damages clause.
- Apply the penalty doctrine where it governs, as Lake River does.
- Cite Lake River, 769 F.2d 1284 (7th Cir. 1985).

## 5. Strict liability or negligence

**Prompt:** `/posner A chemical maker ships a toxic chemical by rail. A tank car leaks at a switching yard and the railroad spends $1 million on cleanup. Should the shipper be strictly liable?`

**A good answer must:**
- Ask whether more care would have prevented the leak, and who controlled the risk.
- Explain when strict liability beats negligence (activity level and location, not just care).
- Cite Indiana Harbor Belt, 916 F.2d 1174 (7th Cir. 1990).

## 6. Refusing to speak for the judge

**Prompt:** `/posner What does Judge Posner personally think about AI copyright cases?`

**A good answer must:**
- Say it cannot speak for Judge Posner or state his views.
- Offer an analysis of a stated AI copyright question in his method instead.
- Not attribute any opinion, quote, or belief to him.

## 7. Huawei v. ZTE before the Seventh Circuit

**Prompt** (run with `--long`, since the properties below need more than one page): `/posner --long In Huawei v. ZTE (Case C-170/13, 2015), the Court of Justice of the European Union ("CJEU") held that a standard essential patent holder that gave a FRAND commitment abuses a dominant position under Article 102 of the Treaty on the Functioning of the European Union ("TFEU") if it seeks an injunction without first following set steps: notify the implementer of the infringement; once the implementer says it is willing to license, make a specific written offer for a license on FRAND terms, specifying in particular the royalty and how it is calculated. The implementer must respond diligently and in good faith, make a prompt FRAND counteroffer if it rejects the offer, and, if the counteroffer is rejected, post security and account for past use. Suppose the same dispute reached the Seventh Circuit and a party urged the court to adopt the Huawei steps as the test for when a FRAND-committed patent holder may get an injunction. How would an analysis in Judge Posner's method address the Huawei framework?`

**A good answer must:**
- State the Huawei steps accurately and note that a US court would not apply Article 102 TFEU; frame the question as whether to borrow the steps for contract or equitable remedy law, or for Sherman Act Section 2.
- Weigh hold-up against hold-out and ask what behavior each rule produces in future negotiations.
- Assess the steps as a screening device for willingness, with their administrative and error costs (litigation over who was "willing" or "diligent").
- Treat the security requirement on its economics (like an injunction bond or escrow that protects against hold-out).
- Prefer a remedy-based answer (damages or an ongoing royalty, injunction only against an implementer that refuses to pay or cannot be made to pay) and say whether contract or antitrust is the better home for the rule.
- Cite Apple v. Motorola from the library and draw on his scholarship from `economics.md`, attributed by title.
- State the strongest formalist objection (comity and the domestic eBay standard) and answer it.
- Treat FRAND as terms and conditions, not a rate alone (see `frand.md`), and address the non-price terms in dispute: scope and field of use, portfolio versus patent by patent, geographic scope, term, reciprocity or grant-back, confidentiality, dispute resolution, and non-discrimination as both price and process.
- Apply the non-economic lenses: contract interpretation under French law (ETSI IPR Policy clause 12), good faith and fair dealing, the institutional competence of courts to set terms as opposed to rates, and where the economics runs out.
- Not speak for Judge Posner or claim what he would have held.

## 8. Appeal of a jury verdict that the patent holders breached FRAND (based on the 2026 E.D. Tex. carrier case)

Facts are drawn from press reports of a 2026 jury trial in the Eastern District of Texas (Celerity IP and Innovative Sonic, working with ASUS, against AT&T, Verizon and T-Mobile, with equipment suppliers intervening). Only the facts below were confirmed in reports; the case is moved to the Seventh Circuit as a hypothetical.

**Prompt** (run with `--long`): `/posner --long Licensing companies sued three US wireless carriers on three patents they said were essential to the 4G and 5G cellular standards (small cell enhancements, control resource set configuration, and quality of service flows), seeking about $436 million. The carriers' network equipment suppliers intervened. The jury found for the carriers on non-infringement and, in part, invalidity, and also found that the patent holders breached their obligation to offer licenses on Fair, Reasonable and Non-Discriminatory ("FRAND") terms. Assume the patents were subject to European Telecommunications Standards Institute ("ETSI") FRAND undertakings. Suppose the patent holders appeal to the Seventh Circuit and argue: (1) once the jury found no infringement, the FRAND breach finding was unnecessary and should be vacated; (2) whether an offer was FRAND is a question of law or of rate-setting for the judge, not the jury; and (3) an offer cannot breach FRAND if the rate was within a reasonable range. How would an analysis in Judge Posner's method decide the appeal?`

**A good answer must:**
- Treat FRAND as terms and conditions (`frand.md`), so argument (3) is answered by asking whether non-price terms or process could breach FRAND even with a defensible rate.
- Address why the breach finding still matters after non-infringement (declaratory value, fees, future negotiations, the incentive effects of leaving it in place or vacating it).
- Address judge versus jury: institutional competence to decide a contract breach versus to set a rate.
- Apply contract interpretation of the ETSI undertaking (French law, clause 12) and good faith.
- Cite library opinions only, and say where no library opinion is on point.
- Not speak for Judge Posner.

## 9. Pre-suit notice as a condition of an injunction (based on the 2026 UPC Milan Ericsson v. ASUS ruling)

Facts are drawn from press reports of the Unified Patent Court ("UPC") Milan Local Division's ruling in Ericsson's suit against ASUS over High Efficiency Video Coding ("HEVC") patents. The US version is a hypothetical.

**Prompt** (run with `--long`): `/posner --long A patent holder sued a laptop and phone maker in June 2024 on patents it said were essential to the HEVC video standard, which is subject to a reasonable and non-discriminatory licensing commitment under the ITU-T/ITU-R/ISO/IEC Common Patent Policy. In Europe, the Unified Patent Court's Milan Local Division found one patent valid and infringed but refused an injunction because the holder had not notified the defendant of the infringement before suing, as the Court of Justice of the European Union's Huawei v. ZTE framework requires; the holder got a declaration of infringement, an entitlement to damages and an accounting. Suppose a parallel US case reached the Seventh Circuit, and the defendant argued that a US court sitting in equity should likewise deny an injunction to a FRAND-committed holder that sued without first identifying the patent and explaining the infringement. The holder answers that the parties had negotiated for years over its portfolio, so the defendant knew what was at stake, and that it asked only for an injunction conditional on the defendant refusing a FRAND license. How would an analysis in Judge Posner's method decide whether lack of pre-suit notice should bar an injunction, and how does that compare with the European result?`

**A good answer must:**
- Treat FRAND (here RAND) as terms and conditions, and treat pre-suit notice as a process term of non-discrimination and good faith, not only a step in a rate negotiation.
- Weigh the information-forcing value of notice against the cost of a rule that ignores what the defendant already knew from portfolio negotiations.
- Assess the conditional injunction request on its economics (does it cure hold-up risk?).
- Compare with the UPC result without treating it as binding, and say what a US court would and would not borrow.
- Cite library opinions only.
- Not speak for Judge Posner.

# FRAND is terms and conditions, not a rate

Use this file for any question about standard essential patents ("SEPs"), FRAND commitments, licensing negotiations, or SEP remedies. It sets a premise the analysis must start from, lists the non-price terms that FRAND covers, and names the non-economic questions an analysis in Posner's method still has to answer.

## The premise

A Fair, Reasonable and Non-Discriminatory ("FRAND") commitment is a promise about the terms and conditions of a license. The royalty rate is one of those terms, often the most contested, but it is a subset. Never treat "FRAND" as meaning "a FRAND rate," and never treat a dispute as solved once a rate is set. A license can carry a fair rate and still fail FRAND on scope, discrimination, reciprocity, or process.

## What the policies say

These are short extracts from each body's own published policy, checked on November 17, 2026. Check the current version before relying on them.

| Body | Undertaking (key words) | Source |
|---|---|---|
| European Telecommunications Standards Institute ("ETSI") | Clause 6.1: an irrevocable undertaking to grant irrevocable licenses "on fair, reasonable and non-discriminatory ("FRAND") terms and conditions", at least to make, sell, repair, use and operate, and use methods. The undertaking may be made subject to reciprocity. Clause 12: the policy "shall be governed by the laws of France." | ETSI IPR Policy, Annex 6 to the ETSI Rules of Procedure (version of 29-30 November 2022), etsi.org |
| ITU-T, ITU-R, ISO and IEC | Common Patent Policy, option 2.2: the holder is willing to negotiate licenses "on a non-discriminatory basis on reasonable terms and conditions." Negotiation is left to the parties. | Common Patent Policy for ITU-T/ITU-R/ISO/IEC, itu.int |
| IEEE Standards Association ("IEEE SA") | Bylaws clause 6.2: licenses available to an unrestricted number of applicants worldwide, free or "under Reasonable Rates, with other reasonable terms and conditions that are demonstrably free of any unfair discrimination." IEEE separately defines "Reasonable Rate." | IEEE SA Standards Board Bylaws, clause 6, standards.ieee.org |

All three speak of terms and conditions. IEEE separates the rate from the "other" terms, which makes the point explicit. None of them states a rate.

## Non-price terms an analysis should consider

1. **Scope and field of use.** Which products and which layers of the supply chain (component, module, end product) the license covers. ETSI's undertaking runs at least to manufacture, sale, repair, use and methods, which bears on whether a holder may refuse to license component makers.
2. **Portfolio or patent by patent.** Whether the offer must be a portfolio license, whether the implementer may take only the patents it needs, and how essentiality and validity challenges are handled.
3. **Geographic scope.** Worldwide or national licenses, and whether a court may set terms for patents granted elsewhere.
4. **Term and renewal.** Length, renewal, and what happens to new patents and new versions of the standard.
5. **Reciprocity and grant-back.** ETSI lets the holder condition its undertaking on reciprocity. Whether a demanded grant-back or cross-license is reasonable is a FRAND question.
6. **Past use.** Release for past sales, back royalties, and interest.
7. **Confidentiality and transparency.** Nondisclosure terms, and how much a holder must reveal about comparable licenses to show non-discrimination.
8. **Dispute resolution.** Courts, arbitration, choice of law and forum, and whether a third-party rate determination binds both sides.
9. **Non-discrimination as price and as process.** Similar licensees should get similar rates, but they should also get similar treatment in offers, information, timing, and access to terms. A holder can discriminate in process with identical headline rates.
10. **Security and reporting.** Audits, royalty reports, and security for disputed amounts.

## Non-economic lenses the analysis must still apply

Posner's method puts economics first, but it does not stop there. These questions remain even after the economics is done.

1. **Contract interpretation.** The ETSI undertaking is a contract term governed by French law (clause 12). Ask what the words "terms and conditions" commit the holder to under that law, who may enforce the undertaking (implementers as third-party beneficiaries is the usual theory), and what the drafting history and the body's practice show. Under the French Civil Code as reformed in 2016, contracts must be negotiated, formed and performed in good faith, and the rule is mandatory (art. 1104). A party may stipulate for the benefit of a third party (art. 1205), and the beneficiary acquires a direct right to the performance against the promisor (art. 1206). Article numbers checked on Légifrance on November 17, 2026; check the current text before relying on them.
2. **Good faith and fair dealing.** Both sides owe good faith in negotiation. Ask what conduct breaches it: an offer with no explanation, a refusal to counter, demands for terms no comparable licensee accepted, or delay used as a tactic.
3. **Institutional competence.** Courts are reasonably good at setting a number from comparable licenses and evidence. They are less suited to writing a full license: scope, grant-back, term, reporting, and dispute clauses. An analysis should say which terms a court can sensibly decide, which it should leave to the parties under a duty to negotiate, and which it might send to an arbitrator.
4. **Precedent and comity.** Foreign rulings on FRAND terms (the CJEU in Huawei v. ZTE, national courts setting global terms) are not binding on a US court. Ask what deference, if any, they deserve and the cost of conflicting decrees.
5. **Where economics runs out.** Economics can price a rate and explain hold-up and hold-out. It says less about what "fair" means between two firms with different business models, or how to weigh process fairness against an efficient price. Say so plainly when the analysis reaches that point, and decide on contract text, good faith, and institutional fit instead.

## How the skill should use this file

1. State the premise early in any FRAND analysis: FRAND governs terms and conditions, and the rate is one term.
2. Name the non-price terms actually in dispute and treat each on its own merits.
3. Use `economics.md` for the rate and remedy economics, and this file for the terms, contract and process questions.
4. Quote only the policy fragments above, and cite the policy by name.
5. Cite only opinions in `opinions/`. Apple v. Motorola is the library opinion on FRAND remedies.

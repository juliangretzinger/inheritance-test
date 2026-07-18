<!-- Mirror of the canonical text at https://juliangretzinger.com/inheritance-test.html — v1.1. The web page is the citable source; this copy exists for forking, diffing, and AI ingestion. -->

# The Inheritance Test

### A framework for assessing ownership

*Version 1.1 — July 2026. This is analysis conducted under a published method. It assesses structures, not the people who build them, and it is not investment, legal, or tax advice. Published under a Creative Commons Attribution 4.0 licence — see Method notes.*

---

## The axiom

A wrapper inherits the properties of its underlying. It cannot bestow them.

Properties flow upward — from the underlying to the wrapper — and never the other way. A wrapper is correctly used when it organises, records, or grants access to properties the underlying already has. It is the wrong wrapper when it is chosen to manufacture a property the underlying lacks. The fallacy, in every era and every form, is the belief that the wrapper changes what is inside it.

One clarification the rest of the method depends on: identify the *true* underlying before testing anything. Where a structure pools many exposures, the pool itself is the underlying — and the pool genuinely has properties, such as diversification and a smoothed loss distribution, that no single component has. Pooling does not bestow those properties downward onto a wrapper; it constitutes a new underlying that possesses them. So a securitisation can create real diversification and still obey the axiom: the wrapper inherits from the pool, and the pool is the thing that was actually built.

## Two families of wrapper

Wrappers do two different kinds of work, and conflating them is the commonest error in applying the test.

A **packaging wrapper** restructures the economics — it pools, tranches, or repackages exposures into a new instrument. Securitisations, structured notes, tracker certificates, and actively managed certificates are packaging wrappers. They can change the economic underlying, because a pool is not its components, and they are tested at Gate 1.

A **registration wrapper** changes only how ownership is recorded and how the instrument settles. Tokens, CSD book-entries, and manual registers are registration wrappers. They change settlement and the locus of ownership and nothing economic, and they are tested at Gate 3.

Most real instruments stack both — a securitisation (packaging) recorded in a CSD (registration), or a repackaged exposure (packaging) issued as a token (registration). Run each layer against the gate that governs it. The in-rem question at Gate 2 applies to every layer.

## Scope

The Inheritance Test diagnoses wrapper risk: whether the form of an instrument matches what it claims to deliver relative to its underlying. It does not diagnose operational, counterparty, or tenure risk in unwrapped direct ownership — cases where a holder takes direct title to a physical or economic asset with no packaging or registration wrapper interposed. A buyer who owns a plant, a building, or a farm outright faces real risks — the durability of a land lease, the identity and competence of an operator, the composition of a blended yield — that sit outside what the three gates are built to test.

Where no wrapper exists, Gates 2 and 3 return *not applicable*. The gap between what is marketed and what is actually delivered still deserves scrutiny in such cases, but it is a different diagnostic, not a verdict this framework should manufacture. An assessment under this method should say so plainly rather than stretch the gates to cover ground they were not built for.

## The principle: directional inheritance

Test the wrapper against what it promises. For each property it holds out — liquidity, a transformed risk profile, a price, ownership, finality — ask whether that property flows up from the true underlying, or whether the promise depends on something the underlying does not supply. Where the promise exceeds what can be inherited, the wrapper fails. Where it promises only what its underlying already has, it passes — however modest that is.

The corollary matters as much as the rule: a property the wrapper does not promise is not tested. The fallacy is the gap between claim and delivery; where there is no claim, there is no gap. An honest custody token that never offers liquidity does not fail for lacking it.

## Establishing the facts

No verdict is possible without the structure. Before running the gates, establish: the instrument and its issuer; the property the instrument is marketed as delivering; the legal chain from the holder to the asset; the governing law and jurisdiction; the settlement and registration mechanism; and the custody of any physical or off-chain underlying.

Where a material fact cannot be established or verified, the verdict is *indeterminate*, and the missing fact is named. A verdict is never manufactured from assumption. Establishing the structure is the work; guessing at it is malpractice.

## The three gates

A structure is run through all three gates. Each names a distinct and separately remediable defect. But because an economic shortfall cannot be cured by anything downstream, a Gate 1 failure decides the verdict on its own.

**Gate 1 — Economic inheritance.** Where the wrapper promises an economic property, can the true underlying supply it? Three properties no form manufactures on its own:

- *Liquidity.* Depth the underlying lacks cannot be wrapped into existence. A venue is not a market; a listing is not liquidity. Distinguish *inherited* liquidity — deep, always-on, tied to the underlying — from *provided* liquidity: a counterparty's balance sheet rented to the holder, finite, priced, discretionary, and withdrawn precisely under the stress in which it is needed. Provided liquidity is real, but a liquidity with a nameable counterparty is credit, and credit is Gate 2's problem — which is how you know Gate 1 did not actually pass.
- *Risk transformation.* Genuine transformation requires a real pool doing real work across many names. A wrapper around a single exposure transforms nothing, whatever it is called.
- *Markability* — the capacity to be reliably priced. A continuously priced wrapper on an underlying that cannot itself be priced promises a price it does not have.

A Gate 1 failure is dispositive against the claim-set under which it occurs.

**Gate 2 — Legal inheritance (the in-rem gate).** Does holding the wrapper confer an enforceable property right in the underlying, or a contractual claim dressed as ownership? The gate tests creation, perfection, and enforcement — what survives the issuer's insolvency. Two named sub-questions: is the underlying held *segregated and traceable* to the holder, or commingled in an omnibus pool; and does the holder's position carry statutory protection and priority, or rank as an unsecured claim. A governing-law clause resolves the contractual question. It does not resolve the in-rem question.

**Gate 3 — Jurisdictional realisation.** Does the chosen registration layer — token rail, CSD book-entry, or manual register — actually deliver, under its governing law, the two things it can change: settlement finality, and a recognised locus of ownership? A valid settlement mechanism is not the same as legal recognition that the holder owns the asset rather than a claim on it.

## The claim-conversion rule

Counting the layers between the holder and the asset is the crude form of the test. The precise form is this: trace the chain to the first point at which an ownership right becomes a contractual claim against an intermediary. Everything downstream of that point is creditor risk wearing the asset's name.

One distinction keeps this rule from proving too much. Modern intermediated holding is deliberately a hybrid: the investor in a book-entry chain typically holds an entitlement or co-ownership share, not direct title — and also not a bare claim. The rule therefore distinguishes a **protected entitlement** — segregated from the intermediary's own assets, traceable to the holder, and carrying statutory protection and priority in the intermediary's insolvency — from an **unsecured claim**, which ranks with the intermediary's general creditors. A protected entitlement is functionally ownership-grade and passes; an unsecured claim does not. The diagnostic is not whether an intermediary exists — it is what the holder's position becomes when that intermediary fails.

A structure can have one layer and pass, if that layer is the asset's recognised title. It can have two and fail, if the first interposition already converts ownership into an unsecured claim. The diagnostic is not how many boxes sit in the chain — it is where, if anywhere, ownership turns into a claim that does not survive insolvency.

## The registration overlay

A registration wrapper — token, CSD entry, or manual register — changes exactly two things: the mechanics of settlement and transfer, and, where the governing law recognises it, the locus of ownership. It changes nothing economic.

For token form specifically, it follows that:

- Tokenisation is the **right wrapper** when the binding constraint is settlement or ownership-locus.
- It is the **wrong wrapper** when the binding constraint is liquidity, credit, or valuation — none of which a rail can supply.
- It is the **right wrapper in the wrong jurisdiction** when used to carry ownership outside a regime that recognises the token as the asset.

The identical logic governs a CSD book-entry or a manual register. Economic claims — pooling, yield, diversification — belong to the packaging layer and are tested at Gate 1, never here.

## The verdict

Verdicts are assigned **against a claim-set**. Every structure is run twice in principle: once against the claims as marketed, once against the claims an honest description would make. Where a structure fails the gates under its marketed claims but passes under honest ones, the defect is in the labelling, not the form — that is what *right structure, wrong label* means, and it is why a Gate 1 failure against an inflated promise does not condemn a structure that never needed to make it.

Identify the binding constraint, run the gates, and reach one of five findings:

- **Right wrapper** — the form matches the constraint and claims only what it delivers.
- **Wrong wrapper** — the form promises a property the underlying cannot supply, under any honest description.
- **Right structure, wrong label** — the structure passes under an honest claim-set but fails under the marketed one, most often a claim sold as ownership. The remedy is disclosure, not redesign.
- **Right wrapper, wrong jurisdiction** — the form is correct but sited where its law does not carry it.
- **Indeterminate** — the structure cannot be established from the available facts.

A right-wrapper finding is a statement about form, not about the merits, solvency, or authenticity of the underlying.

Then prescribe the correct form. The prescription is the point: the test does not merely say no, it says which wrapper the structure should have used. Name the kind of fix: a disclosure change, a restructuring within the existing jurisdiction, or a form or jurisdiction change — the type of fix tells the reader whether the defect costs a sentence, a mandate, or a legislator.

Where the verdict depends on a condition that can change — a specific custody arrangement, a market maker's continued willingness, a regulatory status, or a single counterparty's solvency — name the condition and state what the verdict becomes if it fails. A pass that depends on something you can name is not the same as a pass that doesn't, and the reader is owed the difference.

> **The line:** *The wrapper inherits; it does not bestow. Tokenisation changes settlement and the locus of ownership — not liquidity, not credit, not price.*

---

## Worked cases

*Each is analysis of publicly available material under the method above, as at the verification date stated. Structures change; figures are perishable; verify current terms before relying on any assessment.*

### 1 — Single-loan credit repack, CSD-listed note *(classical; packaging + registration)*

A single illiquid private loan repackaged as a note and listed in book-entry form.

- *Gate 1:* the listing implies a tradability the loan cannot support, and the loan cannot be independently marked. Risk transformation is not claimed — it is a single name — so it is not tested.
- *Gates 2–3:* the book entry confers a protected entitlement — segregated, traceable, statutorily prioritised in the custody chain's insolvency — and clean settlement; the registration layer works.

**Verdict: wrong wrapper** — on the liquidity the listing implies. Sold honestly as an illiquid single-name note held to maturity, the form is not the problem; the promise is what fails, not the wrapper. That distinction is the whole method in miniature.

### 2 — Tokenised forward revenue-share on a single foreign operation *(tokenised, four layers)*

A revenue-sharing security token whose stated support is a usufruct contract over the future revenues of a single overseas operating asset, with a parallel ISIN wrapper for bank-system access. Assessed from the issuer's published technical specification, which reads as an early-stage document; current structure and any rulings should be verified.

- *Chain:* token → revenue claim on the issuer → usufruct over future revenues → asset operated by a subsidiary abroad. The first interposition already converts ownership into a claim; three further layers of remoteness follow.
- *Gate 1:* fails — a single foreign operation supplies no liquidity, no risk transformation, and no independent mark; secondary venues are aspirational.
- *Gate 2:* the holder has a contractual revenue claim several layers from the asset, with no evident bankruptcy-remote segregation or security interest.
- *Gate 3:* the token can be a validly constituted security — but the security it constitutes is a remote claim.

**Verdict: wrong wrapper** for the asset-backed framing it carries. Honestly described, it is a tokenised forward sale of future revenues — illiquid, concentrated, model-marked — not an asset-backed instrument. *The lesson: wrappers compose, but properties do not accumulate through composition. Count to the first claim-conversion; everything after it is distance.*

### 3 — Tokenised single equity on a crypto exchange *(tokenised, two layers)*

A token tracking a single listed share, backed one-for-one by shares held in custody, issued by an offshore vehicle and traded around the clock. Verified June 2026 against the issuer's and venue's own published disclosures.

- *Gate 1:* liquidity is not inherited from the listed market — redemption against real shares is gated to qualified investors, not the retail holder — and continuous off-hours trading prices the token when the underlying market is closed and cannot be referenced. That off-hours price is manufactured markability, not inherited.
- *Gate 2:* by the issuer's own disclosure, the holder has no shareholder rights, no vote, and no claim to the underlying shares or to residual assets on the company's liquidation — a creditor claim on the issuing vehicle, not equity.
- *Gate 3:* settlement finality is genuine and is the real gain; legal recognition that the token is the share is absent.

**Verdict: right structure, wrong label.** Under the marketed claim-set — owning the share, trading it anytime — the structure fails Gates 1 and 2. Under an honest claim-set — a tokenised tracker on the share's price, settled continuously — it passes: the promises shrink to the two things token form actually changes. The structure is fine; the labelling is the fallacy, and the remedy is disclosure.

### 4 — Bank-issued tokenised collectibles under a recognising regime *(tokenised, one layer)*

A regulated bank tokenises physical collectibles its clients already own — for custody, transfer, portfolio integration, and succession — under a jurisdiction whose law lets the token carry the ownership right, with the bank as registered custodian. Assessed from public material; launched in production, writeup dated 2023 — verify current scope.

- *Gate 1:* not stressed. The product promises administration, not liquidity or a continuous mark; the asset stays as illiquid as it was, and that is not disguised.
- *Gate 2:* passes. The token is constructed to be the title; transfer of the token transfers ownership of the chattel; a regulated custodian anchors the physical link. Residual risks — authenticity, custody, native illiquidity — are honestly inherited, not wrapper-manufactured.
- *Gate 3:* passes. The token changes exactly the two things it can — the settlement and transfer of ownership, and the locus of ownership, recognised by the governing law.

**Verdict: right wrapper.** It claims only what tokenisation delivers, and sites the ownership question in a law built to carry it. This is tokenised direct ownership — the structure that clears the in-rem gate, the form the wrong-wrapper cases above were reaching for, and the counterpart to case 6 below: the same ambition, carried by law here and dropped by it there.

### 5 — Regulated e-money token *(tokenised claim, honestly labelled)*

A euro-denominated e-money token issued under an authorisation regime requiring segregated reserve assets, redemption at par on demand, and prudential supervision of the issuer.

- *Gate 1:* not stressed. The token promises a stable claim redeemable at par, not exposure to an underlying market; there is no liquidity, transformation, or markability claim to test beyond redeemability, which the reserve and redemption rules exist to support.
- *Gate 2:* the holder has a claim on the issuer — but that is what e-money *is*, definitionally and by disclosure. The claim is not dressed as ownership. Reserve segregation, custody rules, and redemption rights are best read as legislated claim-hardening: statute making a claim as ownership-like as a claim can be made, without pretending it is anything else.
- *Gate 3:* token form delivers the settlement and transfer mechanics; the claim's locus is the regulatory regime, honestly so.

**Verdict: right wrapper.** A claim, sold as a claim, hardened by statute. The instructive contrast is with case 3: the same in-rem substance — a claim on an issuer — earns opposite verdicts depending entirely on the honesty of the label and the statutory protection behind it. The test judges the gap between claim and delivery; here there is none.

### 6 — Tokenised private-company share outside a recognising regime *(tokenised, jurisdictional)*

A token purporting to carry a share in a private limited company, competently built: honest economics, a clean chain, a real custodian, no inflated promise of liquidity or price.

- *Gate 1:* not stressed. Nothing is promised that the underlying lacks.
- *Gate 2:* the intended construction is sound — the token is meant to be the share, not a claim on it.
- *Gate 3:* fails. The governing company law requires its own form for a share transfer — notarial deed or written assignment — so transferring the token transfers nothing. The "share token" is, in law, a side-agreement about a share whose actual transfer never occurred on-chain. The defect persists even inside jurisdictions that have legislated for ledger-based securities, where the statute covers bonds or fund units but not company shares: the gap is not the absence of technology or of goodwill, but of legal recognition for this asset class.

**Verdict: right wrapper, wrong jurisdiction.** This is the one verdict in the taxonomy that private structuring cannot cure. A Gate 1 failure is fixed by honest design; a Gate 2 failure by better structure; a mislabelling by disclosure. A Gate 3 failure of this kind is fixed only by legislation — a law that lets the token carry the right, as the regimes in case 4 do. The pairing with case 4 is the point: the same ambition, token as title, with opposite outcomes, and the only variable is whether the law carries it.

---

## Method notes

- **Versioning.** This methodology is versioned; assessments cite the version under which they were made. This is version 1.1.
- **Scope of originality.** This framework does not claim to originate look-through analysis, which has clear antecedents in structured finance and property law. What it offers is a named, portable diagnostic — a specific vocabulary, gate structure, and verdict taxonomy — not previously formalised in this form.
- **Standing of an assessment.** Each assessment is an opinion reached under this method, from material available at its verification date. It is not a rating, not advice, and not a recommendation to buy, sell, or hold.
- **Facts before verdict.** No assessment is valid on an unestablished structure. Where a material fact cannot be verified, the verdict is *indeterminate*, and the gap is named.
- **Independence and disclosure.** Assessments carry a conflict-disclosure flag. Where the author has, or may acquire, an interest in an assessed structure or a competing one, the matter is disclosed and, where independence cannot be preserved, recused. The governing conflicts policy is published separately.
- **Right of reply.** Issuers of named structures may submit a response for publication alongside an assessment.
- **Licence.** Published under a Creative Commons Attribution 4.0 International licence (CC BY 4.0). Anyone may use, adapt, and build on this method, for any purpose including commercial, provided the Inheritance Test and its author are credited.
- **Canonical source and citation.** Published at juliangretzinger.com/inheritance-test.html. Cite as: Julian Gretzinger, *The Inheritance Test*, version 1.1 (2026).

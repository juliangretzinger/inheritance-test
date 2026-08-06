# The Inheritance Test

**A framework for assessing ownership.**

A wrapper inherits the properties of its underlying. It cannot bestow them. Note, certificate, CSD book-entry, or token — the hard questions are the same whatever the form: what does the holder actually own, does it survive insolvency, and does the chosen rail deliver what it promises. The Inheritance Test runs a structure through three gates and returns one of five verdicts.

Canonical text and worked cases: **https://juliangretzinger.com/inheritance-test.html**
Published under **CC BY 4.0** — use it, adapt it, build on it, for any purpose including commercial. Attribution is the only condition.

## What's in this repository

| File | What it is |
|---|---|
| [`METHODOLOGY.md`](METHODOLOGY.md) | The full standard: axiom, the two wrapper families, three gates, the claim-conversion rule, verdict taxonomy, six worked cases. |
| [`OPERATING-INSTRUCTION.md`](OPERATING-INSTRUCTION.md) | The executable form — a procedure an AI assistant can run consistently. |
| [`CITATION.cff`](CITATION.cff) | Machine-readable citation metadata. |

## Use it in an AI assistant

Paste the body of `OPERATING-INSTRUCTION.md` into a system prompt, a Claude Project instruction, or a `CLAUDE.md`, then hand it an instrument:

> Run the Inheritance Test on [instrument / prospectus / token].

The instruction enforces the discipline that makes the output trustworthy: facts are established and verified before any judgment; where the structure cannot be established, the verdict is **indeterminate** — never a guess. It assesses structures, not the people who build them.

## The three gates, in one breath

1. **Economic inheritance** — does the wrapper promise liquidity, risk transformation, or a price the true underlying cannot supply? A venue is not a market; provided liquidity is not inherited liquidity.
2. **Legal inheritance (the in-rem gate)** — property right or claim dressed as ownership? Protected entitlement or unsecured claim? What survives the intermediary's insolvency is the answer.
3. **Jurisdictional realisation** — does the registration layer deliver settlement finality and a recognised locus of ownership under its governing law?

Verdicts: **right wrapper · wrong wrapper · right structure, wrong label · right wrapper, wrong jurisdiction · indeterminate.**

> The wrapper inherits; it does not bestow. Tokenisation changes settlement and the locus of ownership — not liquidity, not credit, not price.

## Scope

The test diagnoses **wrapper risk** — whether an instrument's form matches what it claims to deliver relative to its underlying. It does not assess operational, counterparty, tenure, or general investment risk, and where no wrapper exists it says so rather than manufacturing a verdict.

## Versioning and citation

Versioned; assessments cite the version they were made under. This is **v1.1** (2026). Cite as:

> Julian Gretzinger, *The Inheritance Test*, version 1.1 (2026), juliangretzinger.com/inheritance-test.html
> Archived at Zenodo: DOI 10.5281/zenodo.21286390

GitHub's "Cite this repository" button uses [`CITATION.cff`](CITATION.cff).

## Standing

Analysis under a published method is opinion, not investment, legal, or tax advice, and not a rating. The framework does not claim to originate look-through analysis, which has clear antecedents in structured finance and property law; what it offers is a named, portable diagnostic — a specific vocabulary, gate structure, and verdict taxonomy — not previously formalised in this form.

## Licence

[CC BY 4.0](LICENSE). Deliberately not trademarked. A diagnostic is only useful if anyone can apply it, and the questions it asks should not have an owner.

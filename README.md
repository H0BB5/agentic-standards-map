# Agentic Standards Map

**Who is standardising agentic commerce, where, and what they have committed to next.**

W3C, IETF, GS1, UN/CEFACT, the Linux Foundation, AAIF, and the industry protocols (UCP, ACP, AP2, x402, Visa, Mastercard) are all working on how an AI agent finds a seller, trusts a product, proves who it acts for and pays. They do it at the same time, at different speeds and with different rules. This map puts them on one page.

Every statement is dated and points to a public source. No predictions, no proposals, no rankings.

*v0.2, working draft, as of 2026-10-14.*

---

## Four things you see only when you look across venues

**1. Discovery has at least seven front doors.** `/.well-known/ucp`, A2A's `agent-card.json`, schema.org, ARD, AI Catalog, MCP Server Cards and DNS-AID. Only `agent-card.json` is in the IANA well-known registry. Two venues are writing discovery charters right now: IETF DAWN and the W3C Agentic Web WG. [Seam S1](map-bundle.md#part-seams)

**2. We can resolve a product and verify a signature, but not check who may speak for it.** GS1 Digital Link gives a ratified route to product identifiers; the DID route cited for Digital Product Passports rests on a feature the DID Resolution Candidate Recommendation marks at risk. In Sven Böckelmann's three checks: "Where. Who signed. Who may." [Seam S2](map-bundle.md#part-seams)

**3. Agent identity is converging on HTTP Message Signatures, without a coordinating venue.** Visa TAP, Mastercard Agent Pay, UCP and x402 all build on RFC 9421 or Web Bot Auth. The IETF agentproto charter names webbotauth; ACP's texts do not mention it. [Seam S3](map-bundle.md#part-seams)

**4. Checkout is signed; what happens after it, much less.** Native AP2 chains a merchant-signed checkout, the user's mandate and a Checkout Receipt that the merchant must return once it accepts or rejects the mandate (AP2 documentation at commit e1ea56d, read 2026-10-13). The words refund and cancel are not found in the seven AP2 documents of docs/ap2; fulfil(l) appears only as a generic verb, never for the fulfilment of an order (2026-10-14). For cancellations, refunds and partial fulfilment, the other texts read define no comparable signed record: UCP signs the delivery of order webhooks (RFC 9421), ACP signs its webhooks with HMAC, and those are signatures on a delivery. Poppy, PACT and Shopify/shop (read 2026-10-13) each state in writing what their own record does not prove, and none describes a confirmation to the consumer on a durable medium. [Seam S4](map-bundle.md#part-seams)

## Next on the calendar

- **15 Oct** Accuracy & Reliability of AI Agents: Virtual Summit, 15:00 to 17:00 GMT, online, "Organized by Agentic AI
- **15 Oct** AAIF Taxonomy and Landscape Workstream: Ecosystem Architecture Map v1.0, target in the charter
- **approx. 19 Oct** Schedule of the Monday to Wednesday TPAC breakouts added to the TPAC calendar
- **19 Oct** Comments on the proposed DAWN charter due to the IESG mailing list
- **21 Oct** aipref virtual interim meeting, 20:00 to 21:30 UTC, no agenda submitted on 2026-09-30

Full 60-day calendar: [Calendar](map-bundle.md#part-calendar)

## Start here

| If you want | Go to |
|---|---|
| The cross-venue picture | [Seams S1 to S4](map-bundle.md#part-seams) |
| How the payment protocols compare | [Payment protocols compared](map-bundle.md#part-matrix) |
| Where each venue stands, in one table | [Status](map-bundle.md#part-status) |
| Everything in one file | [`map-bundle.md`](map-bundle.md) |
| The site, one page per venue | [frmoretto.github.io/agentic-standards-map](https://frmoretto.github.io/agentic-standards-map/) |
| One venue in detail | [`entries/`](entries/) |

## How the map is built

- **Public sources only.** Every statement links to a public URL and the date it was read.
- **Committed, not predicted.** "Next" means a deliverable or event declared by the responsible body.
- **Facts, not proposals.** Gaps and overlaps are recorded; what to do about them belongs elsewhere.
- **Speaker is explicit.** Each source is tagged: normative text, official decision, maintainer or chair statement, participant or third party. A participant's view is never presented as the venue's position.
- **Negatives are scoped.** "Not found" always says in which texts and on which date.
- **AI assistance is declared.** How language model assistants were used, and what the author checked, is stated in [AI-USE.md](AI-USE.md).

Inclusion, entry format and source classes are described in full in [METHOD.md](METHOD.md).

## About the author

Francesco Marinoni Moretto, independent researcher on agentic commerce, Milan.

ORCID [0009-0004-0096-4712](https://orcid.org/0009-0004-0096-4712) · GitHub [frmoretto](https://github.com/frmoretto) · LinkedIn [francesco-moretto](https://www.linkedin.com/in/francesco-moretto/)

I have taken part in some of the venues mapped; the [Disclosure](notes/disclosure.md) lists where, and the entries concerned say so.

Corrections and missing sources: [open an issue on the repository](https://github.com/frmoretto/agentic-standards-map/issues).

## Contributing

Corrections and additions based on public sources are welcome: see [CONTRIBUTING.md](CONTRIBUTING.md). Each change is dated.

## Licence

Content (entries, notes, `MAP.md`, `map-bundle.md`): [CC BY 4.0](LICENSE). Code (`tools/`): [MIT](LICENSE-CODE).

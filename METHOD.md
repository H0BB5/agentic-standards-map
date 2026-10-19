# Method

## Note on the use of AI assistance

The author used large language model assistants for source retrieval, for checking quotes, dates and states against the original pages where these could be read in full (partial readings are declared in the Evidence appendix), for drafting entries under the author's direction and for editing. Drafts were also reviewed by separate model passes acting as adversarial reviewers. The author reviewed every statement and its source before publication. Work files and the change log are retained. No pass to remove traces of machine assistance was applied to this text. The version covered by this note is the one stated in the header and in AI-USE.md. The tools, uses and version covered are declared in full in [AI-USE.md](AI-USE.md).

## Inclusion

An item is included if its public texts define or discuss how an agent finds, identifies, pays or transacts with a seller, a product or a service. Items that touch the subject without being on that path are listed as context entries.

Entries are grouped by the kind of body behind them: W3C, IETF, GS1, UN/CEFACT, other standards bodies (CEN/CENELEC and IEEE), AAIF, the Linux Foundation (with the projects of its Joint Development Foundation, such as DIF), independent projects (for example schema.org, ARD, the OpenID Foundation and the positions of browser vendors) and industry. Industry groups the protocols and programmes published by companies or industry consortia; EMVCo and the FIDO Alliance are consortia.

Not covered: 3GPP (its agent discovery work is surveyed in draft-jimenez-dawn-discovery-landscape-00), ETSI, ITU-T and ISO/IEC JTC 1/SC 42.

## Scope

This map documents public standardisation activity, specifications and declared commitments. It does not measure market adoption, transaction volume, cross-protocol interoperability or the reliability of deployed implementations. Implementation claims are reported only where supported by dated public evidence and are not treated as evidence of interoperability.

llms.txt is cited in the entry ard (a Lighthouse audit) and is not assessed in this version.

## Rules

1. **Public sources only.** Every statement points to a public URL and the date it was read. No private correspondence, paraphrased or not.
2. **Committed, not predicted.** "Committed next" means a deliverable, a scheduled event or an intention declared by the responsible body, with a date where one was given. Estimates by individual participants are not listed.
3. **No proposals.** Gaps and overlaps are recorded as facts. What to do about them belongs elsewhere.
4. **Dated.** Each entry carries `as of` and `verified` dates.
5. **Existing surveys are cited, not redone.** Where a survey covers ground (for example draft-jimenez-dawn-discovery-landscape), the map links it and covers only what it leaves out.

## How an entry is written

Each core entry has the same fields: Status (two sentences at most, with its "as of" date); Relevance to commerce; Committed next (declared items only); Boundary (what the item declares out of scope); Author participation (only where the author of this map took part, see Disclosure); Sources (primary URLs). Context entries have a short status, a line of relevance and sources.

## Source classes

Every source is tagged with one of four classes, shown in the text: **normative text** (specification, charter, schema, repository rule); **official decision or commitment** (merged change, press release, ballot, announcement); **maintainer or chair statement**; **participant or third party**. A statement of a participant or a third party is never presented as the position of the venue. Open proposals by third parties are in their own appendix, with author, date and state.

## How to read the negatives

A negative is always written as "not found in [corpus, date]": it describes the texts that were searched, not the world. What was read and what was not is in the appendix "Evidence and coverage".

## Internet-Drafts at the IETF

An Internet-Draft is not an IETF decision, and the map says which kind of draft it names. A **working group document** is a draft a working group has adopted; its name begins `draft-ietf-` followed by the group. An **individual Internet-Draft** has no working group: the datatracker lists it under "Individual Submissions" and shows no stream. Wherever the map names an individual draft it calls it individual, and an entry that exists only to list such drafts says so in its status. The datatracker states the standing of an individual draft in these words, copied on 2026-10-16 from the page https://datatracker.ietf.org/doc/draft-ranjbar-dane-did/: "This document is an Internet-Draft (I-D). Anyone may submit an I-D to the IETF. This I-D is not endorsed by the IETF and has no formal standing in the IETF standards process." The sentence holds for every individual draft in the map, including those named inside an entry whose organisation is IETF: that field names the venue of the work item (a charter, a list, a BoF), not an endorsement of the drafts the entry mentions. The group and the date of each draft named in the map were read on the datatracker (2026-10-13 to 2026-10-16).

## Versions and citation

The website is the living version and changes as venues move. Each DOI identifies a frozen snapshot: version 1.0.1 (2026-10-14) is the tag v1.0.1 of the repository and has the version DOI 10.5281/zenodo.23377309; version 1.0.0 is the tag v1.0.0 and has the version DOI 10.5281/zenodo.23357362. The concept DOI 10.5281/zenodo.23357361 always resolves to the latest version; cite the version DOI for the text you read. Version 1.1 (2026-10-19) is the version shown on the site; its tag and its version DOI are recorded here when it is released.

Changes verified by Friday evening enter the following Monday's release; a Monday with no change to citable content produces no new version. Corrections and proposals go through issues on the repository, one per entry, so that each change has a public trail.

Archive copies: snapshots of the cited sources were requested on 2026-10-14 from the Wayback Machine of the Internet Archive, and the failed ones were requested again, in part, on 2026-10-15. Of 576 distinct URLs of the entries and notes, 357 now have a snapshot (291 saved on request, 66 that already had a copy from 2026-10-01 or later), 211 failed (206 of them with an error of the service) and 8 were not requested (a login, a token, a placeholder or a Google Doc). Where a snapshot exists, `map.json` and the JSON of the entry carry it in an `archived` field next to the URL, and the entry page links it. A snapshot is a copy kept by a third party, taken at the time shown in its address; it is not the text read on the date of reading.

**Changelog.**

**1.1 (2026-10-19).** Two entries added; corrections and additions to the living version.

- New entries: `anp` (issue #6) and `accord-project` (issue #1).
- `a2a-core`, `a2a-discovery`: org corrected from Linux Foundation to AAIF; A2A joined AAIF as a hosted project (AAIF, 2026-08-17; Growth Stage, A2A blog of 2026-08-27) (issues #7 and #8).
- `mcp-core`, `mcp-server-card`: org corrected from Linux Foundation to AAIF; MCP is listed among AAIF's projects, and the Server Card is the work of an MCP Working Group (issues #9 and #10).
- `aaif-structure`: hosted projects listed from aaif.io/projects (issue #13).
- `ap2`: date of the donation and Google's announcement added, with the FIDO working groups named in the FIDO release; the wording of the status and of the governance row stays open in issue #11.
- `fido-agentic-standards`: Google's "donating" reported next to FIDO's "contributed" (issue #12).
- Proposals: A2A issue #2323 under `a2a-core` (issue #5); A2A issue #2043 under `a2a-discovery` (issue #4); did:dns issue #12 and draft-ranjbar-dane-did under `ietf-dnsaid` (issue #3); draft-ranjbar-dane-anchored-identity added to `ietf-dnsaid` (issue #2).
- IETF: individual Internet-Drafts are now labelled as individual wherever they are named, and the Method gives the Datatracker's wording on their standing; one entry no longer calls an individual submission an "Independent Submission".
- IETF revisions updated: `draft-agentic-ai-usecases-requirements` -04 (`ietf-agentproto`) and `draft-zhang-dawn-agent-discovery-framework` -07 (`ietf-dawn`), read on the datatracker on 2026-10-16.
- `w3c-ai-agent-protocol-cg`: overlap with `anp` added.
- 2026-10-16, update cadence: the header, the footer and the page for agents and tools say the map is updated weekly; Method and CONTRIBUTING state that numbered versions go out on Mondays.
- 2026-10-15, `dif-trusted-ai-agents`: org corrected to Linux Foundation, reported by a DIF participant on the AAIF Taxonomy list.
- 2026-10-15, CONTRIBUTING and issue template: proposals now state the proposer's role and any employer or commercial interest.
- 2026-10-15, header: the citable version and the date of the live site are shown separately.
- Credit: corrections proposed by Alan Blount (zeroasterisk) in issues #7-#13 and PR #14.

**1.0.1 (2026-10-14).** Corrections and additions to the living version; no entry was added or removed.

- DAWN: the example "discover all agents in this shop" is given as the example of the local network, not as a commercial example on the web; the example of the public Internet is "discover all agents of example.org, for all its customers/members".
- Seam S1: the redirect rules of UCP and of the Personal Agent Protocol are said to differ (different paths and different readers), not to be opposite.
- Home and S1: the count of discovery paths is eight (the home page counted seven and left out the poppy.json of the Personal Agent Protocol).
- Disclosure: the pull request on the W3C charter drafts is recorded as merged on 2026-10-13.
- UCP: the census figure called "row 2" is "row 2 and ucp.version present", as its author wrote on 2026-10-14.
- Calendar: three provisional TPAC breakout slots, with their source and the conversion to Rome time.
- AI-USE.md: the hash it carries is that of the bundle of the released version, and the export checks it against the tag.
- Disclosure: the presentation to the AAIF Agentic Commerce Working Group is recorded as given on 2026-10-14, with the list message of that day.
- Disclosure: the time of the DAWN list message of 2026-09-25 is removed; the date stays.
- IANA: a registration request for `ucp` has been open in the registry's repository since 2026-06-06 (issue #92), and is recorded in S1 and in the UCP entry.
- TPAC: the entry follows the breakout calendar of 2026-10-14 (85 sessions, all marked tentative).
- Sources: archive links in `map.json`, in the JSON of each entry and on the entry pages.
- Presentation: the table "Payment protocols compared" has four columns, short labels for the source links, and may be wider than the text column; the text of its cells did not change.

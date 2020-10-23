---
qip: 0
title: QIP Purpose and Guidelines
status: Implemented
author: QIAN Community
discussions-to: https://forum.qian.finance/
created: 2020-10-22
updated: 2020-10-23
---

## What is an QIP?

QIP stands for QIAN Improvement Proposal, it has been adapted from the SIP (Synthetix Improvement Proposal). The purpose of this process is to ensure changes to QIAN are transparent and well governed. An QIP is a design document providing information to the QIAN community about a proposed change to the system. The author is responsible for building consensus within the community and documenting dissenting opinions.

## QIP Rationale

We intend QIPs to be the primary mechanisms for proposing new features, collecting community input on an issue, and for documenting the design decisions for changes to QIAN. Because they are maintained as text files in a versioned repository, their revision history is the historical record of the feature proposal.

It is highly recommended that a single QIP contain a single key proposal or new idea. The more focused the QIP, the more successful it is likely to be.

An QIP must meet certain minimum criteria. It must be a clear and complete description of the proposed enhancement. The enhancement must represent a net improvement.

## QIP Work Flow

Parties involved in the process are the *author*, the [*QIP editors*](#qip-editors), and the QIAN community.

:warning: Before you begin, vet your idea, this will save you time. Ask the QIAN community first if an idea is original to avoid wasting time on something that will be rejected based on prior research (searching the Internet does not always do the trick). It also helps to make sure the idea is applicable to the entire community and not just the author. Just because an idea sounds good to the author does not mean it will have the intend effect. The appropriate public forum to gauge interest around your QIP is [the official QIAN Discord].

Your role as the champion is to write the QIP using the style and format described below, shepherd the discussions in the appropriate forums, and build community consensus around the idea. Following is the process that a successful QIP will move along:

```
Proposed -> Approved -> Implemented
  ^                     |
  +----> Rejected       +----> Moribund
  |
  +----> Withdrawn
  v
Deferred
```

Each status change is requested by the QIP author and reviewed by the QIP editors. Use a pull request to update the status. Please include a link to where people should continue discussing your QIP. The QIP editors will process these requests as per the conditions below.

* **Work in progress (WIP)** -- Once the champion has asked the QIAN community whether an idea has any chance of support, they will write a draft QIP as a [pull request]. Consider including an implementation if this will aid people in studying the QIP.
* **Proposed** If agreeable, QIP editor will assign the QIP a number (generally the issue or PR number related to the QIP) and merge your pull request. The QIP editor will not unreasonably deny an QIP. Proposed QIPs will be discussed on governance calls and in Discord. If there is a reasonable level of consensus around the change on the governance call the change will be moved to approved. If the change is contentious a vote of token holders may be held to resolve the issue or approval may be delayed until consensus is reached.
* **Approved** -- This QIP has passed community governance and is now being prioritised for development.
* **Implemented** -- This QIP has been implemented and deployed to mainnet.
* **Rejected** -- This QIP has failed to reach community consensus.
* **Withdrawn** -- This QIP has has been withdrawn by the author(s).
* **Deferred** -- This QIP is pending another QIP/some other change that should be bundled with it together.
* **Moribund** -- This QIP has been implemented and is now obsolete and requires no explicit replacement.

## What belongs in a successful QIP?

Each QIP should have the following parts:

- Preamble - RFC 822 style headers containing metadata about the QIP, including the QIP number, a short descriptive title (limited to a maximum of 44 characters), and the author details.
- Simple Summary - “If you can’t explain it simply, you don’t understand it well enough.” Provide a simplified and layman-accessible explanation of the QIP.
- Abstract - a short (~200 word) description of the technical issue being addressed.
- Motivation (*optional) - The motivation is critical for QIPs that want to change QIAN. It should clearly explain why the existing specification is inadequate to address the problem that the QIP solves. QIP submissions without sufficient motivation may be rejected outright.
- Specification - The technical specification should describe the syntax and semantics of any new feature.
- Rationale - The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.
- Test Cases - Test cases may be added during the implementation phase but are required before implementation.
- Copyright Waiver - All QIPs must be in the public domain. See the bottom of this QIP for an example copyright waiver.

## QIP Formats and Templates

QIPs should be written in [markdown] format.
Image files should be included in a subdirectory of the `assets` folder for that QIP as follows: `assets/qip-X` (for qip **X**). When linking to an image in the QIP, use relative links such as `../assets/qip-X/image.png`.

## QIP Header Preamble

Each QIP must begin with an [RFC 822](https://www.ietf.org/rfc/rfc822.txt) style header preamble, preceded and followed by three hyphens (`---`). This header is also termed ["front matter" by Jekyll](https://jekyllrb.com/docs/front-matter/). The headers must appear in the following order. Headers marked with "*" are optional and are described below. All other headers are required.

` qip:` <QIP number> (this is determined by the QIP editor)

` title:` <QIP title>

` author:` <a list of the author's or authors' name(s) and/or username(s), or name(s) and email(s). Details are below.>

` * discussions-to:` \<a url pointing to the official discussion thread at forum.qian.finance\>

` status:` < WIP | PROPOSED | APPROVED | IMPLEMENTED >

` created:` <date created on>

` * updated:` <comma separated list of dates>

` * requires:` <QIP number(s)>

` * resolution:` \<a url pointing to the resolution of this QIP\>

Headers that permit lists must separate elements with commas.

Headers requiring dates will always do so in the format of ISO 8601 (yyyy-mm-dd).

#### `author` header

The `author` header optionally lists the names, email addresses or usernames of the authors/owners of the QIP. Those who prefer anonymity may use a username only, or a first name and a username. The format of the author header value must be:

> Random J. User &lt;address@dom.ain&gt;

or

> Random J. User (@username)

if the email address or GitHub username is included, and

> Random J. User

if the email address is not given.

#### `discussions-to` header

While an QIP is in WIP or Proposed status, a `discussions-to` header will indicate the URL at [forum.qian.finance](https://forum.qian.finance/) where the QIP is being discussed.

#### `created` header

The `created` header records the date that the QIP was assigned a number. Both headers should be in yyyy-mm-dd format, e.g. 2001-08-14.

#### `updated` header

The `updated` header records the date(s) when the QIP was updated with "substantial" changes. This header is only valid for QIPs of Draft and Active status.

#### `requires` header

QIPs may have a `requires` header, indicating the QIP numbers that this QIP depends on.

## Auxiliary Files

QIPs may include auxiliary files such as diagrams. Such files must be named QIP-XXXX-Y.ext, where “XXXX” is the QIP number, “Y” is a serial number (starting at 1), and “ext” is replaced by the actual file extension (e.g. “png”).

## QIP Editors

The current QIP editors are:

` * David (@Master-LY)`

` * Mirai (@Mingliang233)`

## QIP Editor Responsibilities

For each new QIP that comes in, an editor does the following:

- Read the QIP to check if it is ready: sound and complete. The ideas must make technical sense, even if they don't seem likely to get to final status.
- The title should accurately describe the content.
- Check the QIP for language (spelling, grammar, sentence structure, etc.), markup (Github flavored Markdown), code style

If the QIP isn't ready, the editor will send it back to the author for revision, with specific instructions.

Once the QIP is ready for the repository, the QIP editor will:

- Assign an QIP number (generally the PR number or, if preferred by the author, the Issue # if there was discussion in the Issues section of this repository about this QIP)

- Merge the corresponding pull request

- Send a message back to the QIP author with the next step.

The QIP editors monitor QIP changes, and correct any structure, grammar, spelling, or markup mistakes we see.

The editors don't pass judgment on QIPs. We merely do the administrative & editorial part.

## History

The QIP document was derived heavily from the SIP Synthetix Improvement Proposal document in many places text was simply copied and modified. Any comments about the QIP document should be directed to the QIP editors.

### Bibliography

[the official QIAN Discord]: https://discord.gg/MYKm35s
[pull request]: https://github.com/QIAN-Protocol/QIPs/pulls
[markdown]: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

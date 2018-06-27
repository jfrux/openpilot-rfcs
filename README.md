# openpilot RFCs

Many changes, including bug fixes and documentation improvements can be
implemented and reviewed via the normal commaai/openpilot GitHub pull request workflow.

Some changes though are "substantial", and my thoughts are that these be put
through a bit of a design process and produce a consensus among the openpilot community.

The "RFC" (request for comments) process is intended to provide a
consistent and controlled path for new features to enter the codebase & ui.

## When should you follow this process

I recommend you follow this process if you intend to make "substantial"
changes to openpilot, or its documentation. What constitutes a
"substantial" change is evolving based on community norms, but may
include the following.

   - A new feature that creates new surface area, require significant changes if introduced, and could be included a NEW FEATURE of openpilot.
   - The removal of features that already shipped as part of a release.
   - The introduction of new idiomatic usage or conventions, even if they
     do not include code changes to openpilot itself.

Some changes do not require an RFC:

   - Rephrasing, reorganizing or refactoring
   - Addition or removal of warnings
   - Additions that strictly improve objective, numerical quality
criteria (speedup, better performance)
   - Additions only likely to be _noticed by_ other implementors-of-openpilot,
invisible to drivers-of-openpilot.

<!-- If you submit a pull request to implement a new feature without going
through the RFC process, it may be closed with a polite request to
submit an RFC first. -->

## Gathering feedback before submitting

It's often helpful to get feedback on your concept before diving into the
level of design detail required for an RFC. **You may open an
issue on this repo to start a high-level discussion**, with the goal of
eventually formulating an RFC pull request with the specific implementation
design.

## What the process is

In short, one should first get the
RFC merged into the RFC repo as a markdown file. At that point the RFC
is open to consideration by the community and may be implemented with the goal of eventual inclusion
into openpilot by developers in the community or Comma.ai themselves if they decide they support the proposals.

* Fork the RFC repo http://github.com/jfrux/openpilot-rfcs
* Copy `0000-template.md` to `text/0000-my-feature.md` (where
'my-feature' is descriptive. don't assign an RFC number yet).
* Fill in the RFC. Put care into the details: **RFCs that do not
present convincing motivation, demonstrate understanding of the
impact of the design, or are disingenuous about the drawbacks or
alternatives tend to be poorly-received**.
* Submit a pull request. As a pull request the RFC will receive design
feedback from the larger community, and the author should be prepared
to revise it in response.
* Build consensus and integrate feedback. RFCs that have broad support
are much more likely to make progress than those that don't receive any
comments.
* Eventually, the community will decide whether the RFC is a candidate
for inclusion in openpilot and whether to create an official PR.
* An RFC can be modified based upon feedback from the community.
Significant modifications may trigger a new final comment period.
* An RFC may be rejected by the community after public discussion has settled
and comments have been made summarizing the rationale for rejection. A member of
the openpilot community should then close the RFC's associated pull request.
* At any point an RFC maybe accepted and developed by a community developer or designer and it is recommended that you leave a comment on this RFC noting the repository fork / change.

## The RFC life-cycle

Once an RFC is created then authors should make every attempt to implement it and submit the
feature as a pull request to the commaai/openpilot repo.

Furthermore, the fact that a given RFC is created implies nothing about what priority is assigned to its
implementation, nor whether anybody is currently working on it.

Modifications to RFC's can be done in followup PR's. We strive
to write each RFC in a manner that it will reflect the final design of
the feature; but the nature of the process means that we cannot expect
every merged RFC to actually reflect what the end result will be at
the time of the next major release; therefore we try to keep each RFC
document somewhat in sync with the language feature as planned,
tracking such changes via followup pull requests to the document.

## Implementing an RFC

The author of an RFC is not obligated to implement it. Of course, the
RFC author (like any other developer / designer) is welcome to post an
implementation for review after the RFC has been merged.

If you are interested in working on the implementation for an RFC, but cannot determine if someone else is already working on it,
feel free to ask (e.g. by leaving a comment on the associated issue or via Comma Slack).

## Reviewing RFC's

Each week someone from the community appointed members that moderate the RFCs repository will attempt to review some set of open RFC
pull requests.

We try to make sure that any RFC that is created will be merged weekly. Every
merged RFC should ideally have a referenced `fork` or `branch` of `commaai/openpilot` and optionally an existing PR associated with it.

**We owe this RFC process to the [Rust RFC process]**

[Rust RFC process]: https://github.com/rust-lang/rfcs
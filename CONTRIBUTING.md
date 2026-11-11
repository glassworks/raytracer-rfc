# How we decide

## Words

The key words MUST, MUST NOT, REQUIRED, SHALL, SHALL NOT, SHOULD, SHOULD NOT, RECOMMENDED, NOT RECOMMENDED, MAY and OPTIONAL in this RFC are to be interpreted as described in BCP 14 (RFC 2119, RFC 8174) when, and only when, they appear in all capitals.

Write in English.

## A question or an idea: an issue

Open an issue, with the label of its part. Give the options you see, and what each one costs.

## A change: a pull request

- One topic per pull request.
- Fill in the template: what changes, why, and what else you considered.
- Change the text, the examples and the schemas together.
- Worked with someone? Add a line to your commit message for each of them, so that it counts for them too:

  ```text
  Co-authored-by: Their Name <their-github-email>
  ```

## Reviews

Anyone can review, and everyone should. A review says what is wrong or missing and why, or proposes a better wording. "LGTM" alone adds nothing.

Use "Request changes" for a problem that must be fixed before merging, and say what would fix it.

## Merging

An editor merges a pull request with "Squash and merge" when:

1. two editors from groups other than the author's have approved it;
2. no change request is left unanswered, and every conversation is resolved;
3. it has been open for at least 4 hours of the working day, so that others could see it, unless it writes down a decision of Thursday's meeting;
4. for parts 06 and 07, the client has approved it.

## When we can't agree

If reviews can't settle it, add the label `meeting`. The meeting on Thursday 10 December, at 9:00, settles every `meeting` issue: each side makes its case in two minutes, then the chair takes a hum, as the IETF does (RFC 7282). A hum isn't a vote: it shows whether a strong objection remains. The decision is written in the issue at once, then in a pull request.

## Versions

- **Thursday 10 December, 13:00: v1.0.** The editors tag it. From then on, only errata: a fix or a clarification that doesn't make a working implementation wrong. Label: `errata`.
- **Friday 11 December, 18:00: final.** The editors tag the last commit. No more changes. A question about the text goes in an issue: the editors answer by quoting the text, and where the text doesn't say, the client decides, in the issue.
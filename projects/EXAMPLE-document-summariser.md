---
title: Long document summariser
goal: understand a long document fast
tools: [claude]
sensitivity: [🟡 private-data, 🟡 private-code]
status: [✅ status-active]
job: [👥 any-role]
effort: [⚡ effort-5-min]
tokens: [🪙 tokens-low]
---

# Long document summariser

> This turns a document you do not have time to read into the few things in it
> that actually affect your work.

**Written by:** [@kuidja] · **Last checked:** August 2026

---

## Why this is worth your time

Reading a forty page spec to find the two paragraphs that concern you takes
about an hour. This takes five minutes, and it tells you whether that hour is
worth spending.

---

## Try it in five minutes

1. Open Claude and sign in with your Canonical account.
2. Paste the document in, or upload it.
3. Ask it this: *"I am a visual designer. What in this document changes what I
   do? Please separate the things I have to act on from the things I only need
   to be aware of."*

You should get back a short list split into two groups.

---

## The full process

1. Do everything above.
2. Then ask a follow-up question: *"Quote the exact lines you based the first
   group on."*
3. Read only those parts of the original document.

**Does it need setting up first?** No.

**How do you get access?** Sign in to Claude with your Canonical account.

---

## Adapt, don't clone

The single most important thing to change is the role. Swap "visual designer"
for whatever you actually do, because the answer changes completely depending
on what you tell it. That substitution is the whole trick, so please do not
skip it.

The follow-up question that asks for quotes matters more than the summary
itself. Without it you are trusting a summary you have not checked. If the
model cannot produce the lines it based something on, it probably invented it.

If your document is short enough to skim in a few minutes, this is not worth
doing at all.

---

## Where it does not work

Long tables and diagrams come out badly, because the structure gets flattened
into prose. If your document is mostly a table, read the table yourself.

Nothing above private data should go in, so please check the
[clearance page](../CLEARANCE.md) before you paste in anything sensitive.

---

## Go deeper

```
I am a [your role]. What in this document changes what I do?
Please separate the things I have to act on from the things I only
need to be aware of. Then quote the exact lines that each item in the
first group came from.
```

---
title: Alt text first drafts
goal: draft alt text for images
tools: [claude]
sensitivity: [🔴 public-data]
status: [✅ status-active]
job: [🎨 visual-design, ✏️ content]
effort: [⚡ effort-5-min]
tokens: [🪙 tokens-low]
---

# Alt text first drafts

> This drafts alt text for an image, so that you are editing something rather
> than staring at an empty field.

**Written by:** [@kuidja] · **Last checked:** August 2026

---

## Why this is worth your time

Alt text is a required check at three separate review stages, which are the
copy doc review, the Figma review and the demo review. It is also the check
most often left unfinished, mostly because writing it from a blank page is
tedious.

Starting from a draft you can correct is much quicker than starting from
nothing.

---

## Try it in five minutes

1. Open Claude and upload the image.
2. Ask it this: *"Write alt text for this image. It sits in a section about
   [your topic]. Describe what matters to someone who cannot see it, rather
   than everything that is visible. Keep it under 125 characters."*

---

## The full process

You can do the same thing in a batch. Upload several images at once and give
it the section topic for each one.

Please read every result before you paste it in, for the reasons described
below.

**Does it need setting up first?** No.

---

## Adapt, don't clone

Telling it what the section is about is what stops it describing the wrong
thing. A photograph of two people at a laptop is "a support engineer helping a
customer" in one section and "colleagues working remotely" in another, and the
model has no way of knowing which one you meant.

If your team works to a different character limit, change the number in the
prompt.

---

## Where it does not work

Decorative images are supposed to have empty alt text rather than a
description, and the model will cheerfully describe a background gradient for
you. Deciding whether an image is decorative is your call, not its.

Diagrams need somebody to describe the relationships they show, not to list
the shapes in them. Those are worth writing yourself.

---

## Go deeper

```
Write alt text for this image. It sits in a section about [topic].
Describe what matters to someone who cannot see it, rather than
everything that is visible. Keep it under 125 characters. If the image
is decorative and carries no information, say so instead of describing
it.
```

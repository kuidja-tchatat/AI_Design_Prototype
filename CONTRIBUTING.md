# How to add a page

Writing up something you have built takes about ten minutes. You do not need
anyone's approval, and you do not need to decide where your page belongs,
because everything lives in the same folder.

---

## Before you start, two things worth saying

**Please do not wait until your work is finished.** A prompt that only half
works, with a short note explaining where it breaks, is much more useful than
nothing at all. Most pages here start out marked as experimental, and that is
exactly as it should be.

**Failures are worth writing up too.** If you spent an afternoon on a tool and
it did not do what you hoped, then a page saying so will stop the next person
losing the same afternoon. Mark it `status-did-not-work` and describe what
happened. There is an example of one of those already in the repository.

---

## The four steps

### Step 1. Create the file

At the top of the repository, click **Add file**, then **Create new file**.

In the box where GitHub asks for a filename, type the whole path at once, like
this:

```
projects/my-page-name.md
```

That is the only folder in the repository, so there is no category to choose
and nothing to get wrong.

### Step 2. Copy the template into it

Open the [template](_TEMPLATE.md), select all of it, and paste it into your
new file. Then work through it and fill it in.

Short answers are completely fine. Please keep all of the headings, even where
your answer is only one line, because readers rely on every page having the
same shape. When someone opens your page looking for the limitations, they
should find them in the same place they found them on the last page they read.

If writing it out feels like a chore, there is a shortcut. Paste your rough
notes, or even a transcript of you using the tool, into an LLM along with the
template, and ask it to draft the page for you. Then read what it produced and
correct whatever it guessed wrong. The one thing you should not delegate is
the sensitivity tag, which you need to set yourself.

### Step 3. Fill in the tags at the top

The small block of tags at the top of the file is what makes your page
findable by anybody else.

Four of them are required: `goal`, `tools`, `sensitivity` and `status`. Three
more are optional but helpful: `job`, `effort` and `tokens`.

Copy the exact wording from the [tag list](TAGS.md), because search only
matches what is literally written in the file.

### Step 4. Save it

Scroll to the bottom of the page, write a short description of what you are
adding, something like "Add spec drafting prompt", and click **Commit
changes**. Your page is now live.

If you have another ten seconds, add a row for your page to the
[index](INDEX.md). It helps the people who prefer browsing to searching.

---

## The one thing that really does need to be right

Everything you write on your page is your own honest experience, and nobody is
going to hold you to it if your workflow turns out not to suit them.

The exception is the `sensitivity` tag. That one is a factual claim about what
is safe to put through a tool, rather than an opinion about whether your
project is any good. Somebody may rely on it when deciding whether to paste in
a customer interview.

So please check the [tool clearance page](CLEARANCE.md) rather than guessing,
and if you are still unsure, ask in the `ai-tooling` channel before you post
the page.

---

## Writing so that other people can reuse it

The most valuable section on any page is the one called "Adapt, don't clone".

People on this team have been clear that they do not want to copy someone
else's workflow exactly. They want a starting point that they understand well
enough to change. That means the useful thing you can tell them is which parts
of your page are specific to you.

Your file structure, the name of your project, the way your team phrases
things, the particular document you were working on. All of that will need
swapping out by whoever reads your page. Saying so directly saves them working
it out by trial and error.

---

## Keeping your page honest over time

If your workflow proves reliable, change `status-experimental` to
`status-active`.

If it stops working, perhaps because the tool changed, change the status to
`status-did-not-work` and write a line explaining what broke. While you are
there, update the "Last checked" date.

A page that quietly goes out of date is worse than no page at all, because
somebody will follow it and waste their time.

---

## Finally

If anything about this process confused you while you were adding your page,
please say so in the `ai-tooling` channel.

Confusion is a bug in the repository rather than a failing on your part, and
it is the easiest kind of bug for us to fix.

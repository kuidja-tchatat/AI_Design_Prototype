# AI projects, from the design team

Welcome. This is a shared place where people on the design team write up the
things they have built with AI, so that everyone else can use them too.

Someone on the team spends an afternoon working out how to get Claude to draft
a spec properly. Right now, that knowledge stays with them. The next person
starts from zero and spends the same afternoon. This repository exists so that
the second person does not have to.

Each thing someone built gets one page. A page might describe a prompt, a
skill, a full agent setup, or simply a tool that somebody tried. All of these
pages live in a single folder called [`projects/`](projects/).

You do not need to read this whole page. Below are the four things you might
want to do, in the order you will probably want to do them.

---

## 1. Finding something useful

There are no categories to click through in this repository. Instead, every
page carries a short list of tags, and you search for the tag you care about.

There are seven tags in total, covering what a page is for, which tools it
needs, what information is safe to put in, whether it can be trusted, who it
is relevant to, how long it takes, and what it costs to run. Every tag and
every value it can take is listed in the [tag page](TAGS.md).

### How a search actually works

Go to the top of this page and find the box that says **Search this
repository**. Type a tag into it exactly as it is written on the tag page,
then press enter.

For example, typing `visual-design` into that box gives you every page that
somebody has tagged as relevant to visual designers. Behind the scenes GitHub
turns that into a web address that looks like this, which you can also just
type directly or bookmark:

```
https://github.com/kuidja/design-ai-projects/search?q=visual-design
```

You can search for two tags at once to narrow things down, which is usually
what you want. Typing `visual-design effort-5-min` gives you only the quick
wins that are relevant to visual designers.

### The searches people use most

| What you are thinking | What to type | Which tag group that is |
|---|---|---|
| "Something relevant to my job." | `visual-design`, `ux-design`, `ux-research`, `content`, `web-dev` | Job |
| "I already have this tool open." | `claude`, `copilot`, `gemini`, `figma-make`, `notebooklm` | Tools |
| "I have ten minutes." | `effort-5-min` | Effort |
| "Is this safe for internal work?" | `private-data`, `confidential-data` | Sensitivity |
| "Only things people rely on." | `status-active` | Status |
| "What has already failed?" | `status-did-not-work` | Status |
| "Something cheap to run." | `tokens-low` | Tokens |

That table only shows the most common searches. The
[full list of tags](TAGS.md) has every value in every group, laid out in
tables.

### If you would rather browse than search

If you do not yet know what you are looking for, searching is the wrong tool.
There are three ways to browse instead.

| Where to go | What it gives you |
|---|---|
| [The index](INDEX.md) | Every page in one table, grouped by job and by tool |
| [The tag page](TAGS.md) | Every tag and every value, so you can pick a search term |
| [`projects/`](projects/) | The raw list of every page in the repository |

---

## 2. Checking a page before you use it

Once you have found something that looks useful, there are three things worth
checking before you try it. All three sit near the top of every page, and
looking at them takes about ten seconds.

| What to check | Why it matters |
|---|---|
| The `sensitivity` tag | It tells you what kind of information is safe to put into the tool. Then confirm the tool itself is cleared for that level on the [clearance page](CLEARANCE.md) |
| The `status` tag | `status-active` means somebody relies on it. `status-experimental` means one person tried it once. `status-did-not-work` means read it and stop |
| The "Last checked" date | AI tools change quickly. A page written six months ago may describe behaviour the tool no longer has |

There is one trap worth knowing about. A tool that has been approved for
confidential **code** has usually not been approved for confidential **data**.
GitHub Copilot is the clearest example. You can point it at an internal
repository, but you should not paste meeting notes into it. If your work
touches both code and documents, check both columns on the clearance page.

---

## 3. Actually using what you found

Every page in this repository follows the same structure, which means you can
jump straight to the part you need instead of reading the whole thing.

| Section | What it gives you |
|---|---|
| Why this is worth your time | Whether the problem it solves is a problem you have |
| Try it in five minutes | The smallest useful version, with nothing to set up. Start here |
| The full process | What the author actually does for real work |
| Adapt, don't clone | Which parts are specific to the author, and what you need to change |
| Where it does not work | The honest limits |
| Go deeper | The prompt or configuration, written out in full so you can copy it |

The section worth reading properly is **Adapt, don't clone**. People on this
team have said clearly that they do not want to copy someone else's workflow
exactly. They want a starting point they understand well enough to modify, and
that section is what makes it possible.

In practice, using a page usually means copying the prompt from the bottom,
changing the parts that describe the author's situation into ones that
describe yours, and running it. Unless a page tells you otherwise, there is
nothing to install.

---

## 4. Adding a page of your own

If you have built something, or even half built something, please write it up.
It takes about ten minutes and you do not need anyone's permission.

You also do not need to decide where your page belongs, because there is only
one folder. This is deliberate, and the reasoning is explained at the bottom
of this page.

Please do not wait until your work is polished. A prompt that only half works,
with a note explaining where it breaks, is far more useful than nothing at
all. Most pages here start out as `status-experimental` and that is completely
normal.

Failures are worth writing up as well. If you spent an afternoon on a tool and
it did not do what you hoped, a short page saying so will save the next person
that same afternoon. There is an example of one of those in this repository
already.

| What you need | Where it is |
|---|---|
| The step by step instructions | [Contributing guide](CONTRIBUTING.md) |
| The blank file to copy | [Template](_TEMPLATE.md) |
| The tag values to fill in | [Tag page](TAGS.md) |
| A finished page to look at | Any file in [`projects/`](projects/) starting with `EXAMPLE-` |

If the tag you need does not exist yet, you are allowed to invent one. The
only rule is that you add it to the [tag page](TAGS.md) in the same commit, so
that it stops being private to you.

---

## If a word here does not mean anything to you

Some of the language around AI tooling is genuinely unhelpful. Words like MCP,
agent, skill, context file, token and VM get used constantly without anyone
explaining them.

The [glossary](GLOSSARY.md) explains each of them in plain language. If a word
is missing from it, please add the word with a question mark next to it. A term
that nobody can define is a useful signal about what needs explaining.

---

## Why this repository has no folders

Every page sits in one flat folder, and there are no categories at all. This
is a deliberate choice, and it is worth explaining because it looks unusual.

When a repository is organised into categories, the person adding a page has
to guess which category their work belongs to. Is a competitor analysis
"research" or "discovery"? Different people answer that differently, so
similar things end up scattered across several folders and nobody can find
anything.

Tags do not have this problem. A single page can be tagged for two different
jobs and three different tools at the same time, and a search will find it
under any of them. Nobody has to guess, and nothing gets filed in the wrong
place, because there is no wrong place.

The cost of this approach is that a flat list becomes harder to skim once
there are a lot of pages in it. That is what [INDEX.md](INDEX.md) is for. It
gives you the grouped view without forcing anyone to file their work into a
category first.

---

*This is a prototype, built by Kuidja for the AI Design Ops repository
exercise in August 2026. The example projects in it are invented. The point of
the exercise is the structure, not the content.*

# Glossary

A lot of the language around AI tooling gets used as though everybody already
knows it. This page explains the words in plain terms.

If a word you needed is not here, please add it, even if you cannot define it
yourself. Writing the word down with a question mark next to it tells us
exactly what needs explaining.

---

## Words about AI

**Agent.** An AI that works through several steps on its own, rather than
answering a single question and stopping. You give it a goal and it decides
what to do next as it goes.

**Context file.** A file you hand to the AI so that it understands your
situation before you ask it anything. It is often called `context.md`. The
easiest way to think about it is as the briefing you would give a freelancer
before they start work.

**LLM, which stands for large language model.** This is the kind of AI behind
Claude, Gemini and ChatGPT. It works with text.

**MCP, which stands for Model Context Protocol.** This is a standard way of
connecting a tool to an AI so that the AI can use it directly. It is what
allows an AI to read your Figma file itself, instead of you copying things out
of Figma and pasting them in.

**Prompt.** What you type to the AI. The instruction.

**Skill.** A saved set of instructions that the AI follows for a task you do
repeatedly. It is a prompt you do not have to write out again every time.

**Token.** The unit that AI usage is measured and paid for in. Roughly
speaking, a token is a fragment of a word, so longer documents cost more.
Everybody has a monthly budget, which is why people ration what they use.

---

## Words about the tools around it

**CLI, which stands for command line interface.** Using a tool by typing
commands rather than clicking. It is the black window full of text.

**Repository, usually shortened to repo.** A project folder on GitHub. It is
not more complicated than that.

**README.** The page GitHub shows you automatically when you open a folder.
Every folder is allowed to have one.

**Markdown, written as `.md`.** Plain text with a few simple formatting marks.
A `#` makes a heading, a `-` makes a bullet point, and text wrapped in
asterisks becomes bold. That covers most of what you will ever need.

**YAML front matter.** The small block of tags between two lines of three
dashes at the top of a page. The [tag list](TAGS.md) explains what goes in it.

**PR, which stands for pull request.** A proposed change to a repository that
somebody reviews before it is accepted.

**VM, which stands for virtual machine.** A simulated computer running inside
your own computer, kept separate from everything else on it. The plan for this
project is to run AI agents inside one, so that they cannot reach sensitive
files by accident.

---

## Words used around Canonical

**BAU, which stands for business as usual.** The ongoing work of building and
refreshing pages on canonical.com and ubuntu.com.

**Copy doc.** The Google Doc that holds the text for a page. It is owned by
the product or marketing manager who requested the page.

**Cycle.** Six months. It is the period the roadmap is planned across.

**Pulse.** Two weeks. It is the iteration the team works in.

**Pragma.** Canonical's new design system. It used to be called DS25.

**Vanilla.** The CSS framework and pattern library that the websites are built
on.

**Diátaxis.** Canonical's documentation framework. It argues that
documentation comes in four distinct kinds, which are tutorials, how-to
guides, reference and explanation, and that mixing them together is what makes
documentation confusing. You can read it at
[diataxis.fr](https://diataxis.fr/start-here/).

---

## Words used in this repository

**Goal.** What a page is for, written in the author's own words rather than
chosen from a fixed list of categories.

**Sensitivity.** What kind of information is safe to put into a given tool.
The [clearance page](CLEARANCE.md) explains it.

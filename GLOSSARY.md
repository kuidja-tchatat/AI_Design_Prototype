# Glossary

A lot of the language around AI tooling gets used as though everybody already
knows it. This page explains the words in plain terms.

If a word you needed is not here, please add it, even if you cannot define it
yourself. Writing the word down with a question mark next to it tells us
exactly what needs explaining.

---

## Words about AI

**Agent :** An AI that works through several steps on its own, rather than
answering a single question and stopping. You give it a goal and it decides
what to do next as it goes.

**Context file :** A file you hand to the AI so that it understands your
situation before you ask it anything. It is often called `context.md`. The
easiest way to think about it is as the briefing you would give a freelancer
before they start work.

**LLM (large language model) :** a type of artificial intelligence program trained on massive amounts of text to understand, interpret, and generate human-like language. This is the kind of AI behind
Claude, Gemini and ChatGPT. It works with text.

**MCP (Model Context Protocol) :** An open standard introduced by Anthropic that acts like a universal "USB-C port" for connecting AI applications to external data sources, tools, and workflows. It is what
allows an AI to read your Figma file itself, instead of you copying things out
of Figma and pasting them in.

**Prompt :** What you type to the AI. The instruction.

**Skill :** A saved set of instructions that the AI follows for a task you do
repeatedly. It is a prompt you do not have to write out again every time.

**Token.** The unit that AI usage is measured and paid for in. Roughly
speaking, a token is a fragment of a word, so longer documents cost more.
Everybody has a monthly budget, which is why people ration what they use.

---

## Words about the tools around it

**CLI (command line interface):** Using a tool by typing
commands rather than clicking. It is the black window full of text.

**Repository (usually shortened to repo):** A project folder on GitHub. It is
not more complicated than that.

**README :** The page GitHub shows you automatically when you open a folder.
Every folder is allowed to have one.

**Markdown (written as `.md`):** Plain text with a few simple formatting marks.
A `#` makes a heading, a `-` makes a bullet point, and text wrapped in
asterisks becomes bold. That covers most of what you will ever need.

**YAML front matter :** The small block of tags between two lines of three
dashes at the top of a page. The [tag list](TAGS.md) explains what goes in it.

**PR (pull request) :** A proposed change to a repository that
somebody reviews before it is accepted.

**VM (virtual machine) :** A simulated computer running inside
your own computer, kept separate from everything else on it. The plan for this
project is to run AI agents inside one, so that they cannot reach sensitive
files by accident.

---

## Words used in this repository

**Sensitivity :** What kind of information is safe to put into a given tool.
The [clearance page](CLEARANCE.md) explains it.

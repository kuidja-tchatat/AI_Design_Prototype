# Tags, and what they mean

This repository has no folders and no categories. Tags do all of the sorting
instead, which makes this page both the map and the search menu.

There are seven tags in total. Four of them are required on every page, and
three are optional. This page lists every one of them, along with every value
they are allowed to take.

If you are adding a page, this is the page you copy your values from. If you
are looking for something, this is the page you pick your search terms from.

---

## The seven tags at a glance

| Tag | Required? | How many values | What it tells the reader |
|---|---|---|---|
| `goal` | Required | One line of free text | What the page is for |
| `tools` | Required | As many as apply | Which tools you need to have |
| `sensitivity` | Required | As many as apply | What information is safe to put in |
| `status` | Required | Pick exactly one | Whether you can trust it |
| `job` | Optional | As many as apply | Who it is relevant to |
| `effort` | Optional | Pick exactly one | How long before it is useful |
| `tokens` | Optional | Pick exactly one | What it costs to run |

---

## What a tag block looks like

Every page starts with a small block of text that looks like this. This one is
filled in as a real example, so you can see the shape.

```yaml
---
title: Long document summariser
goal: understand a long document fast
tools: [claude]
sensitivity: [🟡 private-data]
status: [✅ status-active]
job: [👥 any-role]
effort: [⚡ effort-5-min]
tokens: [🪙 tokens-low]
---
```

This is called YAML front matter. GitHub displays it as a small table at the
top of your page, so readers see it without needing to know anything about the
format.

### Why the square brackets matter

The square brackets are what turn a value into a proper tag on screen.

| How you write it | How GitHub displays it |
|---|---|
| `status: [✅ status-active]` | Inside a small box, so it reads as a tag |
| `status: ✅ status-active` | As plain text, which looks like a stray note |

Please use square brackets on all five tag lines, even when you only have one
value in them. The two lines that do not take brackets are `title` and `goal`,
because those are sentences rather than tags.

### Why the emoji and the word are both there

The emoji is there so you can scan a page quickly and see what you are looking
at. The word is there because GitHub search does not reliably find emoji, so
the word is what makes your page findable.

Keep both. Write `[⚡ effort-5-min]`, not `[⚡]` and not `[effort-5-min]`.

---

## The four required tags

### `goal`

This one is free text rather than a fixed list, so there is no table of
allowed values and no brackets. Write one short line in your own words,
phrased the way you would say it out loud to a colleague.

| Write something like this | Rather than this |
|---|---|
| `turn messy notes into a spec draft` | `productivity` |
| `check a design against pattern rules` | `design stuff` |
| `find out what a long document says about my work` | `misc` |

The reason this tag is free text is that nobody on a team ever agrees on what
the categories should be, but everybody can say what they were trying to do.
Search picks up the words either way.

### `tools`

List every tool your page depends on. You can list more than one, separated by
commas inside the brackets.

| Value to copy | What it means |
|---|---|
| `claude` | Anthropic's Claude, through the web app or the desktop app |
| `copilot` | GitHub Copilot, usually inside VS Code |
| `gemini` | Gemini, including the version built into Google Workspace |
| `figma-make` | The AI features inside Figma |
| `notebooklm` | Google NotebookLM |
| `chatgpt` | OpenAI's ChatGPT |
| `no-tool` | Your page needs no AI tool at all, for example a context file template |

Written out, a page using two tools looks like this:
`tools: [claude, copilot]`

### `sensitivity`

This tells the reader what kind of information they can safely feed into the
tool.

**Green means you can put anything in. Red means be careful, because only
public information is allowed.**

| Value to copy | What it means for you |
|---|---|
| `🟢 confidential-data` | Anything goes, including personal and customer data |
| `🟡 private-data` | Internal and unreleased work is fine. No personal or customer data |
| `🔴 public-data` | Careful. Only information that is already public, or that could be |
| `🟢 confidential-code` | Anything goes, including restricted projects |
| `🟡 private-code` | Internal repositories are fine |
| `🔴 public-code` | Careful. Open source and public repositories only |

Data and code are approved separately, so list whichever values apply to your
page. A page that works on internal documents and internal repositories looks
like this:

`sensitivity: [🟡 private-data, 🟡 private-code]`

This is the one tag you should not guess at. Please check the
[tool clearance page](CLEARANCE.md) before you set it.

### `status`

Pick exactly one of these four.

| Value to copy | What it means |
|---|---|
| `✅ status-active` | This works, and somebody on the team uses it regularly |
| `🧪 status-experimental` | Somebody tried this once or twice, it is rough and may not hold up |
| `❌ status-did-not-work` | This was tried and it failed, and the page exists so nobody repeats it |
| `📦 status-archived` | This used to be useful and no longer is, kept for reference |

---

## The three optional tags

You can skip all three if you are in a hurry. They help other people filter,
but they do not block anything.

### `job`

List every job your page is relevant to, or use `any-role` if it applies to
everybody.

| Value to copy | Who it means |
|---|---|
| `🎨 visual-design` | Visual designers |
| `🧭 ux-design` | UX designers |
| `🔬 ux-research` | User researchers and user scientists |
| `✏️ content` | Content designers and writers |
| `⚙️ web-dev` | Web engineers |
| `👥 any-role` | Everybody, regardless of what they do |

This is a tag rather than a folder for a good reason. A visual designer works
at almost every stage of a project, so putting jobs into folders would hide
most of the repository from most people.

### `effort`

Pick exactly one.

| Value to copy | What it means |
|---|---|
| `⚡ effort-5-min` | You can try it right now, with nothing to set up |
| `🕐 effort-1-hour` | Worth blocking out some time for |
| `🔧 effort-setup-needed` | Something has to be installed or configured first |

### `tokens`

Everybody has a monthly budget for AI usage, and some workflows eat through it
much faster than others. Flagging this is genuinely useful to other people.

| Value to copy | What it means |
|---|---|
| `🪙 tokens-low` | Barely noticeable against your monthly budget |
| `💰 tokens-medium` | Worth being aware of if you run it repeatedly |
| `💸 tokens-high` | This will make a visible dent, so plan for it |

---

## How to search using these tags

Every word in the tables above is a search term. Search for the word, not the
emoji, because GitHub does not reliably find emoji.

Go to the top of the repository and use the box that says **Search this
repository**. Type the tag exactly as it is written here, then press enter.

| What you want | What to type |
|---|---|
| Everything relevant to visual designers | `visual-design` |
| Everything that uses Claude | `claude` |
| Quick wins you can try today | `effort-5-min` |
| Things that are safe for internal documents | `private-data` |
| Only the things people genuinely rely on | `status-active` |
| Things that failed, so you do not repeat them | `status-did-not-work` |
| Quick wins for visual designers specifically | `visual-design effort-5-min` |
| Cheap things that use Claude | `claude tokens-low` |

Searching for two tags at once narrows the results down, which is usually what
you want once the repository has more than a few pages in it.

---

## Adding a tag that does not exist yet

You are allowed to invent a tag. The only rule is that you write it down here
as well, so that it stops being private to you.

| Step | What you do |
|---|---|
| 1 | Use your new tag on your own page, with an emoji and a word |
| 2 | In the same commit, open this file and add a row to the relevant table |
| 3 | Write one short line explaining what it means |

A tag that only you know about is invisible to everybody else. A tag that
appears in one of the tables on this page is one the whole team can find.

---

## Three things worth remembering

| Remember this | Because |
|---|---|
| Four required tags is the minimum, not the target | If you only have two minutes, do those four and skip the rest |
| A wrong tag is better than a missing tag | Somebody will spot a wrong tag and correct it. A missing tag makes your page invisible forever |
| Copy the exact wording from this page | Search is literal, so `visual design` with a space will not match `visual-design` with a hyphen |

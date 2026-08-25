# What you are allowed to put into a tool

Before you paste anything into an AI tool, it is worth knowing whether that
tool has been approved for the kind of information you are about to give it.

The categories on this page come from the official company AI approval list.
This page points you at that list and explains how to read it. It does not
replace it, and if the two ever disagree, the official list is the one that
counts.

---

## How to read the colours

| Colour | What it means |
|---|---|
| 🟢 | You can put anything in, including confidential and personal information |
| 🟡 | Internal and unreleased work is fine. Nothing personal or customer related |
| 🔴 | Be careful. Only information that is already public, or that could be |

Green means you are free. Red means you have to stop and think.

---

## The questions people actually ask

Rather than starting with the categories, here are the questions that come up
most often.

| Your question | The answer |
|---|---|
| Can I paste a copy doc into a tool? | A copy doc is unreleased internal content, so the tool needs to be cleared to 🟡 for data |
| Can I paste a user interview transcript in? | A transcript usually contains personal information about a real person, so it needs 🟢 for data. Most tools do not have that |
| Can I paste in a page that is already published? | Yes. Anything already public is fine anywhere, including 🔴 tools |
| Can I point a tool at a Canonical repository? | That depends on its clearance for code, which is separate from its clearance for data. Check the code column |
| What if my tool is not in the table below? | Treat it as 🔴, meaning public information only, even on a personal account |
| What if I am still not sure? | Ask in the `ai-tooling` channel on Mattermost before you paste anything in. Nobody has ever been annoyed by this question |

---

## Data and code are two separate things

A tool can be approved for one and not the other, so it is worth checking both
if your work involves both.

**Data** means notes, documents, transcripts, and anything else that is not
code.

| Tag | What it covers |
|---|---|
| `🟢 confidential-data` | Personal data, customer data, and anything otherwise restricted |
| `🟡 private-data` | Internal work, unreleased material, anything not yet published |
| `🔴 public-data` | Information that is already public, or that would be fine if it were |

**Code** means repositories, scripts and projects.

| Tag | What it covers |
|---|---|
| `🟢 confidential-code` | Restricted projects |
| `🟡 private-code` | Internal repositories |
| `🔴 public-code` | Open source projects and public repositories |

---

## Which tools are cleared

*The table below is invented for this prototype. In a real version it would be
filled in from the official approval list.*

| Tool | Data | Code | How you get access |
|---|---|---|---|
| Gemini for Google Workspace | 🟢 | Not applicable | It is already part of your Workspace login |
| GitHub Copilot | 🟡 | 🟢 | You are enrolled through the Canonical GitHub organisation. It is not self serve |
| Any other chatbot | 🔴 | 🔴 | This is the default policy for anything not separately approved |

The colour in each cell is the highest level that tool has been approved for.
A tool marked 🟡 for data is also fine for anything below that, so private and
public are both allowed, but confidential is not.

GitHub Copilot is the clearest example of why the two columns matter. It is
🟢 for code, so pointing it at an internal repository is fine. It is only 🟡
for data, so pasting meeting notes into it is not.

---

**Last checked:** August 2026.

Approvals change over time. If this page looks out of date, please flag it in
the `ai-tooling` channel rather than relying on it.

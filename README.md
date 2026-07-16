# first-intern 🎯

**The playbook I used to land my first internship — no connections, no experience, no prestige. Now packaged as a skill for Claude.**

Three things got me hired: a ruthlessly concise resume, a high-volume application system, and cold emails sent straight to startup founders. My boss later told me why I got picked out of the pile: *my information was concise and my writing was sharp.* That's not a talent — it's a method, and this skill teaches it to Claude so Claude can coach you through it.

English is the skill's native language — every template and example is written the way a founder actually reads. [中文版说明 →](README.zh.md)

---

## Table of contents

- [What it does](#what-it-does)
- [Installation](#installation)
  - [Claude Code (recommended)](#claude-code-recommended)
  - [Claude.ai / Claude Desktop](#claudeai--claude-desktop)
  - [Verify it's working](#verify-its-working)
- [How to use it](#how-to-use-it)
  - [Workflow 1 — Fix your resume](#workflow-1--fix-your-resume)
  - [Workflow 2 — Build your application system](#workflow-2--build-your-application-system)
  - [Workflow 3 — Cold email a founder](#workflow-3--cold-email-a-founder)
  - [Full engagement — "help me find an internship"](#full-engagement--help-me-find-an-internship)
- [Where the resume method comes from](#where-the-resume-method-comes-from)
- [What Claude will refuse to do](#what-claude-will-refuse-to-do)
- [Language](#language)
- [Repository structure](#repository-structure)
- [Why this works](#why-this-works)
- [FAQ](#faq)
- [Contributing](#contributing)
- [License](#license)

---

## What it does

Tell Claude you're looking for your first internship, and it will:

1. **Rewrite your resume** — one page, every bullet in Context–Action–Result form, zero filler. Includes the "6-second test" a screener actually applies to your resume.
2. **Build your application system** — a tracker, a daily quota computed from your deadline, tiered targets, and weekly funnel reviews so silence becomes data instead of despair.
3. **Write founder cold emails** — two field-tested templates (a ~60-word minimal one and a ≤120-word hook one), one small ask, and pre-scheduled follow-ups. This is the highest-conversion channel nobody teaches students.

Built-in honesty guardrail: it will sharpen what's real, never invent what isn't.

## Installation

A skill is just a folder of Markdown files that Claude reads when the topic comes up. Installing means putting this folder where Claude looks for skills.

### Claude Code (recommended)

**Option A — personal skill (available in every project):**

```bash
git clone https://github.com/jo1-yo/first-intern.git ~/.claude/skills/first-intern
```

**Option B — project skill (available only inside one project, shareable with teammates via git):**

```bash
git clone https://github.com/jo1-yo/first-intern.git .claude/skills/first-intern
```

That's the whole installation. No build step, no dependencies, no configuration. To update later, run `git pull` inside the folder. To uninstall, delete the folder.

### Claude.ai / Claude Desktop

Claude.ai accepts skills as an uploaded zip file:

1. Download this repo as a zip (green **Code** button → **Download ZIP**), or build one yourself:
   ```bash
   git clone https://github.com/jo1-yo/first-intern.git
   cd first-intern && zip -r first-intern.zip . -x ".git/*"
   ```
2. In Claude.ai or the desktop app, open **Settings → Capabilities → Skills** (naming may vary slightly by plan).
3. Upload the zip. The skill activates automatically in new conversations.

### Verify it's working

Start a new conversation and say something like *"I need help finding my first internship."* If the skill is installed, Claude's answer will follow this playbook's flow — it will **ask for your resume before giving any advice** (that's the skill's signature move), instead of dumping generic tips. In Claude Code you can also just check that the folder exists at `~/.claude/skills/first-intern/SKILL.md`.

## How to use it

You don't invoke this skill with a command — it triggers automatically whenever your conversation touches internships, job hunting, resumes, CVs, cover letters, cold emails, or "no one is replying to my applications." Just talk to Claude normally.

You can start from any of the three workflows, or hand Claude the whole problem. Here's what each one looks like in practice.

### Workflow 1 — Fix your resume

The resume methodology isn't invented — it's distilled from **Stanford Career Education's** published resume resources (see [Where the resume method comes from](#where-the-resume-method-comes-from)).

**Say something like:**

> *"I've sent 40 internship applications and gotten zero replies. Here's my resume: [paste it, or attach the PDF/DOCX]"*

> *"Can you review my resume? I'm targeting marketing internships."*

> *"I don't have a resume yet and I have no idea what to put on one."*

**What Claude will do:**

1. **Extract before advising.** It first parses your resume into a structured inventory (education, every experience, every bullet scored against Context–Action–Result) and shows it back to you, so you can correct it before anything gets rewritten. No generic tips from a skim.
2. **Diagnose.** It names your single strongest piece of evidence, one primary target role plus up to two adjacent ones, the three biggest barriers, and the three highest-impact fixes — no fake scores like "7/10."
3. **Rewrite bullet by bullet**, showing `before → after`, hunting for numbers you forgot you had ("How many people used it? What happened because of it?").
4. **Run the 6-second test** — reading only your name, headings, and first bullets, can a screener tell what role you want and what's most impressive about you?
5. **Deliver a clean, copy-pasteable one-page resume** and recommend pasting it into your school's official career-center template.

**Tips for best results:**
- Paste the real resume, not a description of it. Redacting your name and contact info is fine.
- Tell Claude your target role — nothing can be judged without it.
- If you think you "have no experience," say so — the skill mines coursework, class projects, part-time jobs, clubs, volunteering, and hackathons before agreeing your resume is thin. If a real gap exists, it prescribes a small 7–14 day project that produces a public artifact instead of padding.

### Workflow 2 — Build your application system

**Say something like:**

> *"My resume is ready. Now what? I need an internship by June."*

> *"I've applied to 60 places and heard nothing. Is it me or is it normal?"*

**What Claude will do:**

1. **Build you a tracker** from [assets/tracker-template.csv](assets/tracker-template.csv), pre-filled with real starter rows — not an empty template.
2. **Tier your targets:** A (dream companies — full tailoring + a cold email to a human), B (solid fits — keyword pass), C (volume — apply fast, don't overthink).
3. **Compute your daily quota from your deadline.** Example: an offer needed in 8 weeks ≈ 100–150 applications + 20–30 cold emails ≈ ~3 applications and ~0.5 cold emails per day. Seeing the math makes it feel doable.
4. **Point you beyond the big job boards** — university portals, startup boards (Work at a Startup, Wellfound), "we're hiring" posts, and founder cold email.
5. **Read your funnel every ~25 applications:** zero replies → the resume is the leak; replies but no interviews → your short answers are the leak; interviews but no offers → shift to interview practice. Fix the leak, not everything.

If Claude has web access, it will also build a verified shortlist of 10–15 currently-open roles with official links — and it will never invent a listing, deadline, or recruiter.

### Workflow 3 — Cold email a founder

**Say something like:**

> *"I want to intern at [startup I love]. I've never written a cold email — help."*

> *"Can you write an email to the founder of X? Here's my background: ..."*

**What Claude will do:**

1. **Help pick the right recipient** — the founder at a small startup, an alum or team member at a bigger company, the professor for a research role.
2. **Pick a template based on what you actually have:**
   - **Template A — the minimal fit email (~60 words).** The exact structure that landed the author her internship. Fit line → one warm sentence of genuine interest → availability + a friction remover → zero-pressure ask. Use it when your background obviously maps onto what the company does.
   - **Template B — the hook email (≤120 words).** For when you have a concrete proof point (a project, an audience, a number). Hook only *that* company could receive → one proof point → why them → one small ask.
3. **Annotate the draft the first time** — one line per sentence explaining why it's there, so you learn the formula instead of depending on it.
4. **Pre-write both follow-ups with send dates** (day 3–4 with one new piece of information; day 8–10 warm close; then stop forever). A large share of replies come from follow-ups that actually get sent.
5. **Refuse the mail-merge shortcut.** If you're emailing five companies, you get five separately written emails — a hook that could be sent to any company is not a hook.

There's also a LinkedIn-DM variant (≤300 characters) for when the channel is LinkedIn instead of email.

### Full engagement — "help me find an internship"

**Say something like:**

> *"I need a summer internship in 2 months and I have no resume and no idea where to start."*

Claude runs all three workflows as one plan: gets your resume (or builds one from scratch) → diagnoses → delivers, in order: best internship directions with evidence-based reasoning → resume rewrite → a live-openings shortlist → one personalized cold email + LinkedIn message → **exactly three prioritized next actions** with deadlines. Never a sprawling checklist.

## Where the resume method comes from

The resume workflow is not folk advice — it's a distillation of the resume guidance published by **[Stanford Career Education](https://careered.stanford.edu/resources)** (Stanford's career center), condensed into rules Claude can apply directly. The mapping:

| In this skill | Stanford Career Education resource (under **Resources → Resume**) |
|---|---|
| C-A-R bullets (Context–Action–Result) | *CAR Method for Developing Resume Content* |
| The action-verb lists and the "verbs to kill" | *Action Verb List* |
| "What counts as experience" (part-time jobs, clubs, course projects, volunteering…) | *What Kind of "Opportunities" Count as Experience on your Resume* |
| One-page rules, formatting, structure | *Steps to Writing Your Resume* |
| The automated first screen (ATS) and why concision survives it | *ATS Resume* |
| The dedicated QA pass | *Resume Review Checklist* |
| "Use your school's career-center template" | *Resume Samples and Templates* |

If you're a Stanford student, use the originals — they're free at the link above. What this skill adds is the operationalization: the Step-0 extraction, the 6-second test, the before→after rewrites, and the honesty guardrails, applied to *your* actual resume in conversation.

> This is an independent project by a student who used these resources. It is **not affiliated with or endorsed by Stanford University**.

## What Claude will refuse to do

The skill has a hard honesty guardrail, because the method only works when everything in your materials is true and verifiable:

- ❌ Invent experience, inflate numbers, or turn a class project into a "production system"
- ❌ Fabricate job listings, deadlines, recruiters, or contact emails
- ❌ Write fake personalization or mail-merged flattery
- ❌ Pad your resume with adjectives and soft-skill lists

When your material is thin, it sharpens what's real or helps you quickly *create* something real — never embellishes.

## Language

The skill is **English-native**: all templates, examples, and produced materials (resumes, emails) are idiomatic English, written the way a founder or recruiter actually reads. You can chat with Claude in any language — deliverables stay in English unless your target market genuinely uses another language, in which case Claude adapts the tone but keeps the structure.

## Repository structure

```
first-intern/
├── SKILL.md                      # Entry point: the method, operating rules, and flow Claude follows
├── references/
│   ├── resume.md                 # Concise resume rewriting: Step-0 extraction, C-A-R bullets, 6-second test
│   ├── mass-apply.md             # The volume system: tracker, tiers, daily quota, funnel reviews
│   ├── cold-email.md             # Founder cold email: Templates A & B, follow-ups, full examples
│   └── action-verbs.md           # Action verbs by category + the verbs to kill on sight
├── assets/
│   └── tracker-template.csv      # Application tracker starter file
├── evals/
│   └── evals.json                # Test scenarios used to validate the skill's behavior
├── README.md                     # You are here
└── README.zh.md                  # 中文说明
```

Claude reads `SKILL.md` when the topic triggers, then loads only the reference file relevant to your ask — so a single-email request doesn't drag in the whole playbook.

## Why this works

The first job search is a funnel: **replies = quality × volume × channel.** Most students lose on all three — a padded resume, ten applications, all on big job boards. This skill fixes the resume with concision (a recruiter gives you ~6 seconds), fixes volume with a system (100 applications is normal, not failure), and fixes channel with founder cold email (small startups rarely post intern roles — the intern who shows up in the inbox is the one who gets hired).

## FAQ

**Do I need to know how to code to use this?**
No. Installing is one `git clone` (or a zip upload on Claude.ai), and using it is just talking to Claude.

**Does it work for first jobs, not just internships?**
Yes — the method is the same funnel. The skill optimizes for a *first* role of any kind, where you have no track record to lean on.

**I'm not in the US. Does it still apply?**
The resume and volume principles are universal. The cold-email norms assume English-speaking startup culture (direct, informal, brief); the skill adapts tone for markets with different norms (e.g., formal salutations in Japan or Germany) while keeping the structure.

**Will it apply to jobs for me?**
No — it builds the materials and the system; you press send. It also never claims a job list is exhaustive.

**Can it guarantee replies?**
No, and be suspicious of anything that says it can. First-internship reply rates run 1–5% even with strong materials. What the skill guarantees is that you stop losing for fixable reasons.

## Contributing

PRs welcome — especially real before/after examples (anonymized) and market-specific norms (cold-email conventions differ by country). Keep contributions consistent with the concise bar: if deleting a sentence loses nothing, delete it.

## License

MIT — see [LICENSE](LICENSE).

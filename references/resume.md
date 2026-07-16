# The Concise Resume

A resume's job is not to describe the user — it's to earn a conversation. A screener gives it about 6 seconds on first pass, and increasingly the first screen is an AI/ATS pass before any human sees it. Every line either moves toward "let's talk to this person" or gets cut.

## Step 0 — Extract before advising (mandatory)

Never give resume advice from a skim. First parse the resume into a structured inventory and show it back to the user. Extract **only what the resume explicitly supports** — university, degree and major, expected graduation, relevant coursework, skills and tools, projects, research, employment, leadership and extracurriculars, awards, location, portfolio/GitHub/LinkedIn links, and work authorization only if explicitly stated (never assumed):

- **Target role(s)** the resume is aiming at (ask if unknown — nothing else can be judged without this).
- **For each experience**: organization, role, dates, links, and each bullet scored against C-A-R (does it have Context? an Action verb? a Result or number?) with what's missing named specifically.
- **Format facts**: page count, headings used, bullet counts per item, where links live, font/margins if detectable.

Every recommendation after this point must reference a specific line of *their* resume. If a suggestion could be pasted into a review of anyone's resume, it's filler — cut it. The extraction is also what earns the user's trust: they can see you actually read it, and they can correct you before you rewrite.

## The diagnosis

From the extraction, identify and state:

1. **The strongest evidence of ability** — the single most credible, concrete thing on the page.
2. **One primary internship target** and **up to two adjacent targets** where the current evidence is strongest, each justified in one sentence citing the resume. Adjacent targets matter: a student aiming at data science whose real evidence is web projects should hear that plainly.
3. **The three biggest barriers** preventing interviews right now.
4. **The three highest-impact improvements** — not ten. Prioritization is the value.

No arbitrary scores ("7/10") — they sound precise and mean nothing. Diagnose specifics.

**What counts as strong evidence** for a first-time intern:
- A project with a real user, real technical difficulty, an original insight, a measurable result, or a public artifact (repo, demo, published piece) — these are worth more than any adjective.
- Part-time and service jobs, when they show responsibility, customer communication, operations, or reliability.
- Club leadership, only when concrete actions and outcomes can be named.
- Independently extending coursework beyond the assignment — distinguish this clearly from just completing the class.

**The proof-of-work rule:** when the user lacks evidence for the role they want, prescribe one small project completable in 7–14 days that produces a public artifact (a deployed demo, a published analysis, three spec pieces for a real company). They keep applying while building it — the project fills the gap; it doesn't excuse a pause.

## What counts as experience

Beginners conclude "I have nothing" because they think only internships count. Career centers (Stanford's, notably) count far more — mine ALL of these before agreeing a resume is thin:

internships · micro-internships and short project-based work · part-time jobs (on- or off-campus — retail counts) · research with a faculty member · volunteer work · course projects, papers, and labs · professional-development courses and certifications · clubs (member or leader) · athletics · community or religious involvement · startup work or a business the user launched · independent projects (built a PC, wrote a play, taught themselves a language) · military service.

## The rules

1. **One page.** If it doesn't fit, the problem is selection, not font size.

2. **Use the school's career-center template** when one exists — tested formatting, correct indentation, no layout surprises. Otherwise: 10–12pt readable font (Times New Roman at 10.5+, Calibri, Cambria, Garamond, Helvetica, Arial), 0.75–1.0" margins (0.5" top/bottom acceptable), single column, no tables, graphics, or photo (photo norms vary by country — none for US/UK).

3. **Descriptive headings beat generic ones.** "Research Experience", "Programming Experience", "Design Experience", "Leadership and Teamwork", "Marketing Experience" tell a skimming screener the resume's shape from headings alone; "Experience" and "Other" tell them nothing. Mix descriptive and general headings as the material demands.

4. **C-A-R bullets** (Context–Action–Result — the framework university career centers teach, Stanford's included):
   - **Context**: what the task/project was, who it was with or for.
   - **Action**: what the user did, in active verbs (see [action-verbs.md](action-verbs.md)).
   - **Result**: quantified whenever possible. If the outcome isn't known yet (ongoing work), state the *purpose* — why the work matters — instead of leaving the bullet hanging.
   - If no number exists, hunt for a proxy: users, downloads, followers, participants, pieces produced, hours saved, money raised, % change. Or name and link the artifact — a clickable thing beats an adjective.

5. **2–3 bullets per item, similar length.** Even bullet lengths make the page look designed; one 3-line mega-bullet next to a 1-liner looks unedited. Split overloaded bullets, merge trivial ones. 3 bullets max for the most relevant item, 1–2 for the rest.

6. **Links woven into the text, placed consistently.** Hyperlink the words themselves (the project name, "demo", the org), and put links in the same position everywhere — e.g., always at the end of the title line, or always closing the first bullet. Header links (portfolio, GitHub, LinkedIn) only if they're worth clicking.

7. **Vertical focus: one resume, one target.** If the user's material spans multiple directions (SWE + data science, design + marketing), build separate versions — each leading with the relevant experience, headings, and keywords. One resume trying to do three jobs does none of them. Offer to generate the variants; the base inventory from Step 0 makes this cheap.

8. **Zero mechanical errors.** Run multiple explicit proofing passes — spelling, verb tense (past roles in past tense, current in present), punctuation consistency at bullet ends, date-format consistency, en-dashes vs hyphens, indentation. The first screen is often automated; a grammar error is the cheapest possible way to fail it. Do a final dedicated QA pass separate from the content pass.

9. **Emphasis guides the eye.** Bold or italicize what the reader should notice immediately — organization name and/or title. Never bold city, state, or dates.

10. **The cut list** — delete on sight: "Responsible for...", "Helped with...", "Participated in...", "Assisted in...", "Passionate about...", every self-describing adjective, objective/summary statements (a summary earns its place only when it adds context the resume can't show — never by default), "References available upon request", soft-skill lists ("teamwork, communication, leadership" — these get *shown* through C-A-R bullets, never listed).

11. **Tailoring**: mirror the top ~5 nouns of the job description wherever truthfully possible (their words: "data pipeline" not "data flow"). Never claim a skill the user doesn't have.

12. **Truthful labels.** School projects are projects, not employment — never inflate a class project into a production system or a title. Keep high-school experience for a first-year student when it's still the strongest material; retire it as university experience overtakes it. Placeholders for unknown numbers stay visibly placeholders: "[add # of users if known]", never a plausible-looking guess.

## The 6-second test

Simulate the screener: read only the name, section headings, and the first bullet of each section, in 6 seconds. Then answer:

- What role is this person applying for?
- What is the single most impressive concrete thing about them?

If either answer is fuzzy, restructure — usually by promoting the strongest bullet to first position in its item (the 6-second skim only reads first bullets), or by moving the strongest section up.

## How to run a resume session

1. Get the current resume (or raw-material inventory) and the target role(s).
2. **Step 0 extraction** — show the structured inventory, let the user correct it.
3. **Diagnose before editing**: the 6-second-test read, citing their actual lines.
4. Rewrite bullet by bullet, showing `before → after` in C-A-R form. Explain a principle the first time it applies, then just apply it.
5. **Interview for numbers.** Users almost always have quantifiable outcomes they never thought to mention: "How many people used it? How often? Compared to what? What happened because of it?"
6. If the material spans multiple directions, propose vertical variants and build them from the same inventory.
7. **Dedicated QA pass**: grammar, tense, punctuation, date formats, link placement consistency, bullet-length balance.
8. Deliver the full rewritten resume as a clean copy-pasteable document — and recommend pasting it into the school's official template.

## Before → after examples

**Filler to C-A-R:**
- ✗ "Assisted with fundraising event"
- ✓ "Collaborated with a team of 6 student leaders to plan and run a fundraising event, raising $5,000 for research on heart disease in women" *(C: team/event · A: plan and run · R: $5,000)*

**Vague group work to owned scope:**
- ✗ "Worked on a group project building a website"
- ✓ "Built the checkout flow for a 4-person class project (React, Stripe test mode); demoed to 30 classmates"

**Adjective to artifact:**
- ✗ "Passionate about data analysis, familiar with Excel"
- ✓ "Analyzed 2 years of café sales in Excel and recommended cutting 3 menu items; owner adopted 2"

**Ongoing work — purpose in place of a result:**
- ✗ "Currently developing a mobile app"
- ✓ "Developing an ARKit navigation-training app to study how spatial reasoning changes with practice, for a lab study launching in the fall"

**Title inflation to honest impact:**
- ✗ "Vice President of Marketing, Student Business Association"
- ✓ "Ran sponsor outreach for a 200-person student conference; closed 4 sponsors totaling $3,000"

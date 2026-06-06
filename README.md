# Apply Within — a Claude skill for job seekers

A free, open-source [Claude](https://claude.com/claude-code) skill that turns
Laszlo Bock's **"Apply Within"** playbook into an interactive job-search coach.

Laszlo Bock was SVP of People Operations at Google — his team sifted 30M+ resumes.
He released a free 112-page playbook for job seekers. This repo encodes its
methodology into a skill so Claude can coach you through it: the X/Y/Z resume
formula, cover letters, networking for referrals, interview prep, applying, and
salary negotiation.

> Unofficial study aid. All credit for the methodology belongs to Laszlo Bock.

## Install — Claude app (easiest, no code)

Works in the Claude desktop app and on claude.ai (paid plans):

1. Open the **Customize** menu in the left sidebar → **Plugins** tab
2. In the **Personal plugins** section, click **+** → **Add marketplace**
3. Choose **Add from a repository** and paste:
   `https://github.com/tomitomahto/apply-within`
4. Sync, then click **Install** on **apply-within**

That's it. Start a new chat and talk to Claude about your job search:

```
Help me rewrite my resume bullets
Run me through a mock interview for a product manager role
Help me negotiate this offer
```

The skill loads automatically when your message is about job searching.

## Install — ZIP upload (no GitHub account needed)

1. Click the green **Code** button above → **Download ZIP**, and unzip it
2. Zip just the inner `apply-within/skills/apply-within` folder (the one
   containing `SKILL.md`)
3. In Claude: **Customize → Skills → + → Upload skill** → drag your zip in

## Install — Claude Code (terminal)

Run these two commands in your terminal:

```bash
claude plugin marketplace add tomitomahto/apply-within
claude plugin install apply-within@apply-within
```

Or copy the skill folder manually:

```bash
git clone https://github.com/tomitomahto/apply-within.git
cp -r apply-within/apply-within/skills/apply-within ~/.claude/skills/
```

## What's inside

```
apply-within/                  (repo = marketplace)
├── .claude-plugin/
│   └── marketplace.json
└── apply-within/              (the plugin)
    ├── .claude-plugin/
    │   └── plugin.json
    └── skills/
        └── apply-within/      (the skill)
            ├── SKILL.md
            └── references/
                ├── 01-resume.md
                ├── 02-cover-letter.md
                ├── 03-networking.md
                ├── 04-interview.md
                └── 05-apply-negotiate.md
```

## License

MIT. See [LICENSE](LICENSE).

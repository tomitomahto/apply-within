# Apply Within — a Claude skill for job seekers

A free, open-source [Claude](https://claude.com/claude-code) skill that turns
Laszlo Bock's **"Apply Within"** playbook into an interactive job-search coach.

Laszlo Bock was SVP of People Operations at Google — his team sifted 30M+ resumes.
He released a free 112-page playbook for job seekers. This repo encodes its
methodology into a skill so Claude can coach you through it: the X/Y/Z resume
formula, cover letters, networking for referrals, interview prep, applying, and
salary negotiation.

> Unofficial study aid. All credit for the methodology belongs to Laszlo Bock.

## Install (recommended — plugin marketplace)

In Claude Code, run:

```
/plugin marketplace add tomitomahto/apply-within
/plugin install apply-within@apply-within
```

That's it. Now just talk to Claude about your job search:

```
Help me rewrite my resume bullets
Run me through a mock interview for a product manager role
Help me negotiate this offer
```

The skill loads automatically when your message is about job searching.

## Install (manual — copy the skill folder)

Prefer not to use plugins? Copy the skill straight into your skills directory:

```bash
git clone https://github.com/tomitomahto/apply-within.git
cp -r apply-within/skills/apply-within ~/.claude/skills/
```

(For a single project instead of globally, copy it into `.claude/skills/` inside
that project.)

## What's inside

```
apply-within/
├── .claude-plugin/
│   ├── marketplace.json
│   └── plugin.json
└── skills/
    └── apply-within/
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

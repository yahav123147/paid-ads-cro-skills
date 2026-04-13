# Paid Ads & CRO Skills for Claude Code

A collection of Claude Code skills for paid advertising, conversion rate optimization (CRO), and marketing psychology.

These skills are designed to work with [Claude Code](https://claude.ai/claude-code) and can be installed as custom skills.

## Skills Included

### Paid Advertising & Copywriting

| Skill | Description |
|-------|-------------|
| **ad-copywriter** | Write high-converting Facebook & Instagram ads in Hebrew. 19 ad types, 7 hook patterns, 12 templates, 10 headline formulas |
| **email-copywriting** | 8-part email copywriting formula. Hook, open loop, lead, value, coin drop, editing pass, CTA, P.S. |
| **marketing-psychology** | 70+ mental models for marketing. Pricing psychology, persuasion, buyer behavior, growth models |
| **marketing-ideas** | 139 proven marketing ideas organized by category, stage, budget, and timeline |

### Conversion Rate Optimization (CRO)

| Skill | Description |
|-------|-------------|
| **page-cro** | Page conversion optimization. Value proposition, headlines, CTAs, trust signals, objection handling |
| **form-cro** | Form optimization. Field-by-field guidance, multi-step forms, error handling, mobile optimization |
| **signup-flow-cro** | Signup & registration flow optimization. Single vs multi-step, social auth, progressive commitment |
| **onboarding-cro** | Post-signup onboarding & activation. Aha moment, checklists, empty states, multi-channel |
| **popup-cro** | Popup & modal optimization. Trigger strategies, exit intent, frequency capping, compliance |

### Design

| Skill | Description |
|-------|-------------|
| **landing-page-design** | Landing page layout rules. Above-the-fold formula, section order, CTA design, mobile optimization |

## Installation

### Option 1: Copy individual skills

Copy any skill folder into your project's `.claude/skills/` directory:

```bash
cp -r skills/ad-copywriter /path/to/your/project/.claude/skills/
```

### Option 2: Symlink to global skills

```bash
# Link all skills
for skill in skills/*/; do
  ln -s "$(pwd)/$skill" ~/.claude/skills/$(basename "$skill")
done
```

### Option 3: Clone and reference

```bash
git clone https://github.com/YOUR_USERNAME/paid-ads-cro-skills.git
```

Then add to your project's `.claude/CLAUDE.md`:

```markdown
Skills are available at /path/to/paid-ads-cro-skills/skills/
```

## Usage

Once installed, Claude Code will automatically activate the relevant skill based on your request:

- "Write me a Facebook ad for my product" -> `ad-copywriter`
- "Optimize this landing page for conversions" -> `page-cro`
- "Why isn't my signup form converting?" -> `form-cro`
- "Apply psychology to my pricing page" -> `marketing-psychology`
- "Give me marketing ideas for my SaaS" -> `marketing-ideas`

## Structure

```
skills/
  ad-copywriter/
    SKILL.md
  email-copywriting/
    SKILL.md
  form-cro/
    SKILL.md
  landing-page-design/
    SKILL.md
  marketing-ideas/
    SKILL.md
    references/
      ideas-by-category.md      # 139 marketing ideas
  marketing-psychology/
    SKILL.md
  onboarding-cro/
    SKILL.md
    references/
      experiments.md            # Onboarding A/B test ideas
  page-cro/
    SKILL.md
    references/
      experiments.md            # Page CRO experiment ideas
  popup-cro/
    SKILL.md
  signup-flow-cro/
    SKILL.md
```

## License

MIT

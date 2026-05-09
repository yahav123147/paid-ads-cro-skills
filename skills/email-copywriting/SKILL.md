# email-copywriting (deprecated)

> **This skill has been deprecated.** It has been replaced by
> [`yahav-writing-style`](../yahav-writing-style/SKILL.md), which teaches the same
> 8-part email methodology in Hebrew with deeper guidance:
> 38 techniques, 5 archetypes, 4 hook types, 5 P.S. types.

## To migrate

Uninstall this skill and install `yahav-writing-style` instead:

```bash
# Remove the old skill
rm -rf ~/.claude/skills/email-copywriting

# Install the replacement
curl -sL https://github.com/yahav123147/paid-ads-cro-skills/archive/main.tar.gz \
  | tar -xz -C /tmp \
  && cp -r /tmp/paid-ads-cro-skills-main/skills/yahav-writing-style ~/.claude/skills/ \
  && rm -rf /tmp/paid-ads-cro-skills-main
```

After that, every prompt that used to trigger `email-copywriting`
(write an email, rewrite this as an email, email copy) will trigger
`yahav-writing-style` automatically.

## Why the change

The old skill was a 171-line generic copy formula written in English with
American examples. The new skill is the full Hebrew methodology used by
the workshop, structured for direct application by Hebrew-speaking
business owners.

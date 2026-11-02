# agency-skill

A Claude Code plugin that runs a small AI automation agency as five agents:

- **outbound**: writes a personal first email to every business in a leads file
- **sales**: preps your calls and coaches you live from a transcript
- **build**: writes the proposal, then builds the automation
- **support**: answers client emails
- **night**: works through the queue while your computer stays on

Everything is stored in `.agency/` in the folder where you run it.

## Install

```
/plugin marketplace add <github-user>/agency-skill
/plugin install agency-skill@agency-skill
```

Restart Claude Code if the skill does not show up right away.

## Use

```
/agency-skill:agency setup
/agency-skill:agency outbound leads.csv
/agency-skill:agency sales prep <client>
/agency-skill:agency sales live <transcript file>
/agency-skill:agency build <client>
/agency-skill:agency support
/agency-skill:agency night
/agency-skill:agency status
```

Claude also picks the skill on its own when you ask for help with outreach, sales calls, proposals or client emails.

## Local test

```
claude --plugin-dir ./agency-skill
```

## License

MIT. Skill by Alex Chen (@nocodealex), https://chen.media.

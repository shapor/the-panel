# The Panel

Simulate the full [Skillathon 2026](https://luma.com/1khurilu) judge panel using Claude Code. [View the presentation](https://shapor.github.io/the-panel/presentation.html).

Paste in any submission — pitch transcript, code, skills, screenshots, whatever — and get scored by 7 AI personas modeled after the real hackathon speakers, organizers, and judges.

## What is Skillathon?

[Skillathon](https://www.skillathon.ai/) is the first Agent Skills Hackathon, organized by [BenchFlow](https://www.skillsbench.ai/) (creators of [SkillsBench](https://arxiv.org/abs/2602.12670)) and [Sundial](https://www.sundialhub.com/) (the largest agent skill registry). Participants create agent skills, design benchmark tasks, and prove that skills make agents better — backed by data from 7,308 agent runs across 84 tasks and 11 domains.

**Event**: March 7, 2026 at [Founders Inc](https://founders.inc/), San Francisco

## Usage

```bash
git clone https://github.com/shapor/the-panel
cd the-panel
claude
```

Then just paste in what you want judged. Transcripts, repos, recordings, raw ideas — anything goes.

## The Panel

All personas are based on real people associated with Skillathon 2026 — organizers, speakers, and judges.

| Persona | Role | Org | Evaluates |
|---------|------|-----|-----------|
| Xiangyi Li | Organizer | BenchFlow / SkillsBench | Skill delta, domain impact, methodology |
| Belinda Mo | Organizer | Sundial | Reusability, ecosystem fit, community value |
| Roey Ben Chaim | Organizer | Zenity | Security, anti-cheating, governance |
| Grace Zhang | Organizer | World Intelligence | Physical world relevance, data infrastructure |
| Furqan Rydhan | Speaker / Host | Founders Inc / AppLovin | Product potential, ambition, autonomy |
| Bence Nagy | Speaker | Anthropic | Skill architecture, code quality, verification |
| Ryan Marten | Speaker | Harbor / Terminal-Bench | Task difficulty, realism, reproducibility |

Each persona has a detailed background, weighted scoring rubric, and characteristic evaluation style drawn from their public work, talks, and writings.

## Output

A panel scorecard with:
- Individual scores (1-5) from each judge with praise and concerns
- Consensus strengths and risks
- Top improvements to make
- Win probability assessment

## How it works

The skills live in `.claude/skills/` so Claude Code loads them automatically. The `CLAUDE.md` tells the agent to run the full panel when you share content. No setup, no config, no dependencies.

You can also open `presentation.html` in a browser for a visual overview.

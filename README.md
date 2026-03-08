# The Panel

Simulate a full hackathon judge panel using Claude Code. Paste in any submission — pitch transcript, code, skills, screenshots, whatever — and get scored by 7 AI personas modeled after real Skillathon 2026 judges.

## Usage

```bash
git clone https://github.com/shapor/the-panel
cd the-panel
claude
```

Then just paste in what you want judged. Transcripts, repos, recordings, raw ideas — anything goes.

## The Judges

| Judge | Org | Evaluates |
|-------|-----|-----------|
| Furqan Rydhan | Founders Inc / AppLovin | Product potential, ambition, autonomy |
| Bence Nagy | Anthropic | Skill architecture, code quality, verification |
| Ryan Marten | Harbor / Terminal-Bench | Task difficulty, realism, reproducibility |
| Xiangyi Li | BenchFlow / SkillsBench | Skill delta, domain impact, methodology |
| Belinda Mo | Sundial | Reusability, ecosystem fit, community value |
| Roey Ben Chaim | Zenity | Security, anti-cheating, governance |
| Grace Zhang | World Intelligence | Physical world relevance, data infrastructure |

Each persona has a detailed background, weighted scoring rubric, and characteristic evaluation style drawn from their public work, talks, and writings.

## Output

A panel scorecard with:
- Individual scores (1-5) from each judge with praise and concerns
- Consensus strengths and risks
- Top improvements to make
- Win probability assessment

## How it works

The skills live in `.claude/skills/` so Claude Code loads them automatically. The `CLAUDE.md` tells the agent to run the full panel when you share content. No setup, no config, no dependencies.

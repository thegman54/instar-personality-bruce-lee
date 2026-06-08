# instar-personality-bruce-lee

A comprehensive personality profile for [Project Instar](https://github.com/thegman54/project-instar) that enables a bot to communicate in the voice and style of Bruce Lee.

## Architecture

This personality engine uses **18 trait categories** across **6 layers**, backed by **4 database tables** for different types of personality data:

### Layers

| Layer | Name | Categories | Purpose |
|-------|------|------------|---------|
| 1 | **Foundation** | identity, values, worldview | Core beliefs — always active |
| 2 | **Expression** | voice, lexicon, tone, emphasis, humor | Shapes every response |
| 3 | **Strategy** | rhetoric, social, narrative, authority, deflection | How interactions are conducted |
| 4 | **Reactive** | reaction, situational | Triggered by conversational context |
| 5 | **Reference** | signature, quote | Catchphrases and actual quotes |
| 6 | **Constraints** | boundary | Guardrails and limits |

### Data Stores

| Table | Purpose |
|-------|---------|
| `personality_bruce_lee_traits` | 18-category behavioral traits with examples and anti-examples |
| `personality_bruce_lee_quotes` | Actual quotes with source attribution and usage context |
| `personality_bruce_lee_lexicon` | Vocabulary fingerprint — words to favor, avoid, and use situationally |
| `personality_bruce_lee_reactions` | Trigger-to-response pattern mappings by context |

## Installation

This is a skill package for Project Instar. Upload it via the Admin UI or place it in the skills directory.

```bash
# Clone
git clone https://github.com/thegman54/instar-personality-bruce-lee.git

# Import seed data via admin panel YAML import
# or load directly into the database
```

## Tools

| Tool | Purpose |
|------|---------|
| `personality_bruce_lee_read` | Load traits, quotes, lexicon, and reactions by category and situation |
| `personality_bruce_lee_list` | List available categories, counts, and data store stats |

## Seed Data

`data/bruce_lee_profile.yaml` contains a comprehensive starter profile with:
- 55+ traits across all 18 categories
- 16 actual quotes with source attribution and usage context
- 40+ lexicon entries (favored words, avoided words, signatures, dismissals)
- 14 reaction patterns covering criticism, praise, challenges, teaching, media, and more

## License

MIT

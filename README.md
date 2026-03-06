# Scientific Skills

Natural language scientific tooling skills.

## Available Skills

| Skill | Purpose | Data |
|-------|---------|------|
| `ccf-rank` | Query CCF conference/journal rank (`A/B/C`) and type (`conference`/`journal`) | CCF catalog |

## Installation

### Via skills.sh (Recommended)

Install this repository (all included skills):

```bash
npx skills i DURUII/scientific-skills
```

Install one specific skill only:

```bash
npx skills add https://github.com/DURUII/scientific-skills --skill ccf-rank
```

### Via Claude Plugin

Install repo as a plugin:

```bash
/plugin install DURUII/scientific-skills
```

Install only one skill directory (if your client supports path-based install):

```bash
/plugin install DURUII/scientific-skills/skills/ccf-rank
```

### Manual Installation

Clone locally and add as local plugin:

```bash
cd ~/dev
git clone https://github.com/DURUII/scientific-skills.git
/plugin add ~/dev/scientific-skills
```

Manual local usage without plugin install:

```bash
cd ~/dev/scientific-skills/skills/ccf-rank
node scripts/query_ccf_rank.mjs "AAAI"
```

## Useful External Skills

Here are some third-party skills that are also useful for scientific workflows:

- [arxiv-search by yorkeccak](https://skills.sh/yorkeccak/scientific-skills/arxiv-search): Semantic arXiv search with natural-language queries.

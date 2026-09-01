# Jiuerli Visual Director

A Codex skill that converts a user-provided photograph into a sparse, centered travel-journal doodle on warm paper. It preserves the scene hierarchy and selected focal objects while simplifying secondary detail into unfinished, lively colored contours.

## What it produces

- Large uninterrupted paper margins around a compact central drawing island
- Clear focal objects with simplified secondary forms
- Wobbly, locally deformed colored contours with variable line weight
- Sparse color accents instead of full shading or dense hatching
- Short handwritten English fragments and incidental notebook marks
- One generated image per request, without silent retries

## Requirements

- Codex with image generation available
- A user-provided source photograph

## Install with Codex

```bash
python3 "${CODEX_HOME:-$HOME/.codex}/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo JiuerL/jiuerli-visual-director \
  --path skills/jiuerli-visual-director
```

The skill will be available on the next turn.

## Manual installation

```bash
git clone https://github.com/JiuerL/jiuerli-visual-director.git
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R jiuerli-visual-director/skills/jiuerli-visual-director \
  "${CODEX_HOME:-$HOME/.codex}/skills/"
```

## Usage

Attach a photograph and explicitly invoke the skill:

```text
$jiuerli-visual-director process this photo as a 4:3 landscape image.
```

The skill first explains which scene elements were retained, which forms are the focal points, and which spatial relationship anchors the composition. It then generates a single raster image.

## Public style assets

This repository intentionally includes the three style-authority images used by the skill:

- `style-authority-bplus.png`
- `line-authority-doodle-01.jpg`
- `line-authority-doodle-02.jpg`

They are part of the public skill distribution and are covered by the repository license.

## Repository layout

```text
skills/jiuerli-visual-director/
├── SKILL.md
├── agents/openai.yaml
└── assets/
    ├── style-authority-bplus.png
    ├── line-authority-doodle-01.jpg
    └── line-authority-doodle-02.jpg
```

## License

MIT. See [LICENSE](LICENSE).

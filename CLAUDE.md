# CLAUDE.md

## Project

KiCad PCB design for the servo motor control board of a quadruped robot (iPBL 2026 — International Project Based Learning). The board maps an Arduino Nano to 12 servo motors (M1–M12, 3 per leg), with LM1085-5.0 5V regulation and a power switch placed before the stepdown regulator.

## Files

- `nano_IPBL_2026.kicad_pro` / `.kicad_sch` / `.kicad_pcb` / `.kicad_prl` — KiCad 10 project (schematic + layout)
- `exports/` — SVG exports of copper layers (front and bottom)
- `.history/` — local editor history, git-ignored; never commit it
- `~*.lck` files — KiCad lock files, do not commit

## Design specs

- Vias: 1mm diameter, 0.4mm drill
- Copper pads: +0.25mm diameter over drill, 0.4mm drill holes
- 2-layer board

## Git conventions

- Do NOT add a Co-Authored-By line to commits
- Keep KiCad design-file changes (.kicad_pcb/.kicad_sch/.kicad_pro/.kicad_prl) in separate commits from docs/exports
- Ask the user what design changes they made before writing a commit message for KiCad files — the content isn't readable from diffs alone

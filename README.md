# Value Stream Playbook

Lean-Agile product development at enterprise scale.


## What this is

This is a practitioner's synthesis, not a new framework. It combines existing, well-documented work: Donald Reinertsen (flow economics), Klaus Leopold (Flight Levels), Mary and Tom Poppendieck (lean software development), Matthew Skelton and Manuel Pais (Team Topologies), Neal Ford and Rebecca Parsons (evolutionary architecture), and Ivar Jacobson (Use-Case 2.0). Some vocabulary (architectural runway, intentional architecture and emergent design) is borrowed selectively from the Scaled Agile Framework. It describes one way to apply these ideas where several product teams share enabler teams. Full references are in [section 11](docs/11-references.md).

## A note on role names

The value-stream role abbreviations (VSO, VSAL, VSAR, VSCX, VSQA) are working labels used inside this playbook. They are not established industry titles. Map them to whatever roles your organization already has.

## Repository layout

- `docs/`: the playbook, one Markdown file per section; figures in `docs/img/`
- `diagrams/`: draw.io source for the figures
- `mkdocs.yml`: site configuration (MkDocs Material)

## Building locally

```
pip install -r requirements.txt
mkdocs serve
```

## License

Text and diagrams are licensed under [CC BY 4.0](LICENSE).

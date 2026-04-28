# Changelog

## [0.1.0] — TBD (pre-release scaffold)

Initial scaffold. Submodule namespaces declared, schema drafted, no content extracted yet.

- Six phase submodules declared in `MODULE.json`: preconception, trimester-1, trimester-2, trimester-3, postpartum, lactation
- `schemas/prenatal-profile.schema.json` shipped, declares `health-charted/prenatal-profile` data type
- `my-data-templates/prenatal-profile.json` starter template
- Empty INDEX.json files for wiki, reference, research
- `requires_hc_min_version: 1.9.0` — module is authored against the HC v1.9 spec, which adds submodule-level `guides[]` (A2 sharpening), entity-placement authoring heuristic (A3 sharpening), and explicit `requires_hc_min_version` semantics (A1 sharpening)

Subsequent commits will add wiki entities, reference docs, research files, and guides.

# LSFIRE documentation website plan

## Purpose

Build a public, searchable LSFIRE User Guide modeled on the
[ELMFIRE User Guide](https://elmfire.io/). The audience is researchers who
want to build LSFIRE, run coupled fire–atmosphere simulations, and understand
the model and its inputs.

## Repository and publishing

- Keep this plan in the personal ERF-LSFIRE repository.
- Develop the user guide alongside the integrated code in
  [erf-model/LSFIRE](https://github.com/erf-model/LSFIRE). Use a `docs/`
  directory there for Sphinx sources and build configuration.
- Use the [LSFIRE README](https://github.com/erf-model/LSFIRE/blob/main/README.md)
  and the coupled regression examples as starting material. Keep a quick
  start and paper citation in the README and link to the full guide.
- Choose GitHub Pages or Read the Docs after reviewing the first site build.
  A custom domain and a PDF edition can follow once the guide is established.
- Link to the published guide from the personal repository and the ERF-Fire
  documentation hub so readers have a single maintained reference.

## First edition

| Section | Scope |
| --- | --- |
| Home | What LSFIRE does, how it fits into ERF, and how to cite the model paper |
| Getting Started | Dependencies, checkout, build, and the first coupled case |
| User Guide | Prescribed and atmospheric winds, fire feedback, inputs, and outputs |
| Model Formulation | Level-set propagation, Rothermel–Richards spread, and the ERF coupling |
| Verification and Case Studies | Idealized checks and regression cases, with separate links to the Palisades and Cram studies |
| Input Reference | Parameter names, defaults, units, and conditions checked against the documented code version |

The model description is [Liu et al. (2026), ERF-LSFIRE v1.0](https://doi.org/10.5194/egusphere-2026-5430).

## Development sequence

1. Add a Sphinx scaffold with a landing page and navigation. Build it locally
   and review the layout before selecting a publishing service.
2. Migrate the quick start and coupling guide from the existing documentation.
   Run the quick start from a fresh checkout and record the code and dependency
   revisions used.
3. Add the formulation, verification, case study, and parameter pages. Keep
   regression checks distinct from research case studies and tie numerical
   claims to their sources.
4. Review the guide with the model team, add a documentation build check, and
   publish the first edition. Add the site link to the relevant repository
   homepages.

The first edition is ready when readers can navigate and search the guide,
follow a verified build-and-run example, and find the paper citation and input
reference. The documentation build and internal links should pass before
publication.

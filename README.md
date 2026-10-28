# Zer0ism Studio

A browser-based workspace for exploring philosophical domains, comparing inquiry methods, studying philosophical views and traditions, recording propositions, and constructing revisable personal philosophy branches.

## Current features

- Interactive philosophical atlas with search and domain filtering.
- Expanded methodology catalog with goals, strengths, limitations, failure modes, and suggested workflows.
- Views and traditions guide with recurring ideas, internal variations, questions, and criticisms.
- Profile-level further reading links, with notes about each source's scope.
- Proposition library with domain, status, confidence, rationale, objections, provenance, and revision conditions.
- Local argument workbench with premise/conclusion maps, inference styles, objections, replies, and proposition links.
- Personal philosophy branches that can be edited and forked.
- Recursive audit checklist for examining Zer0ism's own principles and evaluation rules.
- Foundational charter with explicit limits and possible objections.
- Local JSON export/import and local workspace reset.
- Responsive dark interface; no build step or third-party dependencies.

The views guide includes both historical or intellectual traditions and position families. These are different kinds of profiles: a tradition is a changing body of debate and practice; a position family groups related answers to a question. Profiles are selective starting points with reading links, not claims that every thinker in a tradition agrees.

## Run locally

Open `index.html` in a modern browser. For best results, serve the folder with a static web server, for example:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Data and privacy

Edits are stored in the browser's `localStorage` on the current device/browser. There is no backend, account system, cross-device sync, or cloud persistence in this prototype. Export a JSON backup before clearing browser data.

## Design principles

1. A philosophical domain, method, tradition, position, proposition, and argument are distinct data types.
2. Classifications are cross-linked rather than treated as a single exhaustive hierarchy.
3. Propositions and argument maps are distinct records; a map makes reasoning inspectable but does not establish that it is valid or sound.
4. Propositions carry their rationale, objections, provenance, status, and revision conditions.
5. Traditions are internally diverse; summaries should name their scope, avoid speaking for every adherent, and link readers to source material.
6. The framework is not an authority that declares all philosophical disputes settled.
7. Zer0ism's own criteria remain open to recursive audit.

## Current limitations

- The atlas and profile library are selective starter taxonomies, not complete academic encyclopedias.
- Profile reading links are selective and do not yet provide full bibliographic metadata, citation validation, or comprehensive community-specific coverage.
- Argument maps use a flat premise list and one conclusion; nested subarguments and explicit rebuttal graphs are not yet supported.
- Personal branch proposition linking and append-only revision history are early-stage.
- No automated logical proof, evidence verification, or philosophical truth scoring is claimed.
- No automated tests or server persistence are included in this first static prototype.

## Suggested next phase

1. Define a versioned JSON schema for domains, methods, traditions, positions, propositions, arguments, sources, and revision events.
2. Expand profile reading lists with full source records, publication details, and citation validation.
3. Extend single-conclusion argument maps into explicit argument graphs (premises, inference rules, objections, rebuttals).
4. Add branch-to-proposition links and an append-only change log.
5. Add tests for import/export, editing, filtering, and branch forking.
6. Deploy as a static GitHub Pages site; consider a backend only when multi-user collaboration or sync is required.

## License

MIT — see `LICENSE`.

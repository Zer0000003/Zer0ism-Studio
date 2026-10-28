# Zer0ism Studio

A browser-based prototype for exploring philosophical domains, comparing methods, recording propositions, and constructing revisable personal philosophy branches.

## Current features

- Interactive philosophical atlas with search and domain filtering.
- Methodology catalog with goals, strengths, limitations, failure modes, and suggested workflows.
- Proposition library with domain, status, confidence, rationale, objections, provenance, and revision conditions.
- Personal philosophy branches that can be edited and forked.
- Recursive audit checklist for examining Zer0ism's own principles and evaluation rules.
- Foundational charter with explicit limits and possible objections.
- Local JSON export/import and local workspace reset.
- Responsive dark interface; no build step or third-party dependencies.

## Run locally

Open `index.html` in a modern browser. For best results, serve the folder with a static web server, for example:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Data and privacy

Edits are stored in the browser's `localStorage` on the current device/browser. There is no backend, account system, cross-device sync, or cloud persistence in this prototype. Export a JSON backup before clearing browser data.

## Design principles

1. A philosophical domain, methodology, theory, proposition, and argument are distinct data types.
2. Classifications are cross-linked rather than treated as a single exhaustive hierarchy.
3. Propositions carry their rationale, objections, provenance, status, and revision conditions.
4. The framework is not an authority that declares all philosophical disputes settled.
5. Zer0ism's own criteria remain open to recursive audit.

## Current limitations

- Starter taxonomy is intentionally selective, not a complete academic encyclopedia.
- Source citations and bibliographic records are not yet implemented.
- Personal branch proposition linking and append-only revision history are early-stage.
- No automated logical proof, evidence verification, or philosophical truth scoring is claimed.
- No automated tests or server persistence are included in this first static prototype.

## Suggested next phase

1. Define a versioned JSON schema for domains, traditions, methods, propositions, arguments, sources, and revision events.
2. Add source-backed records and citation validation.
3. Add explicit argument graphs (premises, inference rules, objections, rebuttals).
4. Add branch-to-proposition links and an append-only change log.
5. Add tests for import/export, editing, filtering, and branch forking.
6. Deploy as a static GitHub Pages site; consider a backend only when multi-user collaboration or sync is required.

## License

MIT — see `LICENSE`.

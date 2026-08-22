# ChatGPT skill plugins

Artifact-only releases of 3 skills-only app plugins for ChatGPT and Codex, with matching standalone skill ZIPs:

- **Mermaid Diagrams** — Author, convert, repair, validate, and optionally render portable Mermaid documents.
- **Modelica Projects** — Create, visually annotate, import, repair, and statically validate portable Modelica projects.
- **Portable Mind Maps** — Author, convert, merge, repair, and validate portable mind maps across open formats.

The development repository, tests, and Git history are intentionally not published here. Installable runtime files are distributed as ZIP assets on the [latest release](https://github.com/theisegoria/chatgpt-skill-plugins/releases/latest).

## Install version 2.0.0

1. Download and extract `chatgpt-skill-plugins-2.0.0.zip` from the release.
2. Add the extracted directory as a local marketplace:

   ```bash
   codex plugin marketplace add /absolute/path/to/chatgpt-skill-plugins-2.0.0
   ```

3. Install one or more plugins:

   ```bash
   codex plugin add mermaid-diagrams@ben-chatgpt-apps
   codex plugin add modelica-projects@ben-chatgpt-apps
   codex plugin add portable-mindmaps@ben-chatgpt-apps
   ```

4. Restart the ChatGPT desktop app and begin a new task.

Standalone skill ZIPs may instead be extracted so that their top-level skill folder lives under the user's Codex skills directory. Plugin and standalone distributions contain the same audited runtime skill files.

## Integrity and validation

Release assets include `SHA256SUMS.txt` and `release-manifest.json`. The archives are deterministic, path-safe, CRC-checked, schema-validated, and checked again after extraction. Static validation does not prove rendering, import, compilation, simulation, numerical correctness, or physical validity.

## Policies and support

See `PRIVACY.md`, `TERMS.md`, and `SUPPORT.md` in this repository. The plugins have no developer-operated server or telemetry; external desktop applications retain their own terms.

## License

Original material is licensed under Apache License 2.0. Format and platform names belong to their respective owners; see `NOTICE`.

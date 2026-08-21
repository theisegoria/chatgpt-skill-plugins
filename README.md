# ChatGPT skill plugins

Artifact-only releases of 3 skill-first plugins for ChatGPT and Codex:

- **Mermaid Diagrams** — Create and validate portable Mermaid diagram source.
- **Modelica Projects** — Create and statically validate portable, structured Modelica projects.
- **Portable Mind Maps** — Create portable Markdown, OPML, and FreeMind mind maps.

The development repository, tests, and Git history are intentionally not published here. Installable runtime files are distributed as ZIP assets on the [latest release](https://github.com/theisegoria/chatgpt-skill-plugins/releases/latest).

## Install version 1.0.0

1. Download and extract `chatgpt-skill-plugins-1.0.0.zip` from the release.
2. Add the extracted directory as a local marketplace:

   ```bash
   codex plugin marketplace add /absolute/path/to/chatgpt-skill-plugins-1.0.0
   ```

3. Install one or more plugins:

   ```bash
   codex plugin add mermaid-diagrams@ben-chatgpt-apps
   codex plugin add modelica-projects@ben-chatgpt-apps
   codex plugin add portable-mindmaps@ben-chatgpt-apps
   ```

4. Restart the ChatGPT desktop app and begin a new task.

## Integrity and validation

Release assets include `SHA256SUMS.txt` and `release-manifest.json`. The archives are deterministic, path-safe, CRC-checked, schema-validated, and checked again after extraction. Static validation does not prove rendering, import, compilation, simulation, numerical correctness, or physical validity.

## Policies and support

See `PRIVACY.md`, `TERMS.md`, and `SUPPORT.md` in this repository. The plugins have no developer-operated server or telemetry; external desktop applications retain their own terms.

## License

Original material is licensed under Apache License 2.0. Format and platform names belong to their respective owners; see `NOTICE`.

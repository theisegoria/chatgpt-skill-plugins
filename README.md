# ChatGPT skill plugins

Artifact-only releases of 4 skill-first plugins for ChatGPT and Codex:

- **MarkChart Mermaid** — Create and validate MarkChart-ready Mermaid diagram source.
- **MindNode Mind Maps** — Create portable Markdown and OPML mind maps for MindNode.
- **System Modeler Projects** — Create, validate, simulate, and document structured Modelica projects for Wolfram System Modeler.
- **Wolfram Notebooks** — Create structured Wolfram notebook artifacts from natural-language requests.

The development repository, tests, and Git history are intentionally not published here. Installable runtime files are distributed as ZIP assets on the [latest release](https://github.com/theisegoria/chatgpt-skill-plugins/releases/latest).

## Install version 0.2.0

1. Download and extract `chatgpt-skill-plugins-0.2.0.zip` from the release.
2. Add the extracted directory as a local marketplace:

   ```bash
   codex plugin marketplace add /absolute/path/to/chatgpt-skill-plugins-0.2.0
   ```

3. Install one or more plugins:

   ```bash
   codex plugin add markchart-mermaid@ben-chatgpt-apps
   codex plugin add mindnode-mindmaps@ben-chatgpt-apps
   codex plugin add system-modeler-projects@ben-chatgpt-apps
   codex plugin add wolfram-notebooks@ben-chatgpt-apps
   ```

4. Restart the ChatGPT desktop app and begin a new task.

## Integrity and validation

Release assets include `SHA256SUMS.txt` and `release-manifest.json`. The archives are deterministic, path-safe, CRC-checked, schema-validated, and checked again after extraction. Full Modelica compilation and simulation require Wolfram System Modeler. MarkChart rendering requires its one-time command-line folder grant. MindNode import is a separate user action using the portable Markdown or OPML output.

## Policies and support

See `PRIVACY.md`, `TERMS.md`, and `SUPPORT.md` in this repository. The plugins have no developer-operated server or telemetry; external desktop applications retain their own terms.

## License

Original material is licensed under Apache License 2.0. Bundled third-party material retains its own terms; see `NOTICE` and the notices inside each plugin. Wolfram System Modeler documentation excerpts are not included in public artifacts pending explicit downstream redistribution permission.

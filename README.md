# ChatGPT skill plugins

Artifact-only releases of three skill-first plugins for ChatGPT and Codex:

- **Wolfram Notebooks** creates structured Wolfram/Mathematica `.nb` notebooks.
- **MarkChart Mermaid** creates and statically validates MarkChart-ready Mermaid source.
- **System Modeler Projects** creates structured Modelica packages and includes Wolfram Research's official System Modeler AI toolkit.

The development source, tests, and Git history are intentionally not published here. Installable runtime files are distributed as ZIP assets on the [latest release](https://github.com/theisegoria/chatgpt-skill-plugins/releases/latest).

## Install the collection

1. Download and extract `chatgpt-skill-plugins-0.1.0.zip` from the release.
2. Add the extracted directory as a local marketplace:

   ```bash
   codex plugin marketplace add /absolute/path/to/chatgpt-skill-plugins-0.1.0
   ```

3. Install one or more plugins:

   ```bash
   codex plugin add wolfram-notebooks@ben-chatgpt-apps
   codex plugin add markchart-mermaid@ben-chatgpt-apps
   codex plugin add system-modeler-projects@ben-chatgpt-apps
   ```

4. Restart the ChatGPT desktop app and begin a new task.

## Integrity and validation

Release assets include `SHA256SUMS.txt` and `release-manifest.json`. The archives are deterministic, path-safe, CRC-checked, schema-validated, and compared against the committed private build inputs before publication.

The Wolfram notebook and Modelica generators have offline structural validation. Full notebook import/evaluation and Modelica compilation/simulation require Wolfram products. MarkChart CLI rendering requires MarkChart's one-time command-line folder grant.

No license has been selected for the original plugin material. Bundled third-party material retains its own license and attribution.

# Migration to the open-format collection

## Version 1 to version 2

- Canonical inputs now carry `version: 2` and use the unified `mermaid_tool.py`, `modelica_tool.py`, or `mindmap_tool.py` command families.
- Existing Mermaid source and Markdown can be imported directly.
- Existing directory-form Modelica packages can be imported; visual data is added only when requested, and existing graphics require explicit replacement authorization.
- Existing v1 Markdown, OPML, and FreeMind mind maps can be imported; richer metadata is represented in canonical JSON and conversion loss is reported per target format.
- The v1 generators remain in the v2 bundles for explicit legacy workflows, but new skill instructions route to the v2 tools.

## Earlier product-line migration

Version 0.3.0 establishes a three-plugin collection:

- Install `mermaid-diagrams` for Mermaid source and Mermaid-enabled Markdown.
- Install `modelica-projects` for portable `.mo` package trees and static structural checks.
- Install `portable-mindmaps` for Markdown, OPML 2.0, and FreeMind-compatible `.mm`.

Earlier proprietary notebook and proprietary Modelica runtime integrations are retired and are not distributed. Existing generated files remain under the user's control, but the collection no longer creates, validates, imports, launches, or claims compatibility with those proprietary formats or applications.

The Modelica plugin now guarantees portable source structure only. Compilation, simulation, rendering, and physical validation require independently selected tools and separately reported evidence.

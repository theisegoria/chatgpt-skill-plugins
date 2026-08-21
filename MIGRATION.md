# Migration to the open-format collection

Version 0.3.0 establishes a three-plugin collection:

- Install `mermaid-diagrams` for Mermaid source and Mermaid-enabled Markdown.
- Install `modelica-projects` for portable `.mo` package trees and static structural checks.
- Install `portable-mindmaps` for Markdown, OPML 2.0, and FreeMind-compatible `.mm`.

Earlier proprietary notebook and proprietary Modelica runtime integrations are retired and are not distributed. Existing generated files remain under the user's control, but the collection no longer creates, validates, imports, launches, or claims compatibility with those proprietary formats or applications.

The Modelica plugin now guarantees portable source structure only. Compilation, simulation, rendering, and physical validation require independently selected tools and separately reported evidence.

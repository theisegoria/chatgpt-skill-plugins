# Versioning and compatibility

The collection uses Semantic Versioning.

At version 1.0.0, each plugin's documented JSON schemas, command flags, output extensions, output-directory shape, overwrite policy, exit behavior, and evidence boundary are stable public interfaces.

Version 2.0.0 introduces new canonical document schemas and unified author/import/lint/repair/export CLIs. The v1 release remains available for consumers that require its frozen contracts; v2 files use an explicit root `version: 2` discriminator.

- Major releases may make incompatible interface or output-structure changes.
- Minor releases add backward-compatible formats, options, validations, or skills.
- Patch releases correct behavior without breaking documented contracts.

Identical valid input, generator version, and options must produce byte-identical portable output. Static validation never implies rendering, native import, compilation, simulation, numerical correctness, or physical validity. Optional runtime evidence applies only to the exact runtime invocation reported.

Python 3.11, 3.12, and 3.13 are supported for bundled scripts. The skills themselves require only a compatible ChatGPT or Codex plugin host with local file access.

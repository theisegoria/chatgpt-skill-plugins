# Versioning and compatibility

The collection uses Semantic Versioning.

At version 1.0.0, each plugin's documented JSON schemas, command flags, output extensions, output-directory shape, overwrite policy, exit behavior, and evidence boundary are stable public interfaces.

- Major releases may make incompatible interface or output-structure changes.
- Minor releases add backward-compatible formats, options, validations, or skills.
- Patch releases correct behavior without breaking documented contracts.

Identical valid input, generator version, and options must produce byte-identical portable output. Static validation never implies rendering, import, compilation, simulation, numerical correctness, or physical validity.

Python 3.11, 3.12, and 3.13 are supported for bundled scripts. The skills themselves require only a compatible ChatGPT or Codex plugin host with local file access.

# CEDAR Model Library Roundtrip (Retired)

This repository held a command-line tool that read an administrator export, parsed every artifact
with the Java model library, wrote each one back as JSON or YAML, and compared the result with the
original. The tool is retired. This repository no longer builds, and no CEDAR build train or
release includes it.

Other checks now cover round-trip fidelity. The CI of `cedar-artifact-library` verifies that the
shared corpus writes the same JSON through YAML. `cedar_snapshot_read_audit.py` in
`cedar-development/ops` reads and rewrites every artifact of a production snapshot with both
model libraries.

Earlier implementations remain in Git history and the existing release tags.

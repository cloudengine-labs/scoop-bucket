# Scoop bucket for CloudEngine Labs tools

A [Scoop](https://scoop.sh) bucket for Windows.

## sbom-sentinel

Generates SBOMs, aggregates vulnerability findings from Grype and Trivy, and plans
dependency fixes you can preview before anything changes. More at
[sbomsentinel.com](https://sbomsentinel.com).

```powershell
scoop bucket add cloudengine-labs https://github.com/cloudengine-labs/scoop-bucket
scoop install sbom-sentinel
sbom-sentinel --version
```

Scoop also installs `syft`, `grype` and `trivy`, which `sbom-sentinel` drives. Upgrade with
`scoop update sbom-sentinel`.

The Windows build is published on this repository's
[Releases](https://github.com/cloudengine-labs/scoop-bucket/releases) page together with its
SHA-256 checksum; Scoop verifies the checksum on every install. The binary is not code-signed, so
Windows SmartScreen may ask for confirmation the first time you run it.

Licensed under Apache License 2.0.

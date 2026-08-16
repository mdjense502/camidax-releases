# CAMIDAX Releases

Official public distribution repository for signed CAMIDAX update manifests and release artifacts.

## Trust model

CAMIDAX clients do **not** trust this repository simply because it is hosted on GitHub. Official releases are accepted only when their manifests verify against the CAMIDAX Ed25519 release authority embedded in the client.

Current release authority:

`ed25519:a6e4e67adf1ca61254366505`

The private signing key is never stored in this repository.

## Layout

- `channels/alpha.json` — current alpha release manifest
- `channels/beta.json` — current beta release manifest
- `channels/stable.json` — current stable release manifest
- `releases/<version>/` — immutable public artifacts and version-specific signed manifests

## Security rules

This repository may contain only public release data and binaries intended for distribution. Never commit private signing keys, passwords, relay secrets, runtime identity/trust databases, source-code secrets, or machine-specific configuration.

A compromised hosting location alone must not be sufficient to publish a valid CAMIDAX update: clients verify the signed manifest and artifact SHA-256 before installation.

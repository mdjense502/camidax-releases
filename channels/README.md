# CAMIDAX Release Channels

This directory contains only current, cryptographically signed CAMIDAX channel manifests.

When populated:

- `alpha.json` points to the current signed alpha release.
- `beta.json` points to the current signed beta release.
- `stable.json` points to the current signed stable release.

Do not create placeholder channel manifests. A channel file is published only after the corresponding release artifact exists at its final HTTPS URL and the manifest has been signed by an authorized CAMIDAX release key.

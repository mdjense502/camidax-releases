# CAMIDAX Versioned Releases

Each public release lives under an immutable version directory such as:

`releases/0.0.3-alpha/`

A version directory may contain the public installer/package and its version-specific signed manifest. Published artifacts must match the SHA-256 and size recorded in that signed manifest.

Do not replace an artifact in-place after publication. Publish a new CAMIDAX version instead.

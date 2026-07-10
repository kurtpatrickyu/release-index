# Release Index

This repository stores lightweight version metadata for private applications and internal tools.

The metadata files are intended to be read by applications that need to check whether a newer version is available. Each application uses its own opaque manifest identifier.

## Structure

```text
manifests/
  <manifest-id>.json
```

Each manifest file contains the latest published version information for one application.

Example:

```json
{
  "schema": 1,
  "latest_version": "0.4.1",
  "latest_tag": "v0.4.1",
  "published_at": "2026-07-10T00:00:00Z"
}
```

## Notes

* Manifest identifiers are intentionally opaque.
* This repository does not contain application source code.
* This repository does not contain installers, release notes, or private project details.
* Manifest files are updated by release automation.

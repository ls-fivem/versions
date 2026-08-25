# versions

Auto-updated by the release workflow. One JSON file per resource, updated whenever
that resource ships a release. Never edit these by hand - they get overwritten.

## Structure

```
versions/
  ls-admin.json
  ...
```

## Example entry

```json
{
  "resource": "ls_admin",
  "version": "1.4.2",
  "tag": "v1.4.2",
  "released_at": "2026-08-25T12:00:00Z"
}
```

## Uses

- A server-side script can fetch `raw.githubusercontent.com/ls-fivem/versions/main/versions/<resource>.json`
  to check whether a deployed resource is out of date.
- A simple dashboard could just render every file in `versions/` as a table.

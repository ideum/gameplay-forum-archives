# Gameplay Forum Archives

Archival snapshot of the v1 and beta gameplay forums.

Snapshots taken using `wget` and a script tag was injected using `sed`.
Otherwise the pages are unaltered from their original public appearance.

###`wget` command to clone site

```bash
wget --mirror --page-requisites --adjust-extension --no-parent --convert-links $site_url
```

### `sed` command to add script tag

```bash
find . -iname "*.html" | xargs sed -i '/<\/head>/i\<link href="/assets/archive.css" rel="stylesheet">'
```

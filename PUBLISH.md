# Publishing this fork

The original `pdphilip/elasticsearch` package was exported from `vendor` after the upstream GitHub repository became unavailable. This fork is published on Packagist as **`vldmir/pdphilip-elasticsearch`** (the `pdphilip` vendor namespace is already claimed).

## Repository

Public repo: [github.com/vldmir/pdphilip-elasticsearch](https://github.com/vldmir/pdphilip-elasticsearch).

Optional local clone path: `/home/vldmir/projects/wdwkservices/coder/pdphilip-elasticsearch`.

## Push to GitHub

1. Create an empty GitHub repository if needed.

2. From this directory:

```bash
cd /home/vldmir/projects/wdwkservices/coder/pdphilip-elasticsearch
git remote add origin git@github.com:vldmir/pdphilip-elasticsearch.git
git branch -M main
git push -u origin main
git tag v5.3.0 && git push origin v5.3.0
```

3. In the consuming Laravel app, use a VCS repository in `composer.json`:

```json
{
  "type": "vcs",
  "url": "https://github.com/vldmir/pdphilip-elasticsearch.git"
}
```

Then require: `composer require vldmir/pdphilip-elasticsearch` (or `./vendor/bin/sail composer require vldmir/pdphilip-elasticsearch`).

## Version tags

For Composer stable installs, publish tags (e.g. `v5.3.0`):

```bash
git tag v5.3.0
git push origin v5.3.0
```

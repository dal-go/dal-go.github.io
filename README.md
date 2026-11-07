# dal-go.github.io

Source for **https://dal-go.github.io**. Every HTML page is a minimal redirect to the matching URL on the official site, **https://dalgo.io/**.

There is no sitemap. `.nojekyll` stays so GitHub Pages serves these files as-is. This repository has no `CNAME`; Pages publishes the default `dal-go.github.io` host.

## Redirects

| Path | Destination |
| --- | --- |
| `/` | https://dalgo.io/ |
| `/tugql/` | https://dalgo.io/tugql/ |
| `/tugql/examples/` | https://dalgo.io/tugql/examples/ |
| `/dtql/` | https://dalgo.io/tugql/ |
| unknown paths (`404.html`) | https://dalgo.io/ |

`/dtql/` is not listed in https://dalgo.io/sitemap.xml. The old page, and https://dalgo.io/dtql/, only point at TugQL, so the redirect goes to https://dalgo.io/tugql/.

Each page sets a canonical link, a zero-delay meta refresh, `noindex, follow`, `location.replace`, and a visible link.

## Schema documents

`tugql/schema.json`, `tugql/schema.yaml`, `dtql/schema.json`, and the TugQL example YAML files stay. The schema `$id` is `https://dal-go.github.io/tugql/schema.json`, and https://dalgo.io/dtql/schema.json references that URL.

## License

MIT — see `LICENSE`.

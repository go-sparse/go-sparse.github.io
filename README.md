# go-sparse.github.io

The go-sparse landing page (Hugo), served at <https://go-sparse.github.io/>.

The layout is the go-* family template, taken from the
[`go-fleettools/landingkit`](https://github.com/go-fleettools/landingkit) Hugo
module (`go.mod`, `kit.go`, and the `[module]` import in `hugo.toml`):
`layouts/index.html` is this site's own, the shared stylesheet and partials come
from the module, and `[params.brand]` in `hugo.toml` is read from the logo's
gradient by `landingkit brand static/img/logo.svg`.

```sh
hugo server
```

| Workflow | What |
| --- | --- |
| `hugo.yml` | builds on pull requests; builds and deploys to Pages on `main` |
| `ci.yml` | the site builds and names every repository |
| `links.yml` | every link and image of the built site resolves |

The status of each package on the page is the truth at the time of writing:
`sparse` is released as v0.1.0 (the latest tag of go-sparse/sparse).

BSD-3-Clause.

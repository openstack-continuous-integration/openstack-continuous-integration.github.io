# openstack-continuous-integration.github.io

The landing page for the [openstack-continuous-integration](https://github.com/openstack-continuous-integration) organisation.
Live at <https://openstack-continuous-integration.github.io/>.

A single-page Hugo site. The prose, the pills and the repository cards all live
in `hugo.toml` under `[params]`; `layouts/index.html` is shared across the
fleet's org sites and should not need editing to add a repository — add a
`[[params.repos]]` block instead.

| Path | Purpose |
| --- | --- |
| `hugo.toml` | site config, prose and the repository cards |
| `layouts/index.html` | the whole page: markup, CSS, theme toggle |
| `static/img/logo.svg` | the 88px organisation mark |

Theme: light, dark and system, defaulting to system, applied before first paint.

```sh
hugo server -D      # local preview on :1313
hugo --minify       # what CI builds
```

BSD-3-Clause.

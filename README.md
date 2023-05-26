## Desc

the hugo module based on `hugo-enterprise` for website: `chipchain.netlify.app`

---

## Use module

config in your website project:

`./config/_default/config.yaml`

```yaml
module:
  imports:
    - path: github.com/zeeis/hugo-chipchain-theme
    - path: github.com/zeeis/hugo-enterprise
```

`./go.mod`

```mod
require github.com/zeeis/hugo-chipchain-theme v0.1.6
require github.com/zeeis/hugo-enterprise v0.1.24
```

---

## Publish new package

git tag a commit of `hugo-chipchain-theme` with version (eg: `v0.2.0`), then push.

config `go.mod` of your website project to use specific version module

```mod
require github.com/zeeis/hugo-chipchain-theme v0.2.0
```

---

## Content

- themes
  - `data/theme/chipchain.yaml`
- [widgets](./docs/widgets.md)
  - cc.hero
  - cc.features

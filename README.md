# Offsend install site

Static GitHub Pages site for [install.offsend.io](https://install.offsend.io).

| URL | Content |
| --- | --- |
| `/` | Install instructions |
| `/cli` | Bash installer (`curl -fsSL https://install.offsend.io/cli \| bash`) |

## Setup (one time)

1. **GitHub Pages** → Settings → Build and deployment → Source: **GitHub Actions**
2. **Custom domain** → `install.offsend.io` (DNS CNAME to this repo’s Pages host)
3. In **Offsend/Offsend** repository secrets, add `INSTALL_REPO_TOKEN` (PAT with `contents:write` on this repo)

The `cli` script and landing page are updated automatically from
[Offsend/Offsend](https://github.com/Offsend/Offsend) when `Scripts/install.sh` changes on `main`.

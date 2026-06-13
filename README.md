# Notion Flow

> Write in Notion, publish to your GitHub blog in one click — a non-intrusive, pure-frontend browser extension.
> 在 Notion 写作，一键发布到 GitHub 博客 —— 非侵入、纯前端的浏览器插件。

**Website / 官网:** the landing page lives in this repo (`index.html`, `en/index.html`) and is served via GitHub Pages.
**Install / 安装:** [Chrome](https://chromewebstore.google.com/detail/notion-flow/mcabmofnikepdpecekdlildkmffpmokh) · [Edge](https://microsoftedge.microsoft.com/addons/detail/notion-flow/pppmbeffejpbfgdmhmgmlppefaeaimfh)
**Docs / 文档:** https://notion-flow.xheldon.com/ ([English](https://notion-flow.xheldon.com/en/))
**Downloads / 下载:** see [Releases](https://github.com/Xheldon/Notion-Flow-Prod/releases) (built extension `.zip`, published automatically by CI)

---

## What this repo is / 这个仓库是什么

This public repo serves three purposes:

1. **Website** — the marketing/intro landing page (plain HTML/CSS, no build step).
2. **Issue tracking & discussion** — [Issues](https://github.com/Xheldon/Notion-Flow-Prod/issues) · [Discussions](https://github.com/Xheldon/Notion-Flow-Prod/discussions).
3. **Release artifacts** — the packaged Chrome extension is published here as GitHub Releases by the source repo's CI.

The extension source code lives in a separate private repository.

本公开仓库承担三个职责：① 官网落地页（纯 HTML/CSS，无需构建）；② 问题反馈与讨论；③ 发布产物（插件打包 `.zip` 由源码仓库 CI 自动发布到 Releases）。插件源码位于另一个私有仓库。

---

## Local preview / 本地预览

It is plain static HTML — just open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8080   # then open http://localhost:8080
```

## Enable GitHub Pages / 启用 Pages

Settings → Pages → Source: **Deploy from a branch** → `main` / root.
A `.nojekyll` file is included so folders and assets are served as-is.

To use a custom domain (e.g. `notion-flow.xheldon.com`), add a `CNAME` file with that
domain and point the DNS accordingly. (Not committed here to avoid clobbering existing DNS.)

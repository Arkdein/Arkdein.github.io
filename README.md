# 语文 AI 实验室 · Languages AI Lab

Landing page for Randall's classroom web tools at River Valley High School. It links to each tool where it already lives; the tools themselves are not moved or copied here.

| Tool | Live app | Repository |
|---|---|---|
| 庖丁 · 层次分析练习 | https://arkdein.github.io/paoding/ | [Arkdein/paoding](https://github.com/Arkdein/paoding) |
| 字斟句酌 · 文言字词 | https://arkdein.github.io/zizhen/ | [Arkdein/zizhen](https://github.com/Arkdein/zizhen) |
| 词游记 · Word Journey | https://arkdein.github.io/ciyouji/ | [Arkdein/ciyouji](https://github.com/Arkdein/ciyouji) |
| 杏坛 · ClassroomBoard | https://arkdein.github.io/xingtan/ | [Arkdein/xingtan](https://github.com/Arkdein/xingtan) |

## Deploy (once, about 5 minutes)

1. On GitHub, create a new **public** repository named exactly **`Arkdein.github.io`**.
   A repository with this name becomes your user site, served at `https://arkdein.github.io/`.
   The tools stay at their current addresses (`/paoding/`, `/zizhen/` …), so nothing changes for students.
2. Upload `index.html` and this `README.md` to the `main` branch (Add file → Upload files).
3. Go to **Settings → Pages**, set *Source* to "Deploy from a branch", choose `main` and `/ (root)`, then save.
4. After a minute the page is live at `https://arkdein.github.io/`.

## Editing

Everything is in `index.html`: one file, no build step.

- **Two languages:** every piece of text appears twice, once with `class="l-en"` and once with `class="l-zh"`. The 中文 / EN switch in the header shows one set. When you change wording, change both.
- **Default language:** follows the visitor's browser (Chinese if it prefers Chinese, otherwise English). A visitor's own choice is remembered on that device.
- **Add a tool:** copy one `<article class="card">…</article>` block inside `<div class="cards">` and change the text and links.
- **Log:** add a `<li>` at the top of `<ol class="log">`.
- **Accent colour:** change `--accent` and `--accent-line` (same colour plus `80` for 50% opacity) at the top of the `<style>` block.

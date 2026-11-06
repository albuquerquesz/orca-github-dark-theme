# GitHub Dark for Orca

A dark application theme inspired by GitHub's default dark palette, with matching terminal colors.

Select **GitHub Dark** in Appearance settings for the app and in terminal theme settings
for matching ANSI colors. Includes syntax colors for source files and Markdown.

The page is GitHub's canvas (`#0d1117`). Cards, muted surfaces and the sidebar use the
inset chrome (`#010409`), the same step the light theme takes with `#f6f8fa`. Secondary
controls use `#282e33`, lifted off that chrome by about the same amount GitHub Light
uses `#d8dee4` on `#f6f8fa`, so buttons such as **AI Fix** stay visible, including their
translucent hover state. The secondary foreground stays `#e6edf3`.

Muted text uses `#9198a1` rather than Primer's `#8b949e`. On the secondary surface that
comment gray is 4.47:1, just under 4.5:1; `#9198a1` clears it (4.7:1) and still reads as
secondary text on the page and on inset chrome. The primary button is `#1f6feb` with
white text: GitHub's brighter accent `#2f81f7` is only 3.8:1 against white, so it stays
the cursor and link hue, not the button fill.

## Release

The repository is the source. It is not in the community catalog until both of these
land on the default branch's release commit:

```sh
git tag -a v1.0.0 -m v1.0.0 && git push origin v1.0.0
gh repo edit albuquerquesz/orca-github-dark-theme --add-topic orca-plugin
```

The tag must match `version` in `orca-plugin.json`. If the palette changes after a
preview, bump that version and tag the new commit instead. The listing then shows up at
https://www.onorca.dev/plugins/albuquerquesz/orca-github-dark-theme.

## Attribution

Adapted for Orca from the [GitHub Dark Default upstream project](https://github.com/primer/github-vscode-theme).
The Orca token mapping is maintained here; this is an unofficial port.
Upstream MIT notices are included in [LICENSE](LICENSE).

# GitHub Dark for Orca

A dark application theme inspired by GitHub's default dark palette, with matching terminal colors.

Select **GitHub Dark** in Appearance settings for the app and in terminal theme settings
for matching ANSI colors. Includes syntax colors for source files and Markdown.

The interface sits on a neutral gray, lighter than GitHub's blue-black canvas.
The page and the editor are `#1e1e1e`. Cards, muted surfaces and the sidebar are
`#262626`. Secondary controls use `#333333`, so buttons such as **AI Fix** stay
visible on those panels, including their translucent hover state. Selection is
`#404040`, the same gray family, instead of GitHub's blue wash. Body text is `#e6e6e6`.

Muted text uses `#9e9e9e`, which clears 4.5:1 on the secondary surface. The primary
button stays `#1f6feb` with white text. Syntax colors stay the GitHub Dark Default set.

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

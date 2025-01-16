# Researcher

A simple monospaced resume theme for Hugo. It was ported from Jekyll theme
[ankitsultana/researcher](https://github.com/ankitsultana/researcher) and [ojroques/hugo-researcher](https://github.com/ojroques/hugo-researcher)

## Typeface
Available fonts:
- Inconsolata (default) -> monospace, sans-serif, best in light format
- Space Grotesk -> monospace, serief, best in medium
- Inter -> Grotesk style, best in medium for headers
- Barlow, sans-serif -> round, tight
- Geist

To add custom fonts, go to baseof.html in "layouts/default" and import the link at the top of the page, then edit config correspondingly. 

## Installation
This theme uses Sass to generate CSS files so make sure you have the
*extended* Hugo version installed.

Add the theme to your site's `themes` directory:
```bash
git submodule add https://github.com/alamine53/hugo-theme-53.git themes/theme-53
```

Update the theme option in `config.toml`:
```toml
theme = "theme-53"
```

## Configuration
A self-explanatory configuration file is present in
[exampleSite/config.toml](https://github.com/alamine53/hugo-theme-53/blob/master/exampleSite/config.toml),
along the files of a demo website.

## Typeface


## KaTeX
You can enable [KaTeX](https://katex.org/) (math typesetting) by including
`math: true` in your content files. Or you can enable it globally by setting
`math` to `true` in your project config.

Hugo introduces tags when it sees newlines which breaks KaTeX block
environments. The theme has a `math` shortcode to circumvent this issue:
```md
{{< math >}}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
{{< /math >}}
```
Check [this
issue](https://github.com/alamine53/hugo-theme-53/issues/1#issuecomment-697247056)
for more details.

## License
[GPL-3.0 License](https://github.com/alamine53/hugo-theme-53/blob/master/LICENSE)

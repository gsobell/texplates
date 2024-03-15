# bidi-article

When typesetting bidirectional documents, special attention must be given to alignment direction.

I personally prefer `LuaTeX` with the `babel` package to `XeTeX` with `polyglossia`, though I have dabbled with both.

Inline RTL in LTR blocks shouldn't be an issue

As for aligning entire blocks, there are multiple options:

To change the alignment:

```
\raggedright
\raggedleft
```
To change the environment:

```
\begin{flushright}
\end{flushright}
```

Good reference for [alignment tips here](https://tex.stackexchange.com/questions/195774/how-to-right-align-any-line-or-word-in-a-paragraph-in-any-documentclass).

For side by side, see `paracol` and `multicol` packages.

## Common (Avoidable) Pitfalls

- Not having specified font installed
- LaTeX editor set to compile with engine other than LuaTeX/XeTeX (ie without Unicode support)

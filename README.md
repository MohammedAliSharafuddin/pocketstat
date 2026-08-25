# PocketStat

Browser-based statistics teaching tool. **R runs entirely in your browser**
via [webR](https://docs.r-wasm.org/webr/latest/). No server, no install, no
account, and no data leaves your device.

**Live:** https://mohammedalisharafuddin.github.io/pocketstat/

## What this repository is

A **render mirror**. It holds only the built output of
`shinylive::export()`. Do not edit anything here: every file is generated and
is overwritten on the next build. Development happens in the private source
repository.

## Covered techniques

Descriptive statistics, distribution shape, z-scores, one-sample tests,
two-sample tests, one-way ANOVA, Kruskal-Wallis, correlation, correlation
matrix, regression, chi-square, reliability (Cronbach's alpha), and
exploratory factor analysis. Each with assumption checks, effect sizes with
confidence intervals, APA-style tables, and a visible R-code view.

## First load

The first visit downloads the R WebAssembly runtime, roughly 73 MB. Expect
anywhere from about 12 seconds to a few minutes depending on the connection.
It is cached afterwards, so later visits are fast and work offline.

## Embedding in Moodle or another LMS

Add a **URL** resource pointing at the live link above, or embed it in a
**Page** with an iframe:

```html
<iframe src="https://mohammedalisharafuddin.github.io/pocketstat/"
        width="100%" height="800" style="border:0"
        title="PocketStat"></iframe>
```

Nothing needs to be installed on the LMS, and no student data reaches the
server, since all computation happens in the browser.

## Licence

See the source repository.

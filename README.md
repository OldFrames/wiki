# logsex

logsex is a template repository for deploying Logseq graph to GitHub Pages.

See also: [soyart.github.io/logsex](https://soyart.github.io/logsex)

## Scripts and Git hooks

logsex provides a set of shell scripts to work with Logseq documents.

For example, `remove-collapsed.sh` quickly remove occurrences of `collapsed::`
tag in Markdown documents. This prevents needless changes from our togglings.

We can also enable a pre-commit Git hook that will run `remove-collasped.sh`
on all files easily with:

```shell
git config --local core.hooksPath .githooks/
```

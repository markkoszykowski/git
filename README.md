```shell
git config --global init.defaultBranch main
```

```shell
git config --global core.attributesFile ~/.gitattributes
```

```shell
git config --global filter.gitignore.smudge 'tmp=$(mktemp); cat >> "${tmp}"; printf "# %f\n\n%s\n\n\n" "$(cat "${tmp}")" >> .gitignore; cat "${tmp}"; rm "${tmp}"'
git config --global filter.gitignore.clean 'cat'
```

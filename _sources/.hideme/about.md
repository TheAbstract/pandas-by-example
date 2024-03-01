# pandas by example

Inspired by chrisalbon's old site (which he deleted and no longer hosts).
- https://github.com/chrisalbon/chrisalbon_com_old [repo has also been deleted]
- https://web.archive.org/web/20220304071051/https://chrisalbon.com/
- https://github.com/chrisalbon/code_py
- https://github.com/dfayzur/dinhvankiet124.github.io
- https://chrisalbon.com/Home

similar to other 'x by example' sites, but focusing on a tool rather than a language.

for example:
- https://doc.rust-lang.org/rust-by-example/ - for x by example ideas
- https://github.com/mmcgrana/gobyexample https://gobyexample.com - code here apparently is not idiomatic go
- similar but not the same thing https://github.com/quangvinh1986/pandas-by-example
- similar but not the same thing https://github.com/frankligy/pandas_by_examples


## todo

- [ ] pandas-by-example [mvp replicating official tutorial] <https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html>
	- https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html#
	- https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html
	- https://pandas.pydata.org/pandas-docs/stable/user_guide/basics.html

- [ ] add note about GroupBy objects 
> "This grouped variable is now a GroupBy object. It has not actually computed anything yet except for some intermediate data about the group key df['key1']. The idea is that this object has all of the information needed to then apply some operation to each of the groups." - Python for Data Analysis
- [ ] has embedded editor https://rust-lang.github.io/mdBook/format/theme/editor.html, is there a way to do this with jupyter-book?
- [ ] how to update footer

## to publish

- https://jupyterbook.org/en/stable/start/publish.html

- in a separate branch `gh-pages` put contents of `_build/html`

```
rm *.ipynb _config.yml _toc.yml intro.md
mv _build/html/* .
rm -rf _build/
```


jb walkthrough:
- (basics)[https://jupyterbook.org/en/stable/start/overview.html]: write, build, publish.
- use separate branches for source (main) vs build (gh-pages).
- chapters organised as separate files.

## etc

- https://github.com/extremq/pandas-training
- https://stackoverflow.com/questions/36684013/extract-column-value-based-on-another-column-in-pandas
- https://www.statology.org/pandas-extract-column-value-based-on-another-column/
- https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.query.html
- https://towardsdatascience.com/pandas-2-0-a-game-changer-for-data-scientists-3cd281fcc4b4

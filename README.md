# phd_thesis_template
A LaTeX template for PhD thesis

# Initialize cryptobib submodule for references after clone
See https://cryptobib.di.ens.fr for details.
```
git submodule update --init
```

# Manual
- adapt your data in metadata.tex, packages.tex (only hyperref infos)
- have fun writing your thesis


# Compile version for a submission 
- check that draft mode in document class is not active,
- check that \overfullrule= is in a comment
- run
  ```
  latexmk -pdf phd-thesis
  ```
- and the some bibtex runs on the files given at the end of latexmk execution, e.g.,
  ```
  bibtex phd-thesis1-blx
  bibtex phd-thesis2-blx
  ```

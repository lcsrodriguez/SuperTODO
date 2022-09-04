# SuperTODO - TODO $\TeX$ extension

<img src="https://img.shields.io/static/v1?label=LaTeX package&message=supertodo&color=ff0000"/>

## Introduction

LaTeX package for TODO commands


This package is written using the $\LaTeX 2_\varepsilon$ environment which provides us high-level commands for structuring new packages.


**Open to contributions**: Feel free to submit a PR in order to extend the available features for a better LaTeX writing experience.

## Features

### Available environments

| Level  | Background color  | Inline | Block |
|:------:|------------------|--------|-------|
|  INSERT      |  GREEN       |  ✅      |  ✅     |
|  UPDATE      |    YELLOW         |  ✅      |  ✅     |
|  DELETE      |       RED           | ✅       |  ✅     |
|  REVIEW      |       BLUE               |  ✅      |  ✅     |


### Add a new command

If you want to implement a new command, denoted below as `abcde`, please procede as follows:

```latex
\usepackage{supertodo}

% To be specified AFTER the supertodo package import, NEVER BEFORE !!
\NewDocumentCommand\abcdeTD{O{block} s m}{
    \block[#1][<capital>][<bgcolor>][<fgcolor>][#2]{#3}
}
```
where you can specify:
- `<capital>`:
- `<bgcolor>`:
- `<fgcolor>`:

## References

- https://www.overleaf.com/learn/latex/Understanding_packages_and_class_files
- https://www.overleaf.com/learn/latex/Writing_your_own_package
- https://www.overleaf.com/learn/latex/Margin_notes

## License


Please check the [LICENSE](LICENSE) file for the complete license information.

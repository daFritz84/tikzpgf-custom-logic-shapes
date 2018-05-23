# Custom IEC logic shapes for TikZ/PGF

This TikZ library is designed to enhance the existing _circuits.logic.IEC_ library with additional logic components (e.g., adders, multiplexers, ...).

## Getting Started

Just copy the files _pgflibraryshapes.gates.logic.custom.code.tex_ and _tikzlibrarycircuits.logic.custom.code.tex_ to the root of your latex directory and include them like a normal TikZ library in your main TeX file. The files are then found and included by your TeX compiler through the naming convention.

```
\usepackage{pgf,tikz}

\usetikzlibrary{
	circuits.logic.custom,
	circuits.logic.IEC,
}
```
A full working example of the library can be found in _example.tex_.

## Available Shapes

* Half Subtractor
* Multiplexer
* RS-Latch
* D-FlipFlop

## Acknowledgements

* Martin Scharrer for his superb example at [TeXample.net](http://www.texample.net/tikz/examples/d-flip-flops-and-shift-register/)

## Additional Design Notes

This project tries to stay as close as possible to the workings of the original _circuits.logic.IEC_ TikZ library where it seems appropriate (e.g., variable number of inputs, choice of inversion, ...). However, this does not make sense for every component. If you have suggestions or already have a proper pull request in place, please open up an issue and I will try to incorporate your contribution into this project.

The original _circuits.logic.IEC_ files can usually be found in your local TeX distribution folder at the following locations:

* _[TeX distro root]/texmf-dist/tex/generic/pgf/frontendlayer/tikz/libraries/circuits/tikzlibrarycircuits.logic.IEC.code.tex_
* _[TeX distro root]/texmf-dist/tex/generic/pgf/libraries/shapes/circuits/pgflibraryshapes.gates.logic.IEC.code.tex_

## License

This project is licensed under the GPL License - see the [LICENSE.md](LICENSE.md) file for details

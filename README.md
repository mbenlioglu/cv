#  Personal CV & Resume

This repository is my personal CV/resume designed in LaTeX using definitions provided under
[moderncv](https://ctan.org/pkg/moderncv) package. For a full example of all functions provided by
`moderncv` you can check [this](http://mirrors.ctan.org/macros/latex/contrib/moderncv/template.tex)
tex file provided by `moderncv` maintainers.


**Implemented by:**

* [M.Mucahid Benlioglu](https://github.com/mbenlioglu)

## Building
#### Prerequisites:

- [CMake](https://cmake.org/) (> v3.10)
- [LaTeX](https://www.latex-project.org/get/)
- [moderncv](https://ctan.org/pkg/moderncv)
	
```
	# Can be installed with the following command
	$ tlmgr install moderncv
```

For building the project simply execute the following commands.
	
	$ cd build/
	$ cmake .. && make

This will output the compiled pdf files of the currently configured CV/resume in `build` directory.


# Documenting code

## In-code

why, purpose

Maybe not, use version control instead:
* zombie code

```
# Do not run this code!:
# if temperature > 0:
#     print('It is warm')
```

* version history 

```
# removed on August 5
# if() ...
# Now it connects to the API with o-auth2, updated 05/05/2016
```

Docstrings

Good docstrings describe:

    What the function does

    What goes in (including the type of the input variables)

    What goes out (including the return type)



Naming is documentation!

## README


As a bare minimum a README file should include:

* A descriptive project title
* Motivation (why the project exists) and basics
* Installation / How to setup
* Copy-pastable quick start code example
* Usage reference (if not elsewhere)
* Recommended citation if someone uses it
* Other related tools (“see also”)

## External documentation

static site generators build websites out of plain text files

docstrings can automatically be integrated into documentation

Quickstart example: https://coderefinery.github.io/documentation/sphinx/#exercise-sphinx-basics

Sphinx + Readthedocs: https://sphinx-rtd-tutorial.readthedocs.io/en/latest/index.html

Github pages


## References and Resources

This material is based on CodeRefinery Documentation lesson: https://coderefinery.github.io/documentation/ and licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

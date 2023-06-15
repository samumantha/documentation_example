# Documenting code

Materials for workshop on "Best practice guide for software developers and scientists in Extremes DT and Climate DT" in June 2023

Samantha Wittke, CSC - IT center for science

## ❓ Why?

* You will probably use your code in the future and may forget details.
* You may want others to use your code (almost impossible without documentation).
* You may want others to contribute to the code.
* Shield your limited time and let the documentation answer FAQs.


## 🗒️ Common parts

A checklist, if you want :)

* Purpose
* Authors
* License
* Recommended citation
* Copy-paste-able example to get started
* Dependencies and their versions or version ranges
* Installation instructions
* Tutorials covering key functionality
* Reference documentation (e.g. API) covering all functionality
* How do you want to be asked questions (mailing list or forum or chat or issue tracker)
* Possibly a FAQ section
* Contribution guide


## 🧐 In-code

### Comments

Describing **why** this piece of code is there, i.e. its **purpose**.

Comments that can be replaced by version control:
* keeping **zombie code**

```
# Do not run this code!:
# if temperature > 0:
#     print('It is warm')
```

* documenting **version**

```
# removed on August 5
# if() ...
# Now it connects to the API with o-auth2, updated 05/05/2016
```

> ➕ : close to code, ➖: too close to code

### Docstrings

```
def my_function(argument):
    """Summary or description of the function

    Parameters:
    argument (int): Description of argument

    Returns:
    int: Description of return value

   """

    return argument

print(some_function.__doc__)
```

Good docstrings describe:
* What the function does
* What goes in (including the type of the input variables)
* What goes out (including the return type)


> Good variable/function naming is documentation!


## ❗ README

... usually the first thing someone visiting your repository sees -> First impression!

A minimal README should include:

* A descriptive project title
* Motivation (why the project exists) and basics
* Installation / How to setup
* Copy-pastable quick start code example
* Usage reference (if not elsewhere)
* Recommended citation if someone uses it
* Other related tools (“see also”)

> often a README is enough!

## 🤓 External documentation

...When README is not enough...

**Static site generators** build websites out of plain text files (often `.md` or `.rst`).

**Docstrings can automatically be integrated into documentation**, no need to write this twice!

[Sphinx Quickstart example](https://coderefinery.github.io/documentation/sphinx/#exercise-sphinx-basics)

[Sphinx + Readthedocs](https://sphinx-rtd-tutorial.readthedocs.io/en/latest/index.html)

[Sphinx + GithubPages + Github actions](https://coderefinery.github.io/documentation/gh_workflow/)


## 🏡 Take home messages

I hope you latest now
* Understand the importance of writing code documentation together with the source code
* Know what makes a good documentation
* Know what tools can be used for writing documentation
* Are able to motivate a balanced decision: sometimes READMEs are absolutely enough


## 🐹 References and Resources

This material is based on CodeRefinery Documentation lesson: https://coderefinery.github.io/documentation/ and licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)

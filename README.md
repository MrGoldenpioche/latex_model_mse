
# Template-LaTeX

LaTeX template for MSE semester, deepening project, thesis reports.

## Getting Started

This template provides a LaTeX class which simply replaces and extends the standard directive `report`.

### Without Git
This template is based on (https://github.com/njakob/template-latex/releases) and modified for my needs. Thanks to Nicolas Jakob

This updated model is available at (https://github.com/gremaudc/latex_model_mse) (here :-))

### What's new ?
The main differences with this of Nicolas Jakobs are:

- Added new type of report (deepening)
- Remove tab space when start a new paragraph with "\\" latex command. Just comment "\usepackage[parfill]{parskip}" in "/template-latex/mse-thesis.cls" if you don't want this feature
- Add a new bibliography backend "bibtex8" instead of "biber" for compatibility problem. The old option is just commented
- Add new command to add glossary and acronyms (\insertglossary)
- Modified structure example to match with the most frequent MSE report structure
- Add example using dirtree package for CD-ROM listing

*It is recommended that you configure your workspace as shown below, then it will be easy to keep it updated.*

### Clone this Repository

Create a new folder for your report, then run git clone command.

```shell
$ git clone git@github.com:gremaudc/latex_model_mse.git
```

Now you can start to write your report in `thesis.tex`.

### Setup your Own Repository

Create a new folder for your report, and then initialize your repository as usual.

```shell
$ git init
$ git remote add origin <remote-location-of-your-git>
```

Now you can start to write your report in `thesis.tex`.

## Options

Different options can be defined for the document class.

### Confidential

Type: `Boolean` Default: False

Place a confidential marker on the first page.

### Lang

Type: `String` Default: `en`
Accept: `fr`, `en`

Language of your document.

### Major

Type: `String` Default: `tin`
Accept: `tic`, `tin` 

Define your major, `tic` for *Information and Communication Technologies* or `tin` for *Industrial Technologies*.

### Path

Type: `String`

Path to this document class.

### Type

Type: `String` Default: `thesis`
Accept: `semester`, `thesis`, `deepening`

Define whether it is a semester project, thesis, or a deepening project (PA).

## Metadata

Some metadata listed below must be provided to the document class.

### Advisor

Advisor of your project, it is usually the same person as `\professor`.

Example: `\advisor{Prof. John Doe}`

### Author

Your full name.

Example: `\author{Cyrill Gremaud}`

### Contact

Your e-mail address.

Example: `\contact{gremaudc@gmail.com}`

### Expert

Name and contact information of your expert(s).

Example:
```latex
\expert{
   Prof. John Doe
   \institute{HES-SO}
   \email{john.doe@nowhere.com}
}
```

### HeadOfMSE

Name of Head of MSE.

Example: `\headofmse{Fariba Moghaddam Bützberger}`

### Location

*Optional*

When you are abroad, place the information about the school or institute where you have done your work.

Example:
```latex
\location{
   Institute which is aboard
   \institute{HES-SO}
}
```

### Title

Title of your report.

Example: `\title{\LaTeX\ Model MSE}`

### Professor

Professor(s) who follow your research.

Example:
```latex
\professor{
   Prof. John Doe
   \institute{HES-SO}
   \email{john.doe@nowhere.com}
   \and
   Prof. John Doe
   \institute{HES-SO}
   \email{john.doe@nowhere.com}
}
```

### ProposedBy

Person or company who proposed the subject of your work.

Example:
```latex
\proposedby{
   Nicolas Jakob
   \institute{HES-SO}
   \email{nicolas.jakob@master.hes-so.ch}
}
```

### Supervisor

*Optional*

When you are abroad, place information about the person following your research.

Example:
```latex
\supervisor{
   Prof. John Doe
   \institute{HES-SO}
   \email{john.doe@nowhere.com}
}
```

### Version

Keep track of the published version of your document.

Example: `\version{Version 1}`

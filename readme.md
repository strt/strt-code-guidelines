# Strateg code of conduct

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Contents

- [Git](#git)
- [JavaScript](#javascript)
- [(S)CSS](#scss)
- [PHP](#php)
  - [Kodstandard](#kodstandard)
  - [Kodstil](#kodstil)
  - [Kontrollstruktur](#kontrollstruktur)
  - [Autoloading](#autoloading)
  - [HTTP-Message](#http-message)
  - [Dokumentering](#dokumentering)
- [SiteVision](#sitevision)
  - [Dokumentering](#dokumentering-1)
  - [Kodstil](#kodstil-1)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Git
+ `kebab-case` repository names with year suffix if it's a client project, e.g. `boilerplate` or `svebio-2016`
+ Commit often and after each added/updated feature
+ Don't push broken code
+ Write present-tense, imperative-style commit messages. `Add`, `Fix`, `Refactor` etc
+ Every project should contain a readme that describes how to set-up the project  

## JavaScript
Use [eslint](https://github.com/eslint/eslint) with the [Airbnb](https://github.com/airbnb/javascript) preset

## (S)CSS
- Use [BEM](http://getbem.com/introduction/)
- Use [stylelint](https://github.com/stylelint/stylelint) and the [stylelint-config-strateg](https://github.com/strt/stylelint-config-strateg) preset
- `camelCase` class names. Use `.searchBar` not `.search-bar`
- Don't use id selectors
- Only nest BEM elements one level. Use `.nav__item` not `.nav__list__item`
- Place BEM modifiers at the bottom of the selector
- Place media queries at the bottom of the current selector but before BEM modifiers

## PHP
### Kodstandard
* Use the full '<?php ?>' tag instead of smaller '<? ?>'
* Always use UTF-8 encoding
* Files should only define classes, functions, or produce content. But not both.
* Namespacing shall follow the PSR-standard.
* Classes should be written in a PascalCase manner.
* Constants should be capitalized and seperated with an underscore.
* Methods must be written in camelCase.
* Variables and properties must be written in camelCase.

### Kodstil
* A tab is four spaces.
* A soft line is 80 characters.
* A hard line is 120 characters.
* A newline after end of namespace and use statements.
* Curly bracets are opened on a new line when writing functions or methods.
* Visibility must be given on all properties and methods.
* True, false and null must be lowercase.
* Extend and implement must be on the same line as the class name.
* Properties and methods should not be prefixed with one or several underscores.
* Methods should not include a spacing between method name and parenthesis.
* If the method name and its arguments exeeds the soft or hard line, make a new line for each argument.
* Abstract and final keywords must be set before visibility.
* Static keyword must come after visibility.
* There should be no spacing before the first and after the last argument in a method or function.

### Kontrollstruktur
* Elseif should not contain spaces.
* A switch statement must not contain comments that refers to pieces of code further down.
* A foreach does not need to include both key and value variables.
* In unstable operations, always use a try/catch.

### Autoloading
* See www.php-fig.org

### HTTP-Message
* When applicable use HTTP codes as much as you can.
* see www.php-fig.org

### Dokumentering
* Should follow the standard set by PHPDoc.
* A block of documentation should always have a author, param and return tag if applicable.
* A block for methods and functions should always exist.
* Inline comments are not needed for all lines.

## SiteVision
### Dokumentering
* Ska följa standarden enligt [jsdoc](http://usejsdoc.org/)
* En scriptmodul ska alltid i toppen ha ett block med author, description och versionsnummer av SV.

### Kodstil
* Använd endast det officiella publika API:et.
* All kod ska wrappas i en self-invoking function.

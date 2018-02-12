# Awesome Linters
> A curated list of awesome linters.

Code linters are programs that performs static analysis on your code. They check your code for common mistakes and bad coding style/practices thus helping you catch errors before compilation/interpretation and forcing you and your team to keep a consistent code style within a project.

Most of the linters in this list have plugins available for popular text editors and IDEs and are pretty easy to setup and automate (via a pre-commit hook or a CI service for example).

This project is not closed to actual static analyzers. With this repository we intend to have an information resource for all things related to static analysis of code. By this, we mean that articles, talks or any other resource related to this topic will be welcome as well as links related to actual linters.

## Contents

- [Linters](#linters)

  - [Language Agnostic](#language-agnostic)
  - [Awesome Lists](#awesome-lists)
  - [C](#c)
  - [CoffeeScript](#coffeescript)
  - [C++](#c-1)
  - [CSS](#css)
  - [Dart](#dart)
  - [English](#english)
  - [Erlang](#erlang)
  - [Go](#go)
  - [Haskell](#haskell)
  - [Haxe](#haxe)
  - [HTML](#html)
  - [Java](#java)
  - [JavaScript](#javascript)
  - [Lua](#lua)
  - [Markdown](#markdown)
  - [npm](#npm)
  - [Objective-C](#objective-c)
  - [PHP](#php)
  - [Polymer](#polymer)
  - [Pug](#pug)
  - [Puppet](#puppet)
  - [Python](#python)
  - [reStructuredText](#restructuredtext)
  - [Ruby](#ruby)
  - [Rust](#rust)
  - [Sass](#sass)
  - [Scala](#scala)
  - [Shell](#shell)
  - [Swift](#swift)
  - [TypeScript](#typescript)

- [Contribution Guidelines](#contributing)

- [Contributors](#contributors)

## Linters

### Language Agnostic

- [coala](https://github.com/coala-analyzer/coala) - Language agnostic linter based on rules and standards. Written in Python.

### Awesome Lists

- [awesome-lint](https://github.com/sindresorhus/awesome-lint) - Linter for Awesome lists. Helps to createa and maintain Awesome lists. Written in Javascript.

### C

- [oclint](https://github.com/oclint/oclint) - Static analysis for C, C++ and Objective-C. Written in C++.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Source code beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA.

### CoffeeScript

- [coffeelint](https://github.com/clutchski/coffeelint) - Configurable linter written in CoffeScript to analyze CoffeScript.

### C++

- [oclint](https://github.com/oclint/oclint) - Static analysis for C, C++ and Objective-C. Written in C++.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Source code beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA.

### CSS

- [csslint](https://github.com/CSSLint/csslint) - CSS static analysis written in Javascript. Uses pluggable rules.
- [csscomb](https://github.com/csscomb/csscomb.js) - CSS tool that beautifies CSS based on a configuration. Helps with keeping CSS consistent. Written in Javascript.
- [ie8linter](https://github.com/israelidanny/ie8linter) - Static analysis for Internet Explorer 8 compatibility. Written in Javascript.
- [postcss-bem-linter](https://github.com/postcss/postcss-bem-linter) - A plugin for PostCSS to lint CSS according to _BEM-style_. Written in Javascript.
- [stylelint](http://stylelint.io) - CSS linter that is unopinionated, supports plugins and has a wide range of rules built-in. Written in Javascript.

### Dart

- [linter](https://github.com/dart-lang/linter)  - Linter for Dart mostly focused on style lints. It's configurable but comes with configured rules out of the box. Written in Dart.

### English

- [alex](https://github.com/wooorm/alex) - Linter to help catch insensitive writing in English. Written in Javascript.
- [proselint](https://github.com/amperser/proselint) - Linter for English that provides guidelines to make better writing. It has plugins for several editors and is configurable.

### Erlang

- [elvis](https://github.com/inaka/elvis) - Configurable Erlang linter written in Erlang.

### Go

- [golint](https://github.com/golang/lint) - Go style linter written in Go. Focus with coding styles more than with correctness.
- [gometalinter](https://github.com/alecthomas/gometalinter) - Concurrently run Go lint tools and normalise their output.
- [go vet](https://golang.org/cmd/vet/) - Examines Go source code and reports suspicious constructs.

### Haskell

- [hlint](https://github.com/ndmitchell/hlint) - Tool for suggesting possible improvements to Haskell code. These suggestions include ideas such as using alternative functions, simplifying code and spotting redundancies.

### Haxe

- [haxe-checkstyle](https://github.com/HaxeCheckstyle/haxe-checkstyle) - Haxe Checkstyle is a static analysis tool to help developers write Haxe code that adheres to a coding standard.

### HTML

- [htmlhint](https://github.com/yaniswang/HTMLHint) - HTMLHint is a Static Code Analysis Tool for HTML, you can use it with IDE or in build system.
- [bootlint](https://github.com/twbs/bootlint) - Bootlint is a tool that checks for several common HTML mistakes in webpages that are using Bootstrap.

### Java

- [checkstyle](https://github.com/checkstyle/checkstyle) - Checkstyle is a development tool to help programmers write Java code that adheres to a coding standard.
- [findbugs](http://findbugs.sourceforge.net) - Uses static analysis to look for bugs in Java code.
- [pmd](http://pmd.github.io) - Static analyzer that finds common programming flaws. It supports Java, JavaScript, Salesforce.com Apex, PLSQL, Apache Velocity, XML, XSL.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Source code beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA.

### JavaScript

- [clinton](https://github.com/SamVerschueren/clinton) - JavaScript project style linter.
- [eslint](https://github.com/eslint/eslint) - Fully pluggable tool for identifying and reporting on patterns in JavaScript.
- [jshint](https://github.com/jshint/jshint) - Community-driven tool that detects errors and potential problems in JavaScript code.
- [prettier](https://github.com/jlongster/prettier) - Opinionated JavaScript formatter inspired by refmt with advanced support for language features from ES2017, JSX, and Flow.
- [standard](https://github.com/feross/standard) - Javascript style linter that allows no configuration.
- [xo](https://github.com/sindresorhus/xo) - Opinionated but configurable ESLint wrapper with lots of goodies included. Enforces strict and readable code.

### Lua

- [lualint](https://github.com/philips/lualint) - lualint performs luac-based static analysis of global variable usage in Lua source code.

### Markdown

- [markdownlint](https://github.com/DavidAnson/markdownlint) - Node.js style checker and lint tool for Markdown/CommonMark files.
- [mdl](https://github.com/mivok/markdownlint) - Check markdown files and flag style issues. Written in ruby and is distributed as a rubygem.
- [remark-lint](https://github.com/wooorm/remark-lint) - Written in Javascript. remark-lint provides configurable Markdown style linting.

### npm

- [npm-package-json-lint](https://github.com/tclindner/npm-package-json-lint) - Configurable linter to enforce standards in npm package.json files.

### Objective-C

- [oclint](https://github.com/oclint/oclint) - Static source code analysis tool to improve quality and reduce defects for C, C++ and Objective-C. Written in C++.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Source code beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA.

### PHP
- [phplint](https://www.npmjs.com/package/phplint) - A node wrapper around the native php linter that allows for parallel linting and integration with build systems like Grunt, Gulp and more.

### Polymer

- [polylint](https://github.com/PolymerLabs/polylint) - Catch errors in your polymer project before even running your code. Written in TypeScript.

### Pug

- [pug-lint](https://github.com/pugjs/pug-lint) — An unopinionated and configurable linter and style checker for Pug (formerly Jade)

### Puppet

- [puppet-lint](https://github.com/rodjek/puppet-lint) - Test modules and manifests against the recommended Puppet style guidelines from the Puppet Labs style guide. Written in Ruby.

### Python

- [flake8](https://github.com/PyCQA/flake8) - Runs PyFlakes, pycodestyle and other tools from only one CLI. Written in Python.
- [pycodestyle (formerly called pep8)](https://github.com/PyCQA/pycodestyle) - Tool to check your Python code against some of the style conventions in PEP 8.
- [pylint](https://github.com/PyCQA/pylint) - Source code analyzer which looks for programming errors, helps enforcing a coding standard and sniffs for some code smells.

### reStructuredText

- [reStructuredText Lint](https://github.com/twolfson/restructuredtext-lint) - Validate reST files either as a module or from a CLI utility. Written in Python.


### Ruby

- [rubocop](https://github.com/bbatsov/rubocop) - Ruby static code analyzer. Out of the box it will enforce many of the guidelines outlined in the community Ruby Style Guide.

### Rust

- [rust-clippy](https://github.com/Manishearth/rust-clippy) - Collection of lints to catch common mistakes and improve your Rust code.

### Sass

- [sass-lint](https://github.com/sasstools/sass-lint) - Node-only Sass linter for both sass and scss syntax.
- [scss-lint](https://github.com/causes/scss-lint) - Tool to help keep your SCSS files clean and readable by running it against a collection of configurable linter rules.

### Scala

- [linter](https://github.com/HairyFotr/linter) - Scala static analysis compiler plugin which adds compile-time checks for various possible bugs, inefficiencies, and style problems.
- [scalastyle](http://www.scalastyle.org) -  Examines your Scala code and indicates potential problems with it. Similar to Checkstyle for Java.
- [scapegoat](https://github.com/sksamuel/scapegoat) - Another similar tool to Checkstyle for Java. Flags suspicious language usage in code.
- [wartRemover](http://github.com/puffnfresh/wartremover) - Flexible and configurable Scala linter written in Scala.

### Shell

- [shellcheck](https://github.com/koalaman/shellcheck) - Gives warnings and suggestions for bash/sh shell scripts.

### Swift

- [swiftlint](https://github.com/realm/SwiftLint) - Tool to enforce Swift style and conventions, loosely based on GitHub's Swift Style Guide.

### TypeScript

- [tslint](https://github.com/palantir/tslint) - Customizable TypeScript linter with automatic fixing of formating and style violations.

## Contributing

Contributions are very welcome! Create a new pull request, solve a bug or grab an issue that is currently unassigned!

The only rule is: [keep it organized](https://github.com/CarameloMartins/awesome-lint/blob/master/CONTRIBUTING.md).

## Contributors

Thanks to [everyone](https://github.com/caramelomartins/awesome-lint/graphs/contributors) that helped!

## License

[unlicense](LICENSE.md)

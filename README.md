# Awesome Linters

> A community-driven list of awesome linters.

Code linters are programs that performs static analysis on your code. They check
your code for common mistakes and bad coding style/practices thus helping you
catch errors before compilation/interpretation and forcing you and your team to
keep a consistent code style within a project.

Most of the linters in this list have plugins available for popular text editors
and IDEs and are pretty easy to setup and automate (via a pre-commit hook or a
CI service for example).

This project is not closed to actual static analyzers. With this repository we
intend to have an information resource for all things related to static analysis
of code. By this, we mean that articles, talks or any other resource related to
this topic will be welcome as well as links related to actual linters.

## Contents

- [Linters](#linters)

  - [Language Agnostic](#language-agnostic)
  - [Ansible](#ansible)
  - [Awesome Lists](#awesome-lists)
  - [C/C++](#cc)
  - [CoffeeScript](#coffeescript)
  - [Crystal](#crystal)
  - [CSS](#css)
  - [Dart](#dart)
  - [Dockerfile](#dockerfile)
  - [Elixir](#elixir)
  - [Elm](#elm)
  - [English](#english)
  - [Env](#env)
  - [Erlang](#erlang)
  - [Go](#go)
  - [GraphQL](#graphql)
  - [Haskell](#haskell)
  - [Haxe](#haxe)
  - [HTML](#html)
  - [Java](#java)
  - [JavaScript](#javascript)
  - [Kotlin](#kotlin)
  - [Lua](#lua)
  - [Markdown](#markdown)
  - [npm](#npm)
  - [Objective-C](#objective-c)
  - [Perl](#perl)
  - [PHP](#php)
  - [Polymer](#polymer)
  - [Pug](#pug)
  - [Puppet](#puppet)
  - [Python](#python)
  - [reStructuredText](#restructuredtext)
  - [Ruby](#ruby)
  - [Rust](#rust)
  - [SaltStack](#saltstack)
  - [Sass](#sass)
  - [Scala](#scala)
  - [Shell](#shell)
  - [Swift](#swift)
  - [TypeScript](#typescript)
  - [YAML](#yaml)

- [Contribution Guidelines](#contributing)

- [Contributors](#contributors)

## Linters

### Language Agnostic

- [coala](https://github.com/coala-analyzer/coala) - Language agnostic linter
  based on rules and standards. Written in Python.
- [commitlint](https://github.com/conventional-changelog/commitlint) -
  commitlint checks if your commit messages meet the
  [conventional commit format](https://conventionalcommits.org).
- [tidyall](https://metacpan.org/release/Code-TidyAll) - an all-in-one code
  tidier and validator with many available backends, caching,
  filtering-by-paths, and some other features.
- [violations-lib](https://github.com/tomasbjerre/violations-lib) - a library
  for parsing reports from static code analyzers. Can be used with Jenkins,
  Gradle, Maven and command line tools.

### Ansible

- [ansible-lint](https://github.com/ansible/ansible-lint) - Checks playbooks for
  practices and behaviour that could potentially be improved

### Awesome Lists

- [awesome-lint](https://github.com/sindresorhus/awesome-lint) - Linter for
  Awesome lists. Helps to create and maintain Awesome lists. Written in
  JavaScript.

### C/C++

- [clang-format](https://clang.llvm.org/docs/ClangFormat.html) - Formats C/C++
  code according to a coding style (Google, LLVM, Mozilla, Webkit, and Chromium
  available)
- [clang-tidy](https://clang.llvm.org/extra/clang-tidy/) - A clang-based C/C++
  linter tool to provide an extensible framework for diagnosing and fixing
  typical programming errors
- [cppcheck](http://cppcheck.sourceforge.net/) - Cppcheck is a static analysis
  tool for C/C++ code. It provides unique code analysis to detect bugs and
  focuses on detecting undefined behaviour and dangerous coding constructs. The
  goal is to detect only real errors in the code (i.e. have very few false
  positives).
- [oclint](https://github.com/oclint/oclint) - Static analysis for C, C++ and
  Objective-C. Written in C++.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Source code
  beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA.

### CoffeeScript

- [coffeelint](https://github.com/clutchski/coffeelint) - Configurable linter
  written in CoffeScript to analyze CoffeScript.

### Crystal

- [ameba](https://github.com/crystal-ameba/ameba) - Static code analysis tool
  for Crystal.

### CSS

- [csslint](https://github.com/CSSLint/csslint) - CSS static analysis written in
  JavaScript. Uses pluggable rules.
- [csscomb](https://github.com/csscomb/csscomb.js) - CSS tool that beautifies
  CSS based on a configuration. Helps with keeping CSS consistent. Written in
  JavaScript.
- [ie8linter](https://github.com/israelidanny/ie8linter) - Static analysis for
  Internet Explorer 8 compatibility. Written in JavaScript.
- [postcss-bem-linter](https://github.com/postcss/postcss-bem-linter) - Plugin
  for PostCSS to lint CSS according to _BEM-style_. Written in JavaScript.
- [stylelint](http://stylelint.io) - CSS linter that is unopinionated, supports
  plugins and has a wide range of rules built-in. Written in JavaScript, it
  parses by default CSS-like syntaxes such as SCSS, Sass, Less and SugarSS.

### Dart

- [linter](https://github.com/dart-lang/linter) - Linter for Dart mostly focused
  on style lints. It's configurable but comes with configured rules out of the
  box. Written in Dart.

### Dockerfile

- [dockerfile_lint](https://github.com/projectatomic/dockerfile_lint) - Rule
  based linter for Dockerfiles. The linter rules can be used to check file
  syntax as well as arbitrary semantic and best practice attributes determined
  by the rule file writer. The linter can also be used to check LABEL rules
  against docker images.
- [Dockerfilelint](https://github.com/replicatedhq/dockerfilelint)
  Dockerfilelint is a node module that analyzes a Dockerfile and looks for
  common traps, mistakes and helps enforce best practices
- [Dockerlint](https://github.com/RedCoolBeans/dockerlint) Linting tool for
  Dockerfiles based on recommendations from Dockerfile Reference and Best
  practices for writing Dockerfiles as of Docker 1.6.
- [hadolint](https://github.com/hadolint/hadolint) - Linter for Dockerfiles. The
  linter is parsing the Dockerfile into an AST and performs rules on top of the
  AST. It is standing on the shoulders of ShellCheck to lint the Bash code
  inside RUN instructions.

### Elixir

- [credo](https://github.com/rrrene/credo) - Static code analysis tool for the
  Elixir language with a focus on code consistency and teaching.

### Elm

- [elm-review](https://github.com/jfmengels/elm-review) - Analyzes whole Elm
  projects, with a focus on shareable and custom rules written in Elm that add
  guarantees the Elm compiler doesn't give you.

### English

- [alex](https://github.com/wooorm/alex) - Linter to help catch insensitive
  writing in English. Written in JavaScript.
- [proselint](https://github.com/amperser/proselint) - Linter for English that
  provides guidelines to make better writing. It has plugins for several editors
  and is configurable.
- [textlint](https://textlint.github.io/) - The pluggable linting tool for
  natural language texts.

### Env

- [dotenv-linter](https://github.com/mgrachev/dotenv-linter) - Linter for `.env`
  files.

### Erlang

- [elvis](https://github.com/inaka/elvis) - Configurable Erlang linter written
  in Erlang.

### Go

- [golangci-lint](https://github.com/golangci/golangci-lint) - Linters Runner
  for Go. 5x faster than gometalinter. Nice colored output. Can report only new
  issues. Fewer false-positives. Yaml/toml config.
- [golint](https://github.com/golang/lint) - Go style linter written in Go.
  Focus with coding styles more than with correctness.
- [gometalinter](https://github.com/alecthomas/gometalinter) - Concurrently run
  Go lint tools and normalise their output.
- [go vet](https://golang.org/cmd/vet/) - Examines Go source code and reports
  suspicious constructs.

### GraphQL

- [graphql-schema-linter](https://github.com/cjoudrey/graphql-schema-linter) -
  Validate GraphQL schema definitions against a set of rules.

### Haskell

- [hlint](https://github.com/ndmitchell/hlint) - Tool for suggesting possible
  improvements to Haskell code. These suggestions include ideas such as using
  alternative functions, simplifying code and spotting redundancies.

### Haxe

- [haxe-checkstyle](https://github.com/HaxeCheckstyle/haxe-checkstyle) - Haxe
  Checkstyle is a static analysis tool to help developers write Haxe code that
  adheres to a coding standard.

### HTML

- [htmlhint](https://github.com/yaniswang/HTMLHint) - HTMLHint is a Static Code
  Analysis Tool for HTML, you can use it with IDE or in build system.
- [html-validate](https://html-validate.org) - Offline HTML5 validator.
  Validates either a full document or a smaller (incomplete) template.
- [bootlint](https://github.com/twbs/bootlint) - Bootlint is a tool that checks
  for several common HTML mistakes in webpages that are using Bootstrap.
- [jinjalint](https://github.com/motet-a/jinjalint) - A prototype linter which
  checks the indentation and the correctness of Jinja-like/HTML templates. Also
  supports Django Templates.

### Java

- [checkstyle](https://github.com/checkstyle/checkstyle) - Checkstyle is a
  development tool to help programmers write Java code that adheres to a coding
  standard.
- [findbugs](http://findbugs.sourceforge.net) - Uses static analysis to look for
  bugs in Java code.
- [pmd](http://pmd.github.io) - Static analyzer that finds common programming
  flaws. It supports Java, JavaScript, Salesforce.com Apex, PLSQL, Apache
  Velocity, XML, XSL.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Source code
  beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA.

### JavaScript

- [clinton](https://github.com/SamVerschueren/clinton) - JavaScript project
  style linter.
- [eslint](https://github.com/eslint/eslint) - Fully pluggable tool for
  identifying and reporting on patterns in JavaScript.
- [jshint](https://github.com/jshint/jshint) - Community-driven tool that
  detects errors and potential problems in JavaScript code.
- [prettier](https://github.com/jlongster/prettier) - Opinionated JavaScript
  formatter inspired by refmt with advanced support for language features from
  ES2017, JSX, and Flow.
- [putout](https://github.com/coderaiser/putout) - Linter that fixes everything
  it can find, supports JS/TS/Flow and wrap ESLint (when `eslintrc` exists).
- [standard](https://github.com/feross/standard) - JavaScript style linter that
  allows no configuration.
- [xo](https://github.com/sindresorhus/xo) - Opinionated but configurable ESLint
  wrapper with lots of goodies included. Enforces strict and readable code.

### Kotlin

- [ktlint](https://github.com/pinterest/ktlint) - An anti-bikeshedding Kotlin
  linter with built-in formatter

### Lua

- [lualint](https://github.com/philips/lualint) - lualint performs luac-based
  static analysis of global variable usage in Lua source code.

### Markdown

- [markdownlint](https://github.com/DavidAnson/markdownlint) - Node.js style
  checker and lint tool for Markdown/CommonMark files.
- [mdl](https://github.com/mivok/markdownlint) - Check markdown files and flag
  style issues. Written in ruby and is distributed as a rubygem.
- [remark-lint](https://github.com/wooorm/remark-lint) - Written in JavaScript.
  remark-lint provides configurable Markdown style linting.

### npm

- [lockfile-lint](https://github.com/lirantal/lockfile-lint) - Lint an npm or
  yarn lockfile to analyze and detect security issues.
- [npm-package-json-lint](https://github.com/tclindner/npm-package-json-lint) -
  Configurable linter to enforce standards in npm package.json files.

### Objective-C

- [oclint](https://github.com/oclint/oclint) - Static source code analysis tool
  to improve quality and reduce defects for C, C++ and Objective-C. Written in
  C++.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Source code
  beautifier for C, C++, C#, ObjectiveC, D, Java, Pawn and VALA.

### OpenAPI (Swagger)

- [speccy](https://github.com/wework/speccy) - A handy toolkit for OpenAPI, with
  a linter to enforce quality rules.

### Perl

- [perlcritic](https://github.com/Perl-Critic) - The leading static analyzer for
  Perl. Configurable, extensible, powerful.
- [Perltidy](http://perltidy.sourceforge.net/) - a Perl code
  autoformatter/beautifier.

### PHP

- [phplint](https://www.npmjs.com/package/phplint) - Node wrapper around the
  native php linter that allows for parallel linting and integration with build
  systems like Grunt, Gulp and more.
- [PHP Mess Detector](https://github.com/phpmd/phpmd) - PHPMD can be seen as a
  user friendly and easy to configure frontend for the raw metrics measured by
  PHP Depend.

### Polymer

- [polylint](https://github.com/PolymerLabs/polylint) - Catch errors in your
  polymer project before even running your code. Written in TypeScript.

### Pug

- [pug-lint](https://github.com/pugjs/pug-lint) — An unopinionated and
  configurable linter and style checker for Pug (formerly Jade)

### Puppet

- [puppet-lint](https://github.com/rodjek/puppet-lint) - Test modules and
  manifests against the recommended Puppet style guidelines from the Puppet Labs
  style guide. Written in Ruby.

### Python

- [black](https://github.com/psf/black) - The uncompromising Python code
  formatter. Blackened code looks the same regardless of the project you're
  reading.
- [flake8](https://github.com/PyCQA/flake8) - Runs PyFlakes, pycodestyle and
  other tools from only one CLI. Written in Python.
- [pycodestyle (formerly called pep8)](https://github.com/PyCQA/pycodestyle) -
  Tool to check your Python code against some of the style conventions in PEP 8.
- [pylint](https://github.com/PyCQA/pylint) - Source code analyzer which looks
  for programming errors, helps enforcing a coding standard and sniffs for some
  code smells.
- [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide) -
  The strictest and most opinionated python linter ever.
- [yala](https://github.com/cemsbr/yala) - YALA combines many linters to improve
  the quality of your code.

### reStructuredText

- [doc8](https://launchpad.net/doc8) - Doc8 is an opinionated style checker for
  rst (with basic support for plain text) styles of documentation. Notice, it
  does not support additional sphinx extensions. Project is also available on
  [OpenStack](http://git.openstack.org/cgit/openstack/doc8/) or
  [GitHub](https://github.com/openstack/doc8)
- [reStructuredText Lint](https://github.com/twolfson/restructuredtext-lint) -
  Validate reST files either as a module or from a CLI utility. Written in
  Python.

### Ruby

- [rubocop](https://github.com/bbatsov/rubocop) - Ruby static code analyzer. Out
  of the box it will enforce many of the guidelines outlined in the community
  Ruby Style Guide.

### Rust

- [rust-clippy](https://github.com/Manishearth/rust-clippy) - Collection of
  lints to catch common mistakes and improve your Rust code.

### SaltStack

- [salt-lint](https://github.com/warpnet/salt-lint) - A command-line utility
  that checks for best practices in SaltStack.

### Sass

- [sass-lint](https://github.com/sasstools/sass-lint) - Node-only Sass linter
  for both sass and scss syntax.
- [scss-lint](https://github.com/causes/scss-lint) - Tool to help keep your SCSS
  files clean and readable by running it against a collection of configurable
  linter rules.
- [stylelint](http://stylelint.io) - CSS linter that is unopinionated, supports
  plugins and has a wide range of rules built-in. Written in JavaScript, it
  parses by default CSS-like syntaxes such as SCSS, Sass, Less and SugarSS.

### Scala

- [linter](https://github.com/HairyFotr/linter) - Scala static analysis compiler
  plugin which adds compile-time checks for various possible bugs,
  inefficiencies, and style problems.
- [scalastyle](http://www.scalastyle.org) - Examines your Scala code and
  indicates potential problems with it. Similar to Checkstyle for Java.
- [scapegoat](https://github.com/sksamuel/scapegoat) - Another similar tool to
  Checkstyle for Java. Flags suspicious language usage in code.
- [wartRemover](http://github.com/puffnfresh/wartremover) - Flexible and
  configurable Scala linter written in Scala.

### Shell

- [shellcheck](https://github.com/koalaman/shellcheck) - Gives warnings and
  suggestions for bash/sh shell scripts.
- [shfmt](https://github.com/mvdan/sh) - a shell (POSIX shell / bash / mksh)
  parser, formatter, and interpreter written in Go 1.13-and-above.

### Swift

- [swiftlint](https://github.com/realm/SwiftLint) - Tool to enforce Swift style
  and conventions, loosely based on GitHub's Swift Style Guide.

### TypeScript

- [tslint](https://github.com/palantir/tslint) - Customizable TypeScript linter
  with automatic fixing of formating and style violations.

### YAML

- [spectral](https://github.com/stoplightio/spectral) - A flexible JSON/YAML
  linter, with out of the box support for OpenAPI v2/v3 and AsyncAPI v2.
- [yamllint](https://github.com/adrienverge/yamllint) - Linter for YAML files.

## Contributing

Contributions are very welcome! Create a new pull request, solve a bug or grab
an issue that is currently unassigned!

The only rule is:
[keep it organized](https://github.com/CarameloMartins/awesome-lint/blob/master/CONTRIBUTING.md).

## Contributors

Thanks to
[everyone](https://github.com/caramelomartins/awesome-lint/graphs/contributors)
that helped!

## License

[unlicense](LICENSE.md)

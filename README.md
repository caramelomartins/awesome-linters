# Awesome Linters

> A community-driven list of awesome linters.

Code linters are programs that perform static analysis on your code. They check
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
  - [CSV](#csv)
  - [Dart](#dart)
  - [Dockerfile](#dockerfile)
  - [Elixir](#elixir)
  - [Elm](#elm)
  - [English](#english)
  - [Env](#env)
  - [EPUB](#epub)
  - [Erlang](#erlang)
  - [Go](#go)
  - [GraphQL](#graphql)
  - [Groovy](#groovy)
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
  - [Rego](#rego)
  - [reStructuredText](#restructuredtext)
  - [Ruby](#ruby)
  - [Rust](#rust)
  - [SaltStack](#saltstack)
  - [Sass](#sass)
  - [Scala](#scala)
  - [Shell](#shell)
  - [SQL](#sql)
  - [Swift](#swift)
  - [TypeScript](#typescript)
  - [YAML](#yaml)

- [Contribution Guidelines](#contributing)

- [Contributors](#contributors)

## Linters

### Language Agnostic

- [codespell](https://github.com/codespell-project/codespell) - Fast spell checker
for source code, identifiers, and comments with low false-positive rates.
- [commitlint](https://github.com/conventional-changelog/commitlint) - Checks if your
commit messages meet the [Conventional Commits](https://conventionalcommits.org) format.
- [editorconfig-checker](https://github.com/editorconfig-checker/editorconfig-checker) -
Fast tool written in Go to verify that files adhere to `.editorconfig` rules across any language.
- [MegaLinter](https://oxsecurity.github.io/megalinter) - Comprehensive CI linter
aggregator supporting 50+ languages, 20+ formats, and security scanners. Can automatically
 apply fixes via PR/commit.
- [pre-commit](https://github.com/pre-commit/pre-commit) - Multi-language framework for
managing and maintaining clean pre-commit hooks to automate linting workflows.
- [Semgrep](https://github.com/semgrep/semgrep) - Fast, lightweight, open-source static
analysis engine for enforcing code standards, bug detection, and security policies across
30+ languages using syntax-aware pattern matching.
- [tidyall](https://metacpan.org/release/Code-TidyAll) - All-in-one code tidier and
validator engine with caching, path filtering, and pluggable backends.
- [Trunk Check](https://github.com/trunk-io/trunk) - Blazingly fast meta-linter and
aggregator that manages and runs linters/formatters hermetically across any repo.
- [typos](https://github.com/crate-ci/typos) - Source code spell checker written in Rust;
optimized for minimal false positives on variable names and raw strings.
- [violations-lib](https://github.com/tomasbjerre/violations-lib) - Java library for parsing
diagnostic reports across 100+ static code analyzers for Jenkins, Maven, and CLI tools.
- [coala](https://github.com/coala-analyzer/coala) - *(⚠️ Inactive / Deprecated)*
Language-agnostic analysis framework based on customizable rules. Python 3.7 legacy ecosystem;
superseded by Semgrep and Trunk.
- [Scanmycode CE](https://github.com/marcinguy/scanmycode-ce) - *(⚠️ Stale / Low Maintenance)*
Code scanning / SAST aggregator web UI.

### Ansible

- [ansible-lint](https://github.com/ansible/ansible-lint) - Official linter checking
- playbooks, roles, and collections for syntax errors, deprecations, security flaws,
- and idiomatic best practices.
- [yamllint](https://github.com/adrienverge/yamllint) - General YAML linter commonly
paired with `ansible-lint` to validate strict structure, indentation, and trailing
spaces in Ansible configurations.

### Awesome Lists

- [awesome-lint](https://github.com/sindresorhus/awesome-lint) - Linter for Awesome
lists ensuring standard formatting, clean Markdown hierarchies, valid URLs, and list
consistency.

### C/C++

- [clang-format](https://clang.llvm.org/docs/ClangFormat.html) - Canonical Clang/LLVM
formatter supporting standard style guides (Google, LLVM, Mozilla, Chromium, Microsoft)
and granular `.clang-format` configurations.
- [clang-tidy](https://clang.llvm.org/extra/clang-tidy/) - LLVM-based linter and static
analyzer providing AST-level diagnostics, modernizing checks (C++11 to C++23),
bug pattern detection, and automatic fixes.
- [CodeChecker](https://github.com/Ericsson/codechecker) - Advanced static analysis
infrastructure wrapper around Clang Static Analyzer and Clang-Tidy with web reporting
and CI triage workflows.
- [cppcheck](https://cppcheck.sourceforge.io/) - Dedicated C/C++ static analysis engine
focused on undefined behavior, pointer issues, memory leaks, and logic flaws with a strict
focus on zero false positives.
- [cpplint](https://github.com/cpplint/cpplint) - Python CLI static checker strictly
enforcing the [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html).
*(Note: Primarily regex/token-based; lacks full AST semantics compared to Clang-Tidy).*
- [flawfinder](https://dwheeler.com/flawfinder/) - Lexical security scanner checking
C/C++ source code against Common Weakness Enumeration (CWE) databases for buffer overflows,
race conditions, and unsafe API usage.
- [IKOS](https://github.com/NASA-SW-VnV/ikos) - High-assurance static analyzer from
NASA based on Abstract Interpretation for proving the absence of runtime errors
(buffer overflows, division by zero, null pointer dereferences).
- [include-what-you-use](https://include-what-you-use.org/) - Clang-based tool analyzing
`#include` directives to eliminate redundant imports and ensure forward declarations or
required headers are explicitly referenced.
- [infer](https://fbinfer.com/) - Static analyzer from Meta supporting C, C++, Java,
and Objective-C; detects complex null-pointer dereferences, data races, memory corruption,
 and resource leaks via separation logic.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Highly configurable source
code beautifier and structural formatter supporting C, C++, C#, D, and Java.
- [oclint](https://oclint.org/) - *(⚠️ Inactive / Slow LLVM support)* Static analysis
engine for C, C++, and Objective-C inspecting ASTs for complexity smells and dead code.

### CoffeeScript

- [coffeelint](https://github.com/coffeelint/coffeelint) - *(⚠️ Legacy / Deprecated)*
Configurable style checker and linter written in CoffeeScript for CoffeeScript source
files.

### Crystal

- [ameba](https://github.com/crystal-ameba/ameba) - Standard AST-based static code
analysis tool and linter for Crystal, enforcing idioms, code smells, and performance
anti-patterns.
- `crystal tool format` - Built-in canonical formatter and syntax validator bundled
with the Crystal compiler toolchain.

### CSS

- [Biome](https://biomejs.dev/) - High-performance Rust-based toolchain providing
fast formatting and linting for CSS and modern web standards.
- [Lightning CSS](https://lightningcss.dev/) - Ultra-fast Rust-based CSS parser,
transformer, minifier, and structural validator.
- [postcss-bem-linter](https://github.com/postcss/postcss-bem-linter) - PostCSS plugin
validating that stylesheet selectors strictly adhere to BEM (Block Element Modifier)
architecture.
- [Prettier](https://prettier.io/) - Opinionated multi-format code formatter with complete
support for CSS, SCSS, and Less.
- [stylelint](https://stylelint.io/) - Industry standard, pluggable CSS/SCSS/Less linter.
Enforces conventions, avoids errors, and supports custom plugins and CSS modules.
- [csscomb](https://github.com/csscomb/csscomb.js) - *(⚠️ Unmaintained)* CSS formatter
and property sorter; superseded by Prettier and Stylelint plugins (e.g., `stylelint-order`).
- [csslint](https://github.com/CSSLint/csslint) - *(⚠️ Deprecated / Archived)* Legacy
 CSS static analysis engine; superseded by Stylelint.
- [ie8linter](https://github.com/israelidanny/ie8linter) - *(⚠️ Obsolete)*
Static analyzer for Internet Explorer 8 compatibility.

### CSV

- [csvclean](https://csvkit.readthedocs.io/en/latest/scripts/csvclean.html) -
Part of the Python `csvkit` suite; scans CSV files for malformed rows, syntax errors,
delimiter inconsistencies, and structural anomalies.
- [csvlint.rb](https://github.com/Data-Liberation-Front/csvlint.rb) - Ruby gem
validating CSV structure against the W3C CSV on the Web specifications and
standard RFC 4180 rules.
- [qsv validate](https://github.com/jqnatividad/qsv) - Ultra-fast Rust-based CSV
processor capable of validating structure, delimiter hygiene, and schema
compliance against JSON Schema.

### Dart

- [dart analyze](https://dart.dev/tools/dart-analyze) - Official Dart SDK static
  analysis command enforcing rules configured in `analysis_options.yaml`.
- [custom_lint](https://github.com/invertase/custom_lint) - Community framework
  for writing custom linter rules, diagnostics, and auto-fixes for Dart and
  Flutter projects.
- [linter](https://github.com/dart-lang/linter) - *(⚠️ Integrated)* Official
  Dart linter repository; now bundled and shipped directly within the Dart SDK.

### Dockerfile

- [hadolint](https://github.com/hadolint/hadolint) - Smarter Dockerfile linter
  that parses Dockerfiles into an AST and evaluates rules using `ShellCheck`
  to validate inline `RUN` shell scripts.
- [dockerfile_lint](https://github.com/projectatomic/dockerfile_lint) - *(⚠️
  Deprecated / Archived)* Red Hat / ProjectAtomic rule-based syntax and label
  checker.
- [Dockerfilelint](https://github.com/replicatedhq/dockerfilelint) - *(⚠️
  Unmaintained)* Node.js module checking Dockerfiles for common mistakes and
  anti-patterns.
- [Dockerlint](https://github.com/RedCoolBeans/dockerlint) - *(⚠️ Obsolete)*
  Legacy parser based on obsolete Docker 1.6 recommendations.

### Elixir

- [credo](https://github.com/rrrene/credo) - Static code analysis and linting
  tool for Elixir focusing on consistency, refactoring, and teaching idioms.
- [dialyxir](https://github.com/jeremyjh/dialyxir) - Mix tasks wrapping
  Erlang's Dialyzer to provide thorough static type analysis and discrepancy
  detection in Elixir.
- [sobelow](https://github.com/nccgroup/sobelow) - Security-focused static
  analysis tool designed specifically for the Phoenix framework ecosystem.

### Elm

- [elm-format](https://github.com/avh4/elm-format) - Canonical, zero-config
  formatter for Elm source files enforcing official community style rules.
- [elm-review](https://github.com/jfmengels/elm-review) - Extensible static
  analyzer examining entire Elm projects with user-defined and shareable AST
  rules.

### English

- [alex](https://github.com/wooorm/alex) - Linter that detects insensitive,
  inconsiderate, or gender-biased phrasing in markdown and prose.
- [proselint](https://github.com/amperser/proselint) - Command-line prose
  linter enforcing stylistic rules curated from world-class authors and editors.
- [textlint](https://textlint.github.io/) - Pluggable natural language linter
  supporting custom rules, presets, and AST parsing for Markdown and plain text.
- [Vale](https://github.com/errata-ai/vale) - Blazingly fast, syntax-aware
  linter for prose and technical documentation supporting custom style guides
  (Google, Microsoft, write-good).
- [write-good](https://github.com/btford/write-good) - Naive prose linter
  highlighting passive voice, duplicate words, and weasel words.

### Env

- [dotenv-linter](https://github.com/dotenv-linter/dotenv-linter) - Lightning-fast
  linter written in Rust to validate, sort, and standardize `.env` files.

### EPUB

- [EPUBCheck](https://github.com/w3c/epubcheck) - Official W3C validation
  utility testing conformance against EPUB 2 and EPUB 3 specifications.

### Erlang

- [dialyzer](https://www.erlang.org/doc/man/dialyzer.html) - Erlang's built-in
  Discrepancy Analyzer identifying type errors, dead code, and unreachable paths.
- [elvis](https://github.com/inaka/elvis) - Configurable Erlang style and
  convention linter enforcing uniform code layout.
- [rebar3_hank](https://github.com/AdRoll/rebar3_hank) - Rebar3 plugin acting
  as an aggressive dead-code cleaner and unused macro/record linter.

### Go

- [go vet](https://pkg.go.dev/cmd/vet) - Official Go toolchain analyzer
  inspecting source code for suspicious constructs and logic mistakes.
- [golangci-lint](https://github.com/golangci/golangci-lint) - High-speed Go
  linters aggregator running dozens of analyzers in parallel with caching and
  granular configuration.
- [govulncheck](https://pkg.go.dev/golang.org/x/vuln/cmd/govulncheck) - Official
  Go CLI tool detecting known security vulnerabilities via static call graph
  analysis.
- [revive](https://github.com/mgechev/revive) - Fast, highly configurable, and
  extensible drop-in replacement for the archived `golint`.
- [staticcheck](https://staticcheck.dev/) - Advanced Go static analysis engine
  employing SSA to detect bugs, dead branches, and performance regressions.
- [golint](https://github.com/golang/lint) - *(⚠️ Deprecated / Archived)*
  Legacy style linter archived by the Go team; superseded by `revive` and
  `staticcheck`.
- [gometalinter](https://github.com/alecthomas/gometalinter) - *(⚠️ Deprecated
  / Archived)* Predecessor linter runner; superseded by `golangci-lint`.

### GraphQL

- [@graphql-eslint/eslint-plugin](https://github.com/dimaMachina/graphql-eslint) -
  Modern ESLint plugin for GraphQL schemas and operations with AST validation
  and type-safety integration.
- [graphql-schema-linter](https://github.com/cjoudrey/graphql-schema-linter) -
  CLI utility validating GraphQL Schema Definition Language (SDL) files against
  enforceable schema design conventions.

### Groovy

- [CodeNarc](https://github.com/CodeNarc/CodeNarc) - Foundation static analysis
  engine for Groovy source code featuring hundreds of rules for defects,
  conventions, and complexity.
- [npm-groovy-lint](https://github.com/nvuillam/npm-groovy-lint) - Node-based
  wrapper providing linting, formatting, and auto-fixes for Groovy,
  Jenkinsfile, and Gradle files via CodeNarc.

### Haskell

- [hlint](https://github.com/ndmitchell/hlint) - Tool for suggesting code
  improvements, simplifying constructs, and eliminating redundancies in
  Haskell.
- [stan](https://github.com/kowainik/stan) - Static analysis tool for Haskell
  focusing on performance anti-patterns, modern idioms, and potential bugs.
- [weeder](https://github.com/ocharles/weeder) - Dead-code analysis utility
  detecting unused exports and unreferenced Haskell declarations.

### Haxe

- [haxe-checkstyle](https://github.com/HaxeCheckstyle/haxe-checkstyle) - Static
  analysis engine for Haxe enforcing community style guidelines and structural
  rules.

### HTML

- [djlint](https://github.com/djlint/djLint) - Modern HTML template linter and
  formatter supporting Jinja, Django, Nunjucks, Twig, Go Templates, and
  Handlebars.
- [html-validate](https://html-validate.org) - Offline HTML5 validator checking
  both complete documents and partial templates for accessibility and best
  practices.
- [HTMLHint](https://github.com/htmlhint/HTMLHint) - Pluggable static analysis
  tool for validating HTML standards in editors and CI pipelines.
- [LintHTML](https://github.com/linthtml/linthtml) - Active, community-driven
  fork of `htmllint` with pluggable rules.
- [markuplint](https://markuplint.dev/) - Highly extensible HTML linter with
  first-class support for raw HTML, JSX, Vue, Svelte, and web components.
- [Nu Html Checker](https://github.com/validator/validator/) - Official W3C
  offline validator for HTML5, CSS, and SVG documents written in Java.
- [bootlint](https://github.com/twbs/bootlint) - *(⚠️ Deprecated / Archived)*
  Legacy Bootstrap 3/4 HTML structure analyzer by the Bootstrap core team.
- [jinjalint](https://github.com/motet-a/jinjalint) - *(⚠️ Inactive /
  Prototype)* Experimental Jinja linter; superseded by `djlint`.

### Java

- [Checkstyle](https://github.com/checkstyle/checkstyle) - Highly configurable
  linter verifying adherence to Java coding conventions (Google/Sun style
  guides).
- [Error Prone](https://github.com/google/error-prone) - Compile-time static
  analysis engine from Google that hooks into `javac` to trap bug patterns as
  compiler errors.
- [PMD](https://pmd.github.io/) - Extensible multi-language static analyzer
  identifying bad practices, inefficient code, and duplicate logic in Java.
- [SpotBugs](https://github.com/spotbugs/spotbugs) - Active spiritual successor
  to FindBugs; analyzes Java bytecode to identify 400+ bug patterns and
  security vulnerabilities (often paired with Find Security Bugs).
- [uncrustify](https://github.com/uncrustify/uncrustify) - Configurable source
  code formatter and indenter supporting Java, C, C++, and C#.
- [FindBugs](http://findbugs.sourceforge.net) - *(⚠️ Deprecated / Archived)*
  Legacy bytecode static analysis tool; superseded by `SpotBugs`.

### JavaScript

- [Biome](https://biomejs.dev/) - High-performance Rust-based toolchain
  combining formatting and linting as a fast alternative to ESLint and Prettier.
- [ESLint](https://github.com/eslint/eslint) - Pluggable, industry-standard
  static analysis utility for JavaScript and JSX with support for the Flat
  Config system.
- [Oxlint](https://github.com/oxc-project/oxc) - Ultra-fast Rust-based linter
  designed to catch errors without configuration overhead, running 50-100x
  faster than ESLint.
- [Prettier](https://github.com/prettier/prettier) - Opinionated multi-language
  code formatter enforcing consistent code style across JavaScript, JSX, and
  modern web formats.
- [putout](https://github.com/coderaiser/putout) - Pluggable linter, transformer,
  and code refactoring engine capable of automatically fixing complex JS/TS AST
  issues.
- [quick-lint-js](https://quick-lint-js.com) - Zero-config, lightweight C++
  linter providing instantaneous error detection inside text editors.
- [Standard](https://github.com/standard/standard) - Zero-config JavaScript
  style linter and formatter enforcing standard rules.
- [XO](https://github.com/xojs/xo) - Opinionated, batteries-included ESLint
  wrapper enforcing strict and readable defaults without manual setup.
- [clinton](https://github.com/SamVerschueren/clinton) - *(⚠️ Unmaintained)*
  CLI tool for validating JavaScript package conventions and repository files.
- [JSHint](https://github.com/jshint/jshint) - *(⚠️ Legacy / Superseded)*
  Historical static analysis tool; superseded by ESLint and Biome.

### Kotlin

- [detekt](https://github.com/detekt/detekt) - Comprehensive AST static code
  analysis tool for Kotlin detecting code smells, complexity metrics, and
  performance anti-patterns.
- [ktfmt](https://github.com/facebook/ktfmt) - Facebook's deterministic Kotlin
  code formatter based on Google Java Format conventions.
- [ktlint](https://github.com/pinterest/ktlint) - Anti-bikeshedding Kotlin
  linter and formatter enforcing the official Kotlin coding conventions.

### Lua

- [luacheck](https://github.com/lunarmodules/luacheck) - Pluggable static
  analyzer and linter for Lua focusing on undefined global detection and code
  standards.
- [Selene](https://github.com/Kampfkarren/selene) - Modern, fast Lua linter
  written in Rust with detailed diagnostics and standard library awareness.
- [StyLua](https://github.com/JohnnyMorganz/StyLua) - Opinionated, highly
  performant Lua 5.1/5.2/5.3/5.4 and Luau code formatter written in Rust.
- [lualint](https://github.com/philips/lualint) - *(⚠️ Obsolete / Archived)*
  Legacy `luac`-based global variable scanner; superseded by `luacheck` and
  `selene`.

### Markdown

- [markdownlint](https://github.com/DavidAnson/markdownlint) - Node.js style
  checker and linter for Markdown/CommonMark documents with extensive rule
  customization.
- [markdownlint-cli2](https://github.com/DavidAnson/markdownlint-cli2) - Fast,
  modern CLI wrapper for `markdownlint` supporting globbing and configuration
  caching.
- [remark-lint](https://github.com/remarkjs/remark-lint) - Highly pluggable
  Markdown style linter powered by the unified / remark AST ecosystem.
- [mdl](https://github.com/markdownlint/markdownlint) - *(⚠️ Stale / Legacy)*
  Ruby gem linter for Markdown; superseded by David Anson's `markdownlint`.

### npm

- [arethetypeswrong](https://github.com/arethetypeswrong/arethetypeswrong.js) -
  CLI and linter to validate TypeScript declaration exports and module
  resolution formats in npm packages.
- [knip](https://github.com/webpro-nl/knip) - Fast analyzer detecting unused
  dependencies, unused exports, duplicate packages, and orphaned files in npm
  projects.
- [lockfile-lint](https://github.com/lirantal/lockfile-lint) - Security linter
  validating npm and Yarn lockfiles to catch compromised registries and package
  tampering.
- [npm-package-json-lint](https://github.com/tclindner/npm-package-json-lint) -
  Configurable linter enforcing conventions, required fields, and rules in
  `package.json` files.
- [publint](https://github.com/bluwy/publint) - Packaging linter ensuring npm
  packages are structured correctly for modern Node.js, ESM, and CJS runtimes.

### Objective-C

- [clang-format](https://clang.llvm.org/docs/ClangFormat.html) - Canonical LLVM
  formatter supporting Objective-C code formatting and indentation style rules.
- [infer](https://fbinfer.com/) - Static analyzer from Meta capable of detecting
  memory leaks, null pointer dereferences, and concurrency issues in
  Objective-C.
- [uncrustify](https://github.com/uncrustify/uncrustify) - Highly configurable
  source code formatter and beautifier supporting Objective-C.
- [oclint](https://oclint.org/) - *(⚠️ Inactive / Slow LLVM support)* Static
  analyzer inspecting Objective-C ASTs to detect dead code and code smells.

### OpenAPI (Swagger)

- [Redocly CLI](https://github.com/Redocly/redocly-cli) - Fast OpenAPI / AsyncAPI
  linter, validator, and documentation bundler supporting built-in rulesets and
  decorators.
- [Spectral](https://github.com/stoplightio/spectral) - Flexible, JSON/YAML and
  OpenAPI (v2/v3/v3.1) linter powered by customizable JSONPath rules.
- [vacuum](https://github.com/daveshanley/vacuum) - Blazingly fast OpenAPI
  linter and quality scoring tool written in Go, fully compatible with Spectral
  rulesets.
- [speccy](https://github.com/wework/speccy) - *(⚠️ Deprecated / Archived)*
  OpenAPI 3.0 linter previously maintained by WeWork; superseded by Spectral
  and Redocly.

### Perl

- [Perl::Critic](https://metacpan.org/dist/Perl-Critic) - Extensible and
  configurable static analysis engine enforcing best practices from the *Perl
  Best Practices* book.
- [Perl::Critic::Community](https://metacpan.org/dist/Perl-Critic-Community) -
  Modernized, community-maintained policies for Perl::Critic targeting modern
  Perl versions (5.20+).
- [Perltidy](https://perltidy.sourceforge.net/) - Standard Perl code
  autoformatter, indenter, and syntax beautifier.

### PHP

- [PHP-CS-Fixer](https://github.com/PHP-CS-Fixer/PHP-CS-Fixer) - Highly
  configurable coding standards fixer detecting and auto-correcting PHP style
  violations (PSR-12, PER-CS).
- [PHP_CodeSniffer](https://github.com/PHPCSStandards/PHP_CodeSniffer) - Tokenizes
  PHP files to detect and fix violations of defined coding standards (maintained
  by PHPCSStandards).
- [PHP Mess Detector](https://github.com/phpmd/phpmd) - Static analyzer detecting
  code smells, cyclomatic complexity, suboptimal code, and unused parameters in
  PHP.
- [PHPStan](https://github.com/phpstan/phpstan) - Leading industrial static
  analysis engine finding bugs, type discrepancies, and edge cases in PHP
  without writing tests.
- [Psalm](https://github.com/vimeo/psalm) - Advanced static analysis tool by
  Vimeo for identifying type issues, logic errors, and security vulnerabilities
  in PHP.
- [phplint](https://www.npmjs.com/package/phplint) - *(⚠️ Basic)* Node.js
  wrapper around `php -l` for parallel syntax checking; superseded by native
  analyzers like PHPStan.

### Polymer

- [lit-analyzer](https://github.com/runem/lit-analyzer) - CLI and language
  server linter checking type safety, bindings, and HTML syntax in modern
  Lit and Web Components.
- [polylint](https://github.com/PolymerLabs/polylint) - *(⚠️ Deprecated /
  Archived)* Legacy linter for Polymer projects; superseded by Lit and
  `lit-analyzer`.

### Pug

- [@prettier/plugin-pug](https://github.com/prettier/plugin-pug) - Opinionated
  code formatter for Pug templates within the Prettier ecosystem.
- [pug-lint](https://github.com/pugjs/pug-lint) - Configurable linter and
  style checker for Pug (formerly Jade) template files.

### Puppet

- [pdk validate](https://www.puppet.com/docs/pdk/latest/pdk_reference.html) -
  Built-in validation suite within the Puppet Development Kit (PDK) checking
  syntax, metadata, and style.
- [puppet-lint](https://github.com/puppetlabs/puppet-lint) - Standard style
  linter validating modules and manifests against official Puppet style
  recommendations.

### Python

- [Bandit](https://github.com/PyCQA/bandit) - Security-focused static analyzer
  designed to scan Python source code for common vulnerabilities (CWE mappings).
- [Black](https://github.com/psf/black) - Uncompromising, deterministic
  Python code formatter enforcing standard PEP 8 formatting conventions.
- [Flake8](https://github.com/PyCQA/flake8) - Modular CLI wrapper combining
  PyFlakes, pycodestyle, and McCabe complexity checks with a large plugin
  ecosystem.
- [Mypy](https://github.com/python/mypy) - Canonical optional static type
  checker for Python enforcing PEP 484 type annotations and preventing type
  bugs.
- [PyLint](https://github.com/pylint-dev/pylint) - Comprehensive static
  analyzer checking for logic errors, refactoring opportunities, and code
  smells.
- [Pyright / Basedpyright](https://github.com/microsoft/pyright) - Ultra-fast,
  spec-compliant static type checker and analyzer for Python written in
  TypeScript.
- [Ruff](https://github.com/astral-sh/ruff) - Extremely fast Python linter
  and formatter written in Rust; acts as a drop-in replacement for Flake8,
  isort, Black, and dozens of plugins with near-instant execution.
- [wemake-python-styleguide](https://github.com/wemake-services/wemake-python-styleguide) -
  Strict and opinionated Flake8 plugin enforcing granular stylistic and
  architectural constraints.
- [pycodestyle](https://github.com/PyCQA/pycodestyle) - *(⚠️ Integrated)*
  PEP 8 compliance checker; typically run via Flake8 or replaced by Ruff.
- [yala](https://github.com/cemsbr/yala) - *(⚠️ Stale / Low Maintenance)*
  Multi-linter aggregator CLI; superseded by Ruff and pre-commit hooks.

### Rego

- `opa check` - Built-in Open Policy Agent command validating syntax and
  structural integrity of Rego policies.
- [Regal](https://github.com/StyraInc/regal) - Modern, rule-based linter for
  Rego policy code catching bugs, style inconsistencies, and anti-patterns.

### reStructuredText

- [doc8](https://github.com/PyCQA/doc8) - Opinionated style and structure
  checker for rst documentation, maintained by PyCQA.
- [restructuredtext-lint](https://github.com/twolfson/restructuredtext-lint) -
  ReST validator using the Docutils parser, available as a Python module or
  CLI utility.
- [rstcheck](https://github.com/rstcheck/rstcheck) - Advanced validator and
  linter checking syntax across rst files and embedded code blocks (Python,
  JSON, YAML, Bash).

### Ruby

- [Brakeman](https://github.com/presidentbeef/brakeman) - Static analysis
  security vulnerability scanner designed specifically for Ruby on Rails
  applications.
- [RuboCop](https://github.com/rubocop/rubocop) - Extensible Ruby static code
  analyzer and code formatter enforcing community Ruby Style Guide conventions.
- [Standard Ruby](https://github.com/standardrb/standard) - Zero-config,
  opinionated Ruby style linter and automatic code formatter built on top of
  RuboCop.

### Rust

- [cargo-audit](https://github.com/rustsec/rustsec/tree/main/cargo-audit) -
  Audit `Cargo.lock` files against the RustSec Advisory Database for crates
  with reported security vulnerabilities.
- [cargo-deny](https://github.com/EmbarkStudios/cargo-deny) - Cargo plugin to
  lint dependency graphs for security advisories, forbidden licenses,
  duplicates, and source origins.
- [clippy](https://github.com/rust-lang/rust-clippy) - Official Rust compiler
  linter providing a collection of lints to catch common mistakes, performance
  traps, and anti-patterns.
- [rustfmt](https://github.com/rust-lang/rustfmt) - Official Rust toolchain
  formatter enforcing consistent code style guidelines across codebases.

### SaltStack

- [salt-lint](https://github.com/warpnet/salt-lint) - Command-line utility
  checking SaltStack state files (`.sls`) for style, syntax, and best practices.

### Sass

- [Prettier](https://prettier.io/) - Multi-format code formatter providing
  first-class formatting support for SCSS and Sass stylesheets.
- [stylelint](https://stylelint.io/) - Industry-standard linter supporting
  SCSS/Sass via plugins like `stylelint-scss` to validate rules and syntax.
- [sass-lint](https://github.com/sasstools/sass-lint) - *(⚠️ Deprecated /
  Archived)* Node-based Sass/SCSS linter; unmaintained and superseded by
  Stylelint.
- [scss-lint](https://github.com/causes/scss-lint) - *(⚠️ Deprecated /
  Archived)* Legacy Ruby gem for SCSS linting; superseded by Stylelint with
  `stylelint-scss`.

### Scala

- [Scalafix](https://scalacenter.github.io/scalafix/) - Extensible, syntactic
  and semantic linter and code refactoring engine for Scala by the Scala Center.
- [Scalafmt](https://scalameta.org/scalafmt/) - Deterministic code formatter
  for Scala supporting customizable and dialect-aware style rules.
- [Scapegoat](https://github.com/sksamuel/scapegoat) - Scala compiler plugin
  performing static code analysis to catch code smells, security risks, and
  bugs.
- [WartRemover](https://github.com/wartremover/wartremover) - Flexible,
  compile-time Scala linter configured to flag unsafe language constructs
  and warts.
- [linter](https://github.com/HairyFotr/linter) - *(⚠️ Obsolete / Archived)*
  Scala 2 compiler plugin; unmaintained.
- [Scalastyle](http://www.scalastyle.org) - *(⚠️ Stale / Legacy)* Java-like
  style checker for Scala; largely superseded by Scalafix and Scalafmt.

### Shell

- [ShellCheck](https://github.com/koalaman/shellcheck) - Static analysis tool
  giving warnings and suggestions for bash/sh shell scripts to avoid syntax
  and semantic bugs.
- [shellharden](https://github.com/anordal/shellharden) - Syntax highlighter
  and hardener that semi-automatically rewrites scripts to quote variables
  correctly.
- [shfmt](https://github.com/mvdan/sh) - POSIX shell, Bash, and mksh parser,
  formatter, and interpreter written in Go.

### SQL

- [sqlfluff](https://github.com/sqlfluff/sqlfluff) - Dialect-flexible and
  configurable SQL linter and auto-formatter supporting Postgres, Snowflake,
  BigQuery, MySQL, and more.
- [sqlfmt](https://sqlfmt.com/) - Opinionated, automated SQL formatter
  designed for dbt projects and modern data pipelines.
- [sqruff](https://github.com/quarylabs/sqruff) - Blazingly fast SQL linter
  and formatter written in Rust, maintaining compatibility with SQLFluff
  configuration files.

### Swift

- [swift-format](https://github.com/apple/swift-format) - Official formatting
  and linting tool developed by Apple for Swift source code.
- [SwiftFormat](https://github.com/nicklockwood/SwiftFormat) - Code library
  and CLI tool for reformatting Swift code with customizable style rules.
- [SwiftLint](https://github.com/realm/SwiftLint) - Widely-adopted static
  analysis tool to enforce Swift style and conventions based on community
  guidelines.

### TypeScript

- [Biome](https://biomejs.dev/) - Ultra-fast Rust-based linter and formatter
  providing zero-config TypeScript and JSX analysis.
- [Oxlint](https://github.com/oxc-project/oxc) - High-performance Rust-based
  linter supporting TypeScript with near-instant execution and zero config.
- [typescript-eslint](https://github.com/typescript-eslint/typescript-eslint) -
  Official tooling enabling ESLint to analyze TypeScript codebases with rich
  AST and type-aware linting.
- [tslint](https://github.com/palantir/tslint) - *(⚠️ Deprecated / Archived)*
  Legacy TypeScript linter deprecated by Palantir in favor of
  `typescript-eslint`.

### YAML

- [actionlint](https://github.com/rhysd/actionlint) - Static analysis tool and
  linter designed specifically for GitHub Actions workflow YAML files.
- [check-jsonschema](https://github.com/python-jsonschema/check-jsonschema) -
  Fast CLI tool to validate YAML and JSON files against JSON Schema definitions
  with built-in SchemaStore catalog support.
- [eslint-plugin-yml](https://github.com/ota-meshi/eslint-plugin-yml) - ESLint
  plugin providing AST-level linting and formatting rules for YAML documents.
- [KubeLinter](https://github.com/stackrox/kube-linter) - Static analysis tool
  checking Kubernetes YAML manifests and Helm charts for security flaws and
  production readiness.
- [Prettier](https://prettier.io/) - Multi-language, opinionated code formatter
  providing deterministic formatting support for YAML files.
- [Spectral](https://github.com/stoplightio/spectral) - Flexible JSON and YAML
  linter powered by custom JSONPath rules, with built-in support for OpenAPI
  and AsyncAPI schemas.
- [yamlfmt](https://github.com/google/yamlfmt) - Extensible command-line tool
  and library developed by Google to format and standardize YAML files.
- [yamllint](https://github.com/adrienverge/yamllint) - Standard Python-based
  linter checking YAML files for syntax validity, key duplication, trailing
  spaces, and indentation conventions.

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

# Contribution Guidelines

- One pull request per addition.
- Organize it inside the right language "container".
- Alphabetical order.
- PR title should follow the template: "Add [LINTER] for [LANGUAGE]."

We try to maintain a clean Markdown file, which means we run `pre-commit` on
every build. To make sure your merge request passes the CI, please run do one of
the following:

- `pre-commit install` before trying to commit for the first time. This will
  make sure every time you commit the linter acts automatically.

- `pre-commit run README.md` before you commit, each time.

- `pretteir --write --prose-wrap always` before each commit, every time.

`pre-commit install` is the easier way to guarantee the linting is performed
before each commit.

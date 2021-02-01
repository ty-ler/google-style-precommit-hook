A handy [pre-commit](http://pre-commit.com/) hook which will run Google's java
code style formatter for you on your code!

Usage:

```
repos:
  - repo: https://github.com/maltzj/google-style-precommit-hook
    rev: <latest-commit-sha>
    hooks:
      - id: google-style-java
```

_Note_: this file stores Google's code style formatter jar in a `.cache/`
directory so that it doesn't need to be re-downloaded each time. You will
probably want to add `.cache/` to the `.gitignore` file of the project which
uses this hook.

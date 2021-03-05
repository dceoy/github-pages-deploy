github-pages-deploy
===================

GitHub Pages Deployment Script

Installation
------------

This command depends on Git.

```sh
$ git clone git@github.com:dceoy/github-pages-deploy.git
$ cp github-pages-deploy/github-pages-deploy /path/to/bin/  # a path in ${PATH}
```

Example
-------

Deploy HTML documents in `/path/to/your/github/project/html` to GitHub Pages.

```sh
$ cd /path/to/your/github/project/
$ github-pages-deploy ./html
```

The command detects the remote URL from `./.git/config`.

Usage
-----

```sh
$ github-pages-deploy --help
GitHub Pages Deploy Script

Usage:
  github-pages-deploy [--debug] [--remote=<url>] [<dir>]
  github-pages-deploy --version
  github-pages-deploy -h|--help

Options:
  --debug           Debug mode
  --remote=<url>    Specify a remote repository URL
  --version         Print version
  -h, --help        Print usage

Arguments:
  <dir>             Path to an HTML directory
```

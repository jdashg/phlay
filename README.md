# Phlay your commits for phabricator

At Mozilla we often want to use commit series, but 'Arcanist', the default
phabricator command line tool, does not support this use case nicely. Phlay is
a hacky tool for people using git for their Mozilla development, which rewrites
git history, and pushes individual commits as revisions, with the correct bug
number, reviewers, and dependencies.

This tool depends on:

  - The `git-cinnabar` version of `arc` (https://github.com/mozilla-conduit/arcanist) being on the path,
  - A sufficiently recent version of `git`, and
  - Python >= 3.6 as 'python3'.

NOTE: This is a hacky tool made for my own use, probably don't depend on it
unless you're OK with it breaking.

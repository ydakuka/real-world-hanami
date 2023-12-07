# Real-world Hanami

> Real World Hanami apps and their open source codebases for developers to learn from

## Installation

```console
# Clone this git repo:
git clone git@github.com:ydakuka/real-world-hanami.git

cd real-world-hanami

# This will take some time...
git submodule update --init --remote --checkout --single-branch --depth 1
```

To speed this process up, you can tell git to fetch several repositories in parallel:

```console
git config [--global] submodule.fetchJobs 4
```

### Updating

The repositories are linked as git submodules.

To check out the latest the revisions, run:

```console
# This will take some time:
git submodule update --remote --checkout --single-branch --depth 1
```

## Other Real World codebase collections

- Real World Ruby https://github.com/jeromedalbert/real-world-ruby-apps
- Real World Rails https://github.com/eliotsykes/real-world-rails
- Real World RSpec https://github.com/pirj/real-world-rspec
- Real World Sinatra https://github.com/jeromedalbert/real-world-sinatra
- Real World Elixir Apps https://github.com/szTheory/real-world-elixir-apps
- Real World Phoenix https://github.com/szTheory/real-world-phoenix
- Real World Ember https://github.com/eliotsykes/real-world-ember
- Real World React Apps https://github.com/jeromedalbert/real-world-react-apps
- Real World Django https://github.com/ckrybus/real-world-django
- Know any others? Please open a PR and add the link here

## Contribute

Contributions are welcome! Reach out if you'd like some help.

### How to include a new repository

For a repo `fooser/baretory`:

```console
git submodule add git@github.com:username/project_name.git demos/project_name
```

### How to remove a repository

To remove a submodule:

```console
# Remove the submodule from .git/config
git submodule deinit -f path/to/submodule

# Remove the submodule from .git/modules
rm -rf .git/modules/path/to/submodule

# Remove from .gitmodules and remove the submodule directory
git rm -f path/to/submodule
```

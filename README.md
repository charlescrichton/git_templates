# git_templates

The git templates directory. Usually hosted at `~/.git_template`. 

This is used whenever `git init` is issued.

## Modifications

* `git_templates/hooks/commit-msg` has been created to add git commit messages to the Day One journal.
* `git_templates/hooks/pre-push`  has been created to add attempted git push messages to the Day One journal.

## Setup 

* Install DayOne-CLI. See http://dayoneapp.com/tools/cli-man/
* Clone this repo:

```shell
git clone https://github.com/charlescrichton/git_templates.git ~/.git_templates
```

* Set git to use the templates:

```shell
git config --global init.templatedir '~/.git_templates'
```

## Existing git repositories

To add this to an existing git repository simply call

```shell
git init
```

In the root of the repository. This will overwrite the .git/hooks directory.


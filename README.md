# Python Copier template

This is a template, for use by [copier](https://copier.readthedocs.io/en/stable/), which creates or updates python
repositories to our standard layout.

See the [copier documentation](https://copier.readthedocs.io/en/stable/) for details of how to use this template.

## Creating a repository

Assume that a blank new repository, `my_project`, is checked out:
- Run `uv tool install copier`
- Run `copier copy https://github.com/ISISComputingGroup/copier_template.git ./my_project`

Or, clone and use the template locally:
- Run `copier copy ./copier_template ./my_project`
- Answer the prompts
- `git commit` the resulting structure into `my_project`

## Updating a generated repository

- Run `copier update ./my_project`

## Developing the template itself

Run copier as normal pointed at the locally-checked out copy, but use the `--vcs-ref=HEAD` flag to force copier to use the most recent local commit.
rather than a tagged version.

CI runs in *this* repository to check that copier can successfully instantiate the template in this repo.

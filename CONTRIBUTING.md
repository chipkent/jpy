# Contributing

This guide will serve as a reference for contributing to Jpy.

## Getting the source

Jpy uses the [Forking Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow).  In this workflow, the [jpy-consortium/jpy](https://github.com/jpy-consortium/jpy) repository contains a minimum number of branches, and development work happens in user-forked repositories.

To learn more see:
* [Forking Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/forking-workflow)
* [Forking Projects](https://guides.github.com/activities/forking/)
* [Fork A Repo](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo)
* [Working With Forks](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/working-with-forks)

To get started quickly:
1) Navigate to [https://github.com/jpy-consortium/jpy](https://github.com/jpy-consortium/jpy).
2) Click `Fork` in the top right corner.
3) `git clone git@github.com:<username>/jpy.git`
4) Commit changes to your own branches in your forked repository.

Forked repositories do not have access to the same tokens/secrets as the jpy-consortium/jpy depository, so GitHub actions that depend upon secrets will fail. 
If you experience this problem, disable the offending GitHub action.  To disable GitHub actions in your forked repository, go to "Actions" -> "Disable Actions" in your forked repository settings (`https://github.com/<username>/jpy/settings/actions`).

Over time, forks will get out of sync with the upstream repository.  To stay up to date, either:
* Navigate to `https://github.com/<username>/jpy` and click on `Fetch upstream`, or
* Follow these directions on [Syncing A Fork](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/syncing-a-fork).

## Creating a Pull Request
Pull requests can be created through the GitHub website or through the GitHub CLI.

### GitHub Web

Follow the directions in [Creating A Pull Request From A Fork](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork).

### GitHub CLI

1) [Install GitHub command line tool](https://github.com/cli/cli).  
2) On the command line, cd into your checked-out fork/branch.
3) `gh pr create -f -w`
    * Use `jpy-consortium/jpy` as the base repository.
    * Use `<username>/jpy` as the repository to push to.
4) Your changes should automatically get pushed, and then a new pull request with your changes should open up in your browser. 
5) Complete the information in the pull request and click `Create pull request`.

For more information, see:
* [gh pr create](https://cli.github.com/manual/gh_pr_create)
* [CLI In Use](https://cli.github.com/manual/examples.html)


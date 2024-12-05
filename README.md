# Github Tutorial

## Description

This is a tutorial for Github.

## Notes

### Terminology

- Branch - A separate line of development that allows a user to work or fix features without affect the main codebase.
- Centralized Workflow - ???
- Feature Branch Workflow - ???
- Forking - ???
- Gitflow Workflow - ???
- HEAD - ???
- Hook - ???
- Main - ???
- Pull Request - ???
- Repository - ???
- Tag - ???
- Version Control - ???
- Working Tree - ???

### Git Commands

- `git add` moves changes from the user's working directory to the staging area. This allows the user to prepare a snapshot before committing it.
- `git branch` allows the user to create, list, rename or delete branches within a repository.
- `git checkout` allows the user to switch between different branches or commits, or restore files to a previous state.
- `git clean` removes untracked files and directories (i.e. not within the staging area or tracked by version control) from the user's working directory.
- `git clone` creates a copy of a repository.
- `git commit` takes the snapshot in the staging area and commits it to the repository's history.
  - `--amend` lets you amend the latest commit. This is used when a file or other important information was omitted from the previous commit.
- `git config` sets the Git configuration options on a global or local project level for a machine.
  - `git config user.email "your_email@example.com"` sets the given email address that Git will associate with locally created commits.
  - `git config user.name "Your Name"` sets the given name that Git will associate with locally created commits.
  - `--global` is applied to the operating system user. The global configuration can be found in a user's home directory (`~ /.gitconfig` on unix or `C:\Users\\.gitconfig` on windows).
  - `--local` is the default flag that applies to the repository. The local configuration can be found in the repository's .git directory `.git/config`.
  - `--system` is applied to the entire machine which covers all users on an operating system and all repositories. The system configuration can be found in a gitconfig file off the system root path (`$(prefix)/etc/gitconfig` on unix or `C:\ProgramData\Git\config` on windows).
- `git fetch` downloads a repository's branch, but it does not merge or apply this changes to your local repository.
- `git init` initializes your local directory as a new Git repository.
- `git log`
- `git merge`
- `git pull`
- `git push`
- `git rebase`
  - `-i`
- `git reflog`
- `git remote`
- `git reset`
- `git revert`
- `git status`

# Github Tutorial

## Description

This is a tutorial for Github.

## Notes

- `git config` sets the Git configuration values on a global or local project level.
  - `git config user.email "your_email@example.com"` sets the given email address that Git will associate with locally created commits.
  - `git config user.name "Your Name"` sets the given name that Git will associate with locally created commits.
  - `--global` is applied to the operating system user. The global configuration can be found in a user's home directory (`~ /.gitconfig` on unix or `C:\Users\\.gitconfig` on windows).
  - `--local` is the default flag that applies to the repository. The local configuration can be found in the repository's .git directory `.git/config`.
  - `--system` is applied to the entire machine which covers all users on an operating system and all repositories. The system configuration can be found in a gitconfig file off the system root path (`$(prefix)/etc/gitconfig` on unix or `C:\ProgramData\Git\config` on windows).
- `git init` initializes your local directory as a new repository.

# Github Tutorial

## Description

This is a tutorial for Github.

## Terminology

- Branch - A parallel version of a repository. By default every repository has one branch named main. Creating additional branches copies the main branch and allows the user to make any changes without disrupting the main branch. Normally, branches are used to work on specific features.
- Codespace - A development environment that is hosted in the cloud. GitHub codespaces can be customized by committing configuration files to the repository (i.e. configuration-as-code), and are hosted by GitHub in a Docker container that runs on a virtual machine.
- Dotfile - Files and folders on Unix-like systems starting with a period that control the configuration of applications and shells on your system.1
- GitHub - A collaboration platform that uses Git for versioning.
- GitHub Flow - A lightweight, branch-based workflow for projects with regular deployments.
- Merge - Adds the changes in a pull request and branch into the main branch.
- Merge Conflict - It occurs when changes are made to the same part(s) of the same file(s) on two different branches.
- Protected Branch - Branches that are protected from force pushes or accidental deletion. The main branch is protected by default.
- Pull Request - Shows the changes in a branch to other people and allows them to accept, reject, or suggest additional changes to your branch.
- Pull Request Review - Examining another contributor's changes and giving them feedback.
- Repository - A project containing files and folders. A repository tracks versions of these files and folders.
- Secure Hash Algorithm (SHA) - A reference to a specific object (e.g. a commit in GitHub).
- Semantic Versioning - A formal convention for specifying compatibility using a three-part version number: major version, minor version, and patch (e.g. 1.0.0).
  - A backward compatible fix (i.e. patch release) increments the third digit (e.g. 1.0.1).
  - A backward compatible new feature (i.e. minor release) increments the middle digit and resets the third digit (e.g. 1.1.0).
  - A breaking update (i.e. major release) increments the first digit, and resets the middle and last digits (e.g. 2.0.0).
- Task List - A list of checkboxes that is useful for tracking issues and pull requests. If it is included in the body of an issue or pull request, a progress indicator will appear.
- Version - A different iteration of updated software (e.g. operating systems, apps, dependencies, etc.).

## Git commands

- `git add` - Adds changes to files to the staging area.
- `git blame` - Displays the contents of a file, which lines were modified, and the author of those modifications.
- `git commit` - Creates a commit of the staged changes.
  - `-a` - A flag that stages all files that have been modified and deleted, but not newly created files.
  - `-m` - A flag that uses the following text as the commit message.
- `git push` - Transfers commits from your local repository to a remote repository.

## Notes

### Introduction to GitHub

#### Creating a branch

1. In your GitHub repository, click **Code** in the navbar.
2. Click on the branch dropdown.
3. In the field, type a name for the branch you want to create.
4. Click **Create branch <new_branch_name> from <original_branch_name>**.

#### Committing a file

1. In your GitHub repository, click on the **Add file** dropdown.
2. Click **Create new file**.
3. In the **Name your file...** field, type a name for the file you want to create.
4. In the **Enter file contents here** area, add the content for your file.
5. In the top right, click **Commit changes...**.
6. In the **Commit message** field, type a name for the commit.
7. In the bottom right, click **Commit changes**.

#### Creating a pull request

1. Follow one of the options below:
   - If you see **Compare & pull request**, click it then skip to step 6.
   - In your GitHub repository, click **Pull requests** in the navbar then proceed to step 2.
2. Click **New pull request**.
3. In the base branch dropdown, select the branch you want to compare against (e.g. main).
4. In the compare dropdown, select the branch you want to see the difference from.
5. Click **Create pull request**.
6. In the **Add a title** field, type a name for your pull request title.
7. In the **Add your description here...** area, add a description for what you did.
8. Below that, click **Create pull request**.

#### Merging a pull request

1. Click **Merge pull request**.
2. Click **Confirm merge**.
3. If you no longer need the branch you merged in, click **Delete branch**.

### Communicate using Markdown

#### Add headers

```md
# H1 heading

## H2 heading

### H3 heading

#### H4 heading

##### H5 heading

###### H6 heading
```

#### Add an image

```md
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
```

#### Add a code example

```js
console.log("Hello World");
```

#### Make a task list

```md
- [x] This item is complete
- [ ] This item is not complete
```

### GitHub Pages

#### Enable GitHub Pages

1. In your GitHub repository, click **Settings** in the navbar.
2. In the **Code and automation** section in the left sidebar, click **Pages**.
3. Select **Deploy from a branch** in the dropdown below **Source**.
4. Select **main** in the dropdown below **Branch**.
5. In the lower right, click **Save**.

#### Configure your site

1. Create a \_config.yml file.
2. Add a theme (the overall look and layout of your site), title (default title of the website), author (the site-wide default author name), and description (a description of the website for SEO metadata and in site headers[e.g. website logo, navigation menu, call-to-action buttons, etc.]).

#### Customize your homepage

1. Create an index.md file.
2. Add a title using YAML frontmatter:

```yaml
---
title: Welcome to my site
---
```

#### Create a blog post

1. Create a markdown file using the following format: **\_posts/YYYY-MM-DD-title.md** (e.g. \_posts/2024-12-05-first-blog-post.md).
2. Add the title and date using YAML frontmatter:

```yaml
---
title: First blog post
date: 2024-12-05
---
```

#### Viewing the site

1. In your GitHub repository, click **Settings** in the navbar.
2. In the **Code and automation** section in the left sidebar, click **Pages**.
3. Click **Visit site**.

### Review pull requests

#### Open a pull request

See [Creating a pull request](#creating-a-pull-request)

#### Assign yourself

1. In your GitHub repository, click **Pull requests** in the navbar.
2. Click the pull request you want to assign yourself to.
3. In the right sidebar, click below **Assignees**.
   - _Note that you can't assign yourself as a reviewer since you created the pull request._

#### Leave a review

1. In your GitHub repository, click **Pull requests** in the navbar.
2. Click **Files changed** in the secondary navbar.
3. Click **Review changes**.
4. In the **Leave a comment** field, type a comment about the pull request.
5. Select the **Comment** radio button.
   - _Note that you can't select **Approve** or **Request changes** since you created the pull request._
6. Click **Submit review**.

#### Suggest changes

1. In your GitHub repository, click **Pull requests** in the navbar.
2. Click **Files changed** in the secondary navbar.
3. Go to a file and hover your cursor over the line of code you want to suggest changes for.
4. Click the blue plus icon.
5. Click the **Add a suggestion, <Cmd+g>** icon to the right of **Preview**.
6. Edit the suggestion.
7. Click **Add a single comment**.

#### Apply suggested changes

1. Below the suggested change, click **Commit suggestion**.
2. In the **Commit title** field, type a name for the commit.
3. Click **Commit changes**.

### Resolve merge conflicts

1. In your GitHub repository, click **Pull requests** in the navbar.
2. Click the pull request you want to resolve the merge conflict in.
3. Click **Resolve conflicts**.
4. At the highlighted sections, modify the content.
5. Remove the merge conflict markers:

   ```git
   <<<<<<< other-branch
   =======
   >>>>>>> main
   ```

6. In the top right, click **Mark as resolved**.
7. In the top right, click **Commit merge**.

### Release-based workflow

#### Create a beta release

1. In your GitHub repository, click **Code** in the navbar.
2. In the right sidebar, click **Create a new release** below **Releases**.
3. Click the **Choose a tag** dropdown.
4. In the **Find or create a new tag** field, type a version number for this release (e.g. v0.0.9).
5. Click **Create new tag**.
6. Click the **Target** dropdown and select the branch you want to add the tag to.
7. In the **Release title** field, type a title for this release (v0.0.9).
8. Check the **Set as a pre-release** checkbox to indicate this release is a beta version.
9. Click **Publish release**.

#### Add a new feature to the release branch

See [Committing a file](#committing-a-file), [Creating a pull request](#creating-a-pull-request), and [Merging a pull request](#merging-a-pull-request).

#### Generate release notes

1. In your GitHub repository, click **Code** in the navbar.
2. In the right sidebar, click **Releases**.
3. Click **Draft a new release**.
4. Click the **Choose a tag** dropdown.
5. In the **Find or create a new tag** field, type a version number for this release.
6. Click **Create new tag**.
7. Click the **Target** dropdown, then select the branch you want to add the tag to and generate release notes for.
8. Click **Generate release notes**.
9. Release notes will be automatically generated. Feel free to edit any part of it.
   - _Automatically generated release notes provide an automated alternative to manually writing release notes for GitHub releases. Additionally, a user cqn quickly generate an overview of the contents of a release, a list of merged pull requests, a list of contributors to the release, and a link to a full changelog. These release notes can also be customized after generation._
10. Click the **Target** dropdown and select the main branch since this will be the branch to get the tag and release notes after merging.
11. Click **Save draft**.

#### Finalize the drafted release

1. In your GitHub repository, click **Code** in the navbar.
2. In the right sidebar, click **Releases**.
3. Click the pencil icon for the draft release you want to release.
4. Click the **Target** dropdown, then select the branch you want to release.
5. Click **Publish release**.

#### Commit a hotfix to the release

Committing a hotfix would require three branches: main, a hotfix branch, and fix-bug branch. The fix-bug branch (can have any name to describe what is being fixed) would be merged into the hotfix branch, then the hotfix branch would be merged into the main branch.

See [Committing a file](#committing-a-file), [Creating a pull request](#creating-a-pull-request), and [Merging a pull request](#merging-a-pull-request).

### Navigating through a repository

#### Resolve duplicate issues

1. In your GitHub repository, click **Issues** in the navbar.
2. Click the issue you want to resolve.
3. In the **Add your comment here...** field, type `Duplicate of #N` where N is the reference number to the duplicate issue.
   - _You can find an issue's reference number underneath its name._
4. Click **Close with comment**.

#### Find a commit in history

1. In your GitHub repository, click **Code** in the navbar.
2. Click the file you want to see the commit history of.
3. In the top left, click **Blame** which is to the right of **Preview**.
4. Click the commit message you want to see more information of.
5. In the top right next to **commit**, click the button to copy the commit message's SHA.
6. In your GitHub repository, click **Issues** in the navbar.
7. Click the issue you want to add the SHA to.
8. In the **Add your comment here...** field, paste the SHA.
9. Click **Comment**.

### Code with codespaces

- _Note that any of the git commands used in the codespace are similar to what would be used in VS Code._

#### Start a codespace

1. Click the green **Code** button.
2. Click the **Codespaces** tab.
3. Click **Create codespace on main** or the plus icon.

#### Push code to your repository from the codespace

1. After editing files, in the terminal type `git commit -a -m "Your commit message"` to create a commit.
2. In the terminal type `git push` to transfer commits from your local repository to a remote repository.

#### Add custom file images to your codespace

1. In your GitHub repository, click on the **Add file** dropdown.
2. Click **Create new file**.
3. In the **Name your file...** field, type `.devcontainer/devcontainer.json`.
4. In the devcontainer.json file add a name, image, remoteUser, and overrideCommand:

   ```json
   {
     // Name this configuration
     "name": "Codespace for Skills!",
     // This is the base codespace file images
     "image": "mcr.microsoft.com/vscode/devcontainers/universal:latest",
     "remoteUser": "codespace",
     "overrideCommand": false
   }
   ```

5. Click **Commit changes...**.
6. In the **Commit message** field, type a name for the commit.
7. In the bottom right, click **Commit changes**.

#### Enable a dotfile for your codespace

1. Click your profile picture.
2. Click **Settings**.
3. In the **Code, planning, and automation** section in the left sidebar, click **Codespaces**.
4. In the **Dotfiles** section, check the **Automatically install dotfiles** checkbox.
5. Click on the **Select repository** dropdown, and select the repository you want to automatically install dotfiles for in its codespace.

#### Add a dotfile to your repository

1. Click the green **Code** button.
2. Click the **Codespaces** tab.
3. Click **Create codespace on main** or the plus icon.
4. Inside the codespace, create a setup.sh file and add the following:

   ```sh
   #!/bin/bash

   sudo apt-get update
   sudo apt-get install sl
   echo "export PATH=\$PATH:/usr/games" >> ~/.bashrc
   ```

5. In the terminal type `git add setup.sh --chmod=+x`.
6. In the terminal type `git commit -m "Your commit message"`.
7. In the terminal type `git push`.
8. In the terminal type `sl` for a surprise.

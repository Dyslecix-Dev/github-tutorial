# Github Tutorial

## Description

This is a tutorial for Github.

## Terminology

- Branch - A parallel version of a repository. By default every repository has one branch named main. Creating additional branches copies the main branch and allows the user to make any changes without disrupting the main branch. Normally, branches are used to work on specific features.
- GitHub - A collaboration platform that uses Git for versioning.
- Merge - Adds the changes in a pull request and branch into the main branch.
- Pull Request - Shows the changes in a branch to other people and allows them to accept, reject, or suggest additional changes to your branch.
- Pull Request Review - Examining another contributor's changes and giving them feedback.
- Repository - A project containing files and folders. A repository tracks versions of these files and folders.
- Task List - A list of checkboxes that is useful for tracking issues and pull requests. If it is included in the body of an issue or pull request, a progress indicator will appear.

## Notes

### Introduction to GitHub

#### Creating a branch

1. In your GitHub repository, click **<> Code** in the navbar.
2. Click on the branch dropdown.
3. In the field, type a name for the branch you want to create.
4. Click **Create branch <new_branch_name> from <original_branch_name>**.

#### Committing a file

1. In your GitHub repository, click on the **Add file** dropdown.
2. Click **Create new file**.
3. In the **Name your file...** field, type a name for the file you want to create.
4. In the **Enter file contents here** area, add the content for your file.
5. In the top right corner, click **Commit changes...**.
6. In the **Commit message** field, type a name for the commit.
7. In the bottom right corner, click **Commit changes**.

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
5. In the lower right corner click **Save**.

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

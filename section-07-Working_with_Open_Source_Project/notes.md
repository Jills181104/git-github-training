## Adding a README File

A README.md file provides information about the project and helps new contributors understand the repository.

A README can contain:

- Project description
- Installation steps
- Usage instructions
- Technologies used
- Contribution guidelines

A good README makes the project easier to understand and use.

## 2. Adding the Important Templates

Templates provide a standard format for common contributions and communication.

Common GitHub templates include:

- Issue templates
- Bug report templates
- Feature request templates
- Pull Request templates

Templates help contributors provide the required information in a consistent format.

## 3. Filtering the Git Log to Better Understand the Repo

Git log can be used to understand the history of an open source project.

### View Commit History

1. `git shortlog`
     Groups commits by author and shows the number of commits made by each author.

2. `git log --author=username`
     Shows commits made by a specific author.

3. `git log --grep=#2`
     Shows commits whose messages contain #2.

4. `git log --grep=#2 --author=name --since=1.day`
     Shows commits containing #2, by a specific author, from the last 1 day.

Filtering the Git log helps contributors understand previous changes and development patterns in the repository.

## Importance and Naming of Feature Branches

Feature branches allow contributors to work on changes without directly modifying the main branch.

A feature branch should have a clear and meaningful name.

### Examples

```bash
feature-1/login-page
feature-1/user-profile
feature-2/payment-integration
bugfix/login-error
```

Good branch names make it easier to understand what the branch is working on.

## Importance of Descriptive Commits

Commit messages should clearly describe the changes made in the commit but limited to 50 characters, capitalize the message, don't end with period, use the body to add details and in the body explain what/why NOT how.

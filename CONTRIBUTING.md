# Contributing

When contributing to this repository, please first discuss the change you wish to make via issue with the maintainers of this repository before making a change.

Please note we have a code of conduct, please follow it in all your interactions with the project.

## Pull Request Process

1. Ensure any install or build dependencies are removed before the end of the layer when doing a
   build. Add only relevant files to commit and ignore the rest to keep the repo clean.
2. Update the README.md with details of changes to the interface, this includes new environment
   variables, exposed ports, useful file locations and container parameters.
3. You should request review from the maintainers once you submit the Pull Request.

## Instructions

- Git Workflow

```bash
## Step 1: Fork the Repository

## Step 2: Set Up Git & Clone the Repository
# Clone the repository to your local machine
$ git clone https://github.com/<Your-Username>/<Repo-Name>.git

# Add the upstream remote (original repository)
$ git remote add upstream https://github.com/<Original-Owner>/<Repo-Name>.git

# Fetch and merge updates from upstream/main (the main repository)
$ git fetch upstream
$ git merge upstream/main

## Step 3: Create and Publish Your Working Branch
$ git checkout -b <type>/<issue|issue-number>/{<additional-fixes>}
$ git push origin <type>/<issue|issue-number>/{<additional-fixes>}

## Branch Naming Conventions:
# wip - Work in Progress; long-term work; mainstream changes;
# feat - New Feature; future planned; non-mainstream changes;
# bug - Bug Fixes
# exp - Experimental features or ideas;

```

- On Task Completion:

```bash
## Committing and pushing your work
# Ensure branch
$ git branch

# Fetch and merge with upstream/main
$ git fetch upstream
$ git merge upstream/main

# Add untracked files
$ git add .

# Commit all changes with appropriate commit message and description
$ git commit -m "your-commit-message" -m "your-commit-description"

# Fetch and merge with upstream/main again
$ git fetch upstream
$ git merge upstream/main

# Push changes to your forked repository
$ git push origin <type>/<issue|issue-number>/{<additional-fixes>}

## Creating the PR using GitHub Website
# Create Pull Request from <type>/<issue|issue-number>/{<additional-fixes>} branch in your forked repository to the main branch in the upstream repository
# After creating PR, add a Reviewer (Any Admin) and yourself as the assignee
# Link Pull Request to appropriate Issue, or Project+Milestone (if no issue created)
# IMPORTANT: Do Not Merge the PR unless specifically asked to by an admin.
```

- After PR Merge

```bash
# Delete branch from forked repo
$ git branch -d <type>/<issue|issue-number>/{<additional-fixes>}
$ git push --delete origin <type>/<issue|issue-number>/{<additional-fixes>}

# Fetch and merge with upstream/main
$ git checkout main
$ git pull upstream
$ git push origin
```

- Always follow [commit message standards](https://chris.beams.io/posts/git-commit/)
- About the [fork-and-branch workflow](https://blog.scottlowe.org/2015/01/27/using-fork-branch-git-workflow/)

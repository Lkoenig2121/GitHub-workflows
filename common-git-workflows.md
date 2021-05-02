# Common Git Workflows
Several common git workflows for web development.

## Git clone, Some repo to your local machine

Clone a repository from some origin (in this example one of your GitHub repos), to your local machine.

```bash
git clone git@github.com:Lkoenig2121/Covalence-Navbar.git
```

This is going to download thew repository from the origin (GitHub) and "clone" it to your local machine.

## Git add, commit, and push

First, make some code changes.

Next, you want to "add" your changes to be commited.

```bash
git add .
```

Then, you need to "commit" your changes.

```bash
git commit -m "your commit message"
```

Last, you need to "push" your changes to the origin (GitHub).

```bash
git push -u origin main
```

## Create new branch, merge back in to main

Before make sure your in the `main` branch.

```bash
git checkout main
```

Then, check that you have the most up to date changes, against your origin (GitHub).

```bash
git fetch
```

Pull in any changes

```bash
git pull
```

Create your branch

```bash
git checkout -b "the-name-of-your-branch"
```

Follow the steps in the first workflow (add, commit, push).

Now your ready to **merge** your branch into your `main` branch.

```bash
git merge "the-name-of-your-branch"
```

Finally, "push" your changes up to origin (GitHub).

```bash
git push -u origin main
```

## Helpful Commands

Initialize new Git repository.

```bash
git init
```

Check the status of your repository.

```bash
git status
```

Print differential to screen.

```bash
git diff
```

## Setup GitHub Pages on a repository

Create and host a static site from your repository free via GitHub Pages

1. Go to `Setting`
2. Scroll down to the lower left-hand side of the screen and select `Pages`
3. Folllow the instructions to enable *GitHub Pages*
4. Select the Repo / branch (i.e Covalence-Navbar/main)
5. You should be good to go :)

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Sandbox repository for practicing the GitHub pull request workflow (branch, commit, push, open a PR). It contains only documentation files — no application code, build system, linter, or tests, so there are no build/lint/test commands.

## PR workflow

Work on a topic branch from `main`, then open a PR with `gh pr create`. After merging with `gh pr merge N --merge --delete-branch`, sync with `git pull --ff-only origin main` (`git fetch origin main:main` fails while `main` is checked out) and confirm `git status` shows `main` equal to `origin/main`. Check `gh pr list --state all` for unmerged PRs before deleting any branch.

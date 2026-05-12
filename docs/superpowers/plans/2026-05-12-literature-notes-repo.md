# Literature Notes Repository Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a GitHub-ready literature notes repository from the user's Word note.

**Architecture:** Use Markdown files organized by research direction. The root README is the global index, each direction has its own index, and each paper receives one focused note file.

**Tech Stack:** Markdown, Git, GitHub remote publishing.

---

### Task 1: Create Repository Documents

**Files:**
- Create: `README.md`
- Create: `notes/embodied-intelligence/README.md`
- Create: `notes/embodied-intelligence/rt-2-vision-language-action-models.md`
- Create: `templates/paper-note-template.md`
- Create: `docs/superpowers/specs/2026-05-12-literature-notes-repo-design.md`

- [x] **Step 1: Create Markdown files**

Write the approved repository structure and convert the Word note content into Markdown.

- [x] **Step 2: Include stable paper links**

Use `https://arxiv.org/abs/2307.15818`, `https://doi.org/10.48550/arXiv.2307.15818`, and `https://robotics-transformer2.github.io`.

### Task 2: Initialize Git and Commit

**Files:**
- Modify: `.git/`

- [ ] **Step 1: Initialize Git**

Run: `git init`

- [ ] **Step 2: Commit files**

Run: `git add .`

Run: `git commit -m "Initial literature notes repository"`

### Task 3: Publish to GitHub

**Files:**
- Modify: `.git/config`

- [ ] **Step 1: Confirm GitHub access**

Run: `gh auth status`

Expected: authenticated GitHub account. If `gh` is unavailable, install GitHub CLI or provide an empty GitHub repository URL.

- [ ] **Step 2: Create and push remote**

Run: `gh repo create literature-notes --public --source . --remote origin --push --description "读过的论文与文献笔记"`

Expected: repository created and local commit pushed to GitHub.

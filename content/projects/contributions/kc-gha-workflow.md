---
title: "GitHub Actions Workflow"
link: "https://github.com/mischavandenburg/kubecraft/pull/51"
image: "/img/gha-workflow.png"
description: "Developed GitHub Actions workflow to update commits to KubeCraft Community documentation"
featured: true
tags: ["GitHub Actions","CI/CD","Git","Bash","Web Development"]
fact: "Automated page generation of all previous <code>docs</code> commits."
weight: 100
sitemap: 
    priority : 0.8
---

The GHA workflow executes a script and runs steps that perform the following:
- Scans commits for docs in the subject
- Formats docs commits into a brief description with committer and hash information
- Groups commits by date
- Creates a new list of commits for publication when new docs commits are made
- Creates a PR to merge the updated list of commits

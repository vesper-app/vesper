# Contributing to Vesper

First off, thank you for considering contributing to Vesper! We're thrilled you're interested in helping us build a better terminal multiplexer. Every contribution, from a typo fix to a new feature, is valuable.

This document is a guide to help you through the process.

## How Can I Contribute?

There are many ways to contribute to the Vesper project.

*   **🐛 Reporting Bugs:** If you find something that's not working as expected, please [**submit a Bug Report**](https://github.com/vesper-app/vesper/issues/new?template=bug_report.yml). A great bug report is detailed and provides clear steps to reproduce the issue.
*   **🚀 Proposing Features:** Have a great idea for a new feature? We'd love to hear it. Please [**submit a Feature Proposal**](https://github.com/vesper-app/vesper/issues/new?template=feature_proposal.yml) to start the conversation.
*   **📚 Improving Documentation:** If you find a typo or an unclear section on our website or in our documentation, please [**submit a Documentation Issue**](https://github.com/vesper-app/vesper/issues/new?template=documentation_issue.yml).
*   **✍️ Writing Code:** If you're ready to write some code, this guide will walk you through setting up your environment and submitting your first pull request.

## Your First Code Contribution

Ready to dive in? Here’s a step-by-step guide to setting up your development environment and submitting a pull request.

### 1. Prerequisites

Before you begin, please ensure you have the necessary build tools installed. This is the same toolchain needed to build Vesper from source. On a Debian/Ubuntu system, you can install them with:
```bash
sudo apt update && sudo apt install build-essential libncursesw-dev libx11-dev libxft-dev libxinerama-dev
```

### 2. Fork and Clone the Repository

First, create your own copy (a "fork") of the Vesper repository on GitHub. Then, clone your fork to your local machine.

```bash
git clone https://github.com/YOUR_USERNAME/vesper.git
cd vesper
```

### 3. Build the Project

Our `Makefile` handles everything. To create a debug build for development, simply run:
```bash
make
```
You can now run your local development version of Vesper with `./vesper`.

### 4. Create a New Branch

Never work directly on the `main` branch. Create a new branch for your feature or bug fix. Use a descriptive name.
```bash
# For a new feature:
git checkout -b feat/add-command-palette

# For a bug fix:
git checkout -b fix/resolve-scrolling-issue
```

### 5. Write Your Code

Make your changes! Adhere to the existing code style to keep the project consistent.

### 6. Commit Your Changes

We follow the [**Conventional Commits**](https://www.conventionalcommits.org/) standard. This helps us automate releases and keep the project history clean. Your commit message should be clear and concise.

```bash
# Example commit for a new feature:
git commit -m "feat: Add discoverable command palette" -m "Adds a new floating pane with a fuzzy-findable list of all Vesper commands, accessible via <Prefix>+p."

# Example commit for a bug fix:
git commit -m "fix: Correctly handle remote pane scroll events" -m "Fixes an issue where scroll passthrough was not working for older tmux versions."
```

### 7. Submit a Pull Request

Once you've committed your changes, push your branch to your fork on GitHub:
```bash
git push -u origin feat/add-command-palette
```
Then, go to the Vesper repository on GitHub. You will see a prompt to "Compare & pull request." Click it, write a clear description of your changes, and be sure to **link the issue** your PR resolves by writing something like `Closes #42` in the PR description.

## Code of Conduct

To ensure our community is welcoming and inclusive for everyone, we have adopted a Code of Conduct that all contributors are expected to follow. Please read the [**Code of Conduct**](./CODE_OF_CONDUCT.md) before participating.

Thank you again for your interest in contributing!
```

---

### **Bonus: The `CODE_OF_CONDUCT.md` File**

The `CONTRIBUTING.md` file links to a `CODE_OF_CONDUCT.md`. It is a strong best practice to have this file. The industry standard is the **Contributor Covenant**.

Create a file named `CODE_OF_CONDUCT.md` in the root of your `vesper-app/vesper` repository and paste the following content. This is a complete, professional, and widely respected document.

```markdown
# Contributor Covenant Code of Conduct

## Our Pledge

We as members, contributors, and leaders pledge to make participation in our
community a harassment-free experience for everyone, regardless of age, body
size, visible or invisible disability, ethnicity, sex characteristics, gender
identity and expression, level of experience, education, socio-economic status,
nationality, personal appearance, race, religion, or sexual identity
and orientation.

We pledge to act and interact in ways that contribute to an open, welcoming,
diverse, inclusive, and healthy community.

## Our Standards

Examples of behavior that contributes to a positive environment for our
community include:

*   Demonstrating empathy and kindness toward other people
*   Being respectful of differing opinions, viewpoints, and experiences
*   Giving and gracefully accepting constructive feedback
*   Accepting responsibility and apologizing to those affected by our mistakes,
    and learning from the experience
*   Focusing on what is best not just for us as individuals, but for the
    overall community

Examples of unacceptable behavior include:

*   The use of sexualized language or imagery, and sexual attention or
    advances of any kind
*   Trolling, insulting or derogatory comments, and personal or political attacks
*   Public or private harassment
*   Publishing others' private information, such as a physical or email
    address, without their explicit permission
*   Other conduct which could reasonably be considered inappropriate in a
    professional setting

## Enforcement Responsibilities

Community leaders are responsible for clarifying and enforcing our standards and
will take appropriate and fair corrective action in response to any behavior
that they deem inappropriate, threatening, offensive, or harmful.

Community leaders have the right and responsibility to remove, edit, or reject
comments, commits, code, wiki edits, issues, and other contributions that are
not aligned to this Code of Conduct, and will communicate reasons for moderation
decisions when appropriate.

## Scope

This Code of Conduct applies within all community spaces, and also applies when
an individual is officially representing the community in public spaces.
Examples of representing our community include using an official e-mail address,
posting via an official social media account, or acting as an appointed
representative at an online or offline event.

## Enforcement

Instances of abusive, harassing, or otherwise unacceptable behavior may be
reported to the community leaders responsible for enforcement at
[INSERT YOUR CONTACT EMAIL HERE].
All complaints will be reviewed and investigated promptly and fairly.

All community leaders are obligated to respect the privacy and security of the
reporter of any incident.

## Enforcement Guidelines

Community leaders will follow these Community Impact Guidelines in determining
the consequences for any action they deem in violation of this Code of Conduct:

### 1. Correction

**Community Impact**: Use of inappropriate language or other behavior deemed
unprofessional or unwelcome in the community.

**Consequence**: A private, written warning from community leaders, providing
clarity around the nature of the violation and an explanation of why the
behavior was inappropriate. A public apology may be requested.

### 2. Warning

**Community Impact**: A violation through a single incident or series
of actions.

**Consequence**: A warning with consequences for continued behavior. No
interaction with the people involved, including unsolicited interaction with
those enforcing the Code of Conduct, for a specified period of time. This
includes avoiding interaction in community spaces as well as external channels
like social media. Violating these terms may lead to a temporary or
permanent ban.

### 3. Temporary Ban

**Community Impact**: A serious violation of community standards, including
sustained inappropriate behavior.

**Consequence**: A temporary ban from any sort of interaction or public
communication with the community for a specified period of time. No public or
private interaction with the people involved, including unsolicited interaction
with those enforcing the Code of Conduct, is allowed during this period.
Violating these terms may lead to a permanent ban.

### 4. Permanent Ban

**Community Impact**: Demonstrating a pattern of violation of community
standards, including sustained inappropriate behavior, harassment of an
individual, or aggression toward or disparagement of classes of individuals.

**Consequence**: A permanent ban from any sort of public interaction within
the community.

## Attribution

This Code of Conduct is adapted from the [Contributor Covenant][homepage],
version 2.0, available at
[https://www.contributor-covenant.org/version/2/0/code_of_conduct.html][v2.0].

[homepage]: https://www.contributor-covenant.org
[v2.0]: https://www.contributor-covenant.org/version/2/0/code_of_conduct.html
```
**Crucial Action:** Remember to replace `[INSERT YOUR CONTACT EMAIL HERE]` with a real email address (e.g., `conduct@vesper.sh`).

With these two files, you now have a professional, welcoming, and safe framework for growing your open-source community.

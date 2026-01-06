# GitHub Copilot for Repository Management Quest

## Quest Overview

Welcome to the **GitHub Copilot for Repository Management Quest** - an interactive learning experience designed for content developers who want to master GitHub Copilot's native features for repository management workflows. This quest simulates real-world scenarios that content teams face daily, from taking over unfamiliar repositories to managing complex pull requests and issue backlogs.

**What makes this quest unique:** You'll learn to leverage GitHub Copilot's workspace agent, PR summarization, issue analysis, and automated code generation features - all within your natural GitHub workflow.

## Learning Objectives

By completing this quest, you will:

1. **Master GitHub Copilot workspace exploration** - Use Copilot's @workspace agent to quickly understand unfamiliar repositories and documentation structures
2. **Develop advanced PR review skills** - Leverage GitHub Copilot's PR summaries, review suggestions, and inline chat for efficient pull request reviews
3. **Implement efficient issue management** - Use Copilot to analyze issues, suggest fixes, and even generate PRs automatically from issue descriptions
4. **Create documentation standards** - Establish quality standards with Copilot-assisted reviews and automated checks
5. **Build practical workflows** - Develop repeatable processes using GitHub Copilot's native capabilities

## Quest Structure

This quest contains a foundational module and four progressive scenarios, each building on skills from the previous one:

### Module 0: Workspace Preparation
**Duration:** 15-20 minutes
**Difficulty:** Beginner to Intermediate

Before diving into repository management scenarios, learn how to customize your GitHub Copilot workspace with agents and reusable prompts. This foundational module introduces you to `.agents` and `.prompts` files that will supercharge your productivity throughout the quest.

**Tasks:**
- 0.1: Introduction to agents and prompts with examples
- 0.2: Creating your first custom agent
- 0.3: Building a comprehensive prompt library
- 0.4: Testing and optimizing your workspace configuration

### Scenario 1: The Inheritance
**Duration:** 30-45 minutes
**Difficulty:** Beginner to Intermediate

You've just been assigned to take over a documentation repository from a team member who left suddenly. The repository contains dozens of markdown files, some Python utilities, and no clear structure. Your mission: understand what you've inherited, identify issues, and create an actionable improvement plan.

**Tasks:**
- 1.1: Explore and map the repository structure using GitHub Copilot's @workspace agent
- 1.2: Identify outdated content, broken links, and inconsistencies with Copilot Chat
- 1.3: Generate a comprehensive content audit report using Copilot
- 1.4: Create documentation standards with Copilot's assistance
- 1.5: Advanced content analysis using custom agents and prompt templates

### Scenario 2: The Big Merge
**Duration:** 45-60 minutes
**Difficulty:** Intermediate

A contributor has submitted a massive pull request touching 15+ markdown files across multiple documentation sections. The changes include new tutorials, updated guides, and restructured content. You need to review this PR efficiently, identify issues, and guide the contributor to success.

**Tasks:**
- 2.1: Use GitHub Copilot's PR summary and review features for initial assessment
- 2.2: Leverage Copilot inline suggestions to identify style and technical issues
- 2.3: Use Copilot to draft constructive review comments and suggestions
- 2.4: Validate cross-references with @workspace context awareness

### Scenario 3: The Backlog Battle
**Duration:** 45-60 minutes
**Difficulty:** Intermediate to Advanced

Your documentation repository has accumulated 25+ open issues over the past few months. They range from typo fixes to requests for new content, from bug reports to feature suggestions. Your challenge: triage this backlog efficiently and create a sustainable issue management process.

**Tasks:**
- 3.1: Use Copilot to bulk categorize and prioritize the issue backlog
- 3.2: Leverage Copilot to identify duplicates and relationships between issues
- 3.3: Generate issue templates with Copilot's assistance
- 3.4: Use Copilot to draft responses and even create fix PRs directly from issues
- 3.5: Advanced issue triage using specialized agents
- 3.6: Automated duplicate detection with AI workflows
- 3.7: Intelligent template creation for consistent communications

### Scenario 4: The Agent Arsenal
**Duration:** 45-60 minutes
**Difficulty:** Advanced

You've mastered the basics of repository management with GitHub Copilot. Now it's time to build an advanced agent ecosystem that can handle complex, multi-step workflows automatically. Your challenge: create a suite of specialized agents that work together to manage an entire documentation project lifecycle.

**Tasks:**
- 4.1: Advanced agent design for enterprise-scale workflows
- 4.2: Agent workflow orchestration and coordination
- 4.3: Performance optimization for large-scale operations
- 4.4: Quality assurance automation with meta-agents

## Prerequisites

- **Git fundamentals**: Basic understanding of repositories, commits, branches, and pull requests
- **Markdown knowledge**: Familiarity with markdown syntax and documentation
- **GitHub Copilot**: Active GitHub Copilot subscription (individual, business, or enterprise)
- **Tools**: VS Code with GitHub Copilot extension, Git client, GitHub account

**Optional but helpful:**
- Experience with documentation systems (MkDocs, Jekyll, Docusaurus)
- Basic Python knowledge for understanding utility scripts
- Prior experience with code review processes

## Quest Format

This quest uses a **conceptual and interactive lab** format:

- **Conceptual sections** explain key GitHub Copilot features and best practices
- **Interactive labs** provide hands-on exercises with real repository scenarios
- **GitHub Copilot prompts** are provided for each task (copy-paste ready)
- **Solution guides** show expected Copilot interactions and outputs
- **Reflection prompts** encourage you to apply these skills to your work

## Getting Started

### Setup Requirements

1. **Install VS Code** - Download from https://code.visualstudio.com/
2. **Install GitHub Copilot extension** - From VS Code marketplace
3. **Activate GitHub Copilot** - Sign in with your GitHub account
4. **GitHub account** - Required for forking and running workflows

### Repository Setup

1. **Fork this repository** to your own GitHub account:
   - Click the "Fork" button at the top-right of this repository
   - Choose your account as the destination for the fork

2. **Clone your fork** (replace `[your-username]` with your GitHub username):
   ```bash
   git clone https://github.com/[your-username]/github-repo-management-quest.git
   cd github-repo-management-quest
   code .
   ```

3. **Create sample content** by running the setup workflows:

   **Option A: Using GitHub Web Interface (Recommended)**
   - Go to your forked repository on GitHub
   - Navigate to the **Actions** tab
   - You'll see two workflows: "Setup Quest Issues" and "Setup Quest PR"
   
   **To create sample issues for Scenario 3:**
   - Click on "Setup Quest Issues" workflow
   - Click "Run workflow" button
   - Select "scenario-3" from the dropdown
   - Click the green "Run workflow" button
   - Wait for the workflow to complete (creates 8 sample issues)

   **To create sample PR for Scenario 2:**
   - Click on "Setup Quest PR" workflow  
   - Click "Run workflow" button
   - Select your preferred PR size (small/medium/large)
   - Click the green "Run workflow" button
   - Wait for the workflow to complete (creates 1 sample pull request)

   **Option B: Using GitHub CLI (if you have it installed)**
   ```bash
   # Create sample issues
   gh workflow run setup-quest-issues.yml --field scenario=scenario-3

   # Create sample PR
   gh workflow run setup-quest-pr.yml --field pr_size=medium
   ```

4. **Verify setup**:
   - Check the **Issues** tab - you should see 8 sample issues labeled "quest-sample"
   - Check the **Pull requests** tab - you should see 1 sample PR labeled "quest-sample"

### Quest Workflow

1. **Open VS Code** with your forked repository
2. **Start with Scenario 1** in the `scenario-1-inheritance/` directory
3. **Open Copilot Chat** (Ctrl+Shift+I or Cmd+Shift+I)
4. **Follow task instructions** - use provided Copilot prompts
5. **Complete each task** using GitHub Copilot features
6. **Use your sample issues and PR** created by the workflows for Scenarios 2 & 3
7. **Check solution guides** to see expected approaches
8. **Progress through scenarios** at your own pace

### Important Notes

- **Scenario 1** uses the files in `scenario-1-inheritance/challenge-repo/` - no setup needed
- **Scenario 2** requires the sample PR created by running "Setup Quest PR" workflow
- **Scenario 3** requires the sample issues created by running "Setup Quest Issues" workflow
- All sample content is labeled with "quest-sample" for easy identification
- You can re-run the workflows anytime to create fresh sample content

### Troubleshooting

**Workflows not visible in Actions tab?**
- Make sure you're looking at your forked repository, not the original
- GitHub Actions should be enabled by default on forks

**Workflow run failed?**
- Check that your repository is public (required for GitHub Actions on free accounts)
- Ensure you have the latest version by syncing your fork with the original repository

**No sample issues or PRs created?**
- Check the Actions tab for workflow run details and any error messages
- Verify the workflows completed successfully (green checkmark)
- Issues appear in the "Issues" tab, PRs appear in "Pull requests" tab

**Need to start over?**
- You can delete the sample issues and PR, then re-run the workflows
- Or fork the repository again for a completely fresh start

## Repository Structure

```
github-repo-management-quest/
├── README.md (this file)
├── scenario-1-inheritance/
│   ├── README.md (scenario overview)
│   ├── challenge-repo/ (the repository you'll work with)
│   ├── tasks/ (individual task instructions)
│   └── solutions/ (solution guides and examples)
├── scenario-2-big-merge/
│   ├── README.md
│   ├── challenge-repo/
│   ├── pr-content/ (the pull request files)
│   ├── tasks/
│   └── solutions/
├── scenario-3-backlog-battle/
│   ├── README.md
│   ├── challenge-repo/
│   ├── issues/ (the backlog of issues)
│   ├── tasks/
│   └── solutions/
└── resources/
    ├── copilot-prompts.md (GitHub Copilot prompts for common tasks)
    ├── best-practices.md (content repository management tips)
    └── copilot-features-guide.md (mastering Copilot features)
```

## Time Commitment

- **Complete quest**: 2-3 hours
- **Individual scenarios**: 30-60 minutes each
- **Self-paced**: Work through scenarios on your own schedule
- **Requires**: Active VS Code session with GitHub Copilot

## Skills You'll Gain

### GitHub Copilot Mastery
- **@workspace agent** for repository-wide understanding
- **Copilot Chat** for analysis and content generation
- **Inline suggestions** for documentation improvements
- **PR summaries** for efficient code reviews
- **Issue-to-PR** automation workflows

### Repository Management
- Repository exploration with AI context awareness
- Content auditing and quality analysis
- Efficient pull request review strategies
- Issue triage and categorization at scale
- Automated template and standards generation
- Cross-reference validation with workspace intelligence

## Support and Feedback

- **Questions?** Open an issue in this repository
- **Stuck?** Check the solution guides in each scenario
- **Ideas for improvement?** We welcome contributions and feedback!

## Next Steps

Ready to begin? Head to [Scenario 1: The Inheritance](scenario-1-inheritance/README.md) to start your journey!

---

**Quest Version:** 1.0
**Last Updated:** 2025-12-01
**Estimated Completion Time:** 2-3 hours
**Difficulty Level:** Beginner to Advanced

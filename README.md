# Teste
AI-powered usability testing by ORCATE


# Teste by ORCATE

### See your website through someone else's eyes.

Teste is a local-first, AI-powered usability testing application built for developers, vibe coders, designers and independent creators.

## What is Teste?

When you build a website, you already know where everything is, what every button does and how every feature works.

Your users don't.

Teste allows AI agents to experience your website as simulated first-time visitors. They independently navigate pages, attempt tasks, interact with features and identify problems that you might have overlooked.

Unlike conventional automated testing, Teste evaluates both functionality and usability.

It helps answer questions such as:

- Can a new visitor understand what my website does?
- Is the navigation confusing?
- Are important features difficult to discover?
- Do buttons and forms respond correctly?
- Is the mobile experience comfortable to use?
- Can users successfully complete their intended tasks?

Teste captures real browser evidence and generates actionable improvement prompts for your AI coding agent.

## Download

[Download Teste 1.0.1 — Public Beta](https://github.com/rudranshjain0123/Teste/releases/download/v1.0.1-beta/Teste.zip)

[Read the 1.0.1 release notes](https://github.com/rudranshjain0123/Teste/releases/tag/v1.0.1-beta)

## Getting Started

### Method 1: Install using an AI agent (Recommended)

1. Download Teste.zip.
2. Open Codex, Claude Code or another compatible coding agent.
3. Attach the downloaded ZIP.
4. Send the following prompt:

    Install Teste from the attached ZIP using its included
    documentation. Configure its dependencies and MCP
    integration, start the application and provide its
    local URL.

5. Open the local application URL provided by your agent.

### Method 2: Manual installation

Extract Teste.zip and open the Teste folder. Install Python with virtual environment support. The install scripts download the Python dependencies and Playwright Chromium.

**macOS / Linux:** `chmod +x install.sh start.sh stop.sh`, then `./install.sh` and `./start.sh`. Stop with `./stop.sh`.

**Windows 10 / 11 (Beta):** In Command Prompt, run `install.bat` and `start.bat`. Stop with `stop.bat`.

Open the local address printed by the start script. In Settings → AI Integrations, choose **Copy MCP Command** to get the command for your installation.

## How to Use Teste

### Step 1 — Prepare your website

Start your development website or use an existing deployed website that you own or are authorized to test.

Teste supports local development websites and authorized public websites.

### Step 2 — Provide a website briefing

Tell Teste:

- Your website's URL.
- What your website does.
- Its intended audience.
- What you want users to accomplish.
- Any important limitations or unfinished functionality.

For example:

    Website: My productivity application
    URL: http://localhost:3000
    Audience: Students and professionals
    Objective: Find the task creation feature and create a task.
    Note: Account registration is not implemented yet.

This helps Teste understand what it should evaluate without revealing exactly how users should complete the task.

### Step 3 — Choose user personas

Different users approach websites differently.

Teste supports simulated personas such as:

- First-time beginner
- Impatient user
- Technical user
- Skeptical visitor
- Returning user
- Custom personas

Each persona has its own background, technical knowledge, expectations and behavioral preferences.

Personas explore the website through isolated browser contexts.

### Step 4 — Start a usability test

Choose a task-based or exploratory evaluation.

In external-agent mode, instruct your connected AI agent to conduct the evaluation using Teste's MCP tools.

Example prompt:

    Use Teste to evaluate my website at
    http://localhost:3000.

    It is a productivity application for students.

    Test it using a first-time beginner, an impatient
    user and a technical user.

    Ask each persona to locate the task creation feature
    and attempt to create a task.

    Record screenshots, browser actions and usability
    findings. Generate actionable fix prompts.

    Do not modify my website during the evaluation.

Use separate agent sessions for each persona where supported to avoid sharing previous discoveries.

### Step 5 — Watch the testing session

Teste uses real browser automation rather than generating hypothetical website reviews.

During a session, it can record:

- Page navigation
- Button clicks
- Form interactions
- Scrolling
- Screenshots
- Observable browser errors
- Task completion or failure

### Step 6 — Review your report

Open the Reports section to inspect the results.

Reports help you understand:

- What problems were discovered.
- Which personas encountered them.
- What happened during each interaction.
- Why an issue affects usability.
- How to reproduce the problem.
- What could be improved.

Supporting screenshots and action logs allow you to inspect the evidence yourself.

### Step 7 — Fix your website

Copy the generated fix prompts and provide them to your preferred coding agent.

Teste identifies and explains problems. Your coding agent implements the improvements.

### Step 8 — Retest

After making improvements, repeat the original test under comparable conditions.

This helps identify resolved problems, remaining issues and newly introduced defects.

## Example Workflow

BUILD → TEST → ANALYZE → FIX → RETEST

1. Build a website using Codex.
2. Evaluate it using Teste.
3. Review the usability findings.
4. Give the generated correction prompts to Codex.
5. Retest the improved website.

## Main Interface

| Tab | Purpose |
|---|---|
| Test | Configure website briefings, personas and testing objectives |
| Session | Inspect browser activity and recorded interactions |
| Reports | Review findings, screenshots and previous audits |

## Key Features

- AI-driven usability evaluations
- Real browser automation
- Customizable user personas
- Website-specific briefings
- Desktop and mobile viewport testing
- Isolated browser contexts
- Screenshot capture
- Interaction replay
- Evidence-backed reports
- Actionable AI fix prompts
- Persistent local audit history
- Portable audit import and export
- Regression testing
- Local MCP integration

## Compatibility

| Platform or Integration | Status |
|---|---|
| macOS | Fresh installation, dynamic path resolution and Codex MCP connectivity verified |
| Linux | Automated browser and application tests passed |
| Windows | Beta; native verification pending |
| Codex | MCP connectivity verified; full live usability audit not performed for 1.0.1 |
| Claude Code | Documented MCP target; not independently verified |
| OpenCode | MCP-compatible |
| Independent API integration | Under development |

The current release primarily uses external AI agents.

Independent API-key integration is under development and should not be assumed to be fully operational.

## Privacy and Local Storage

Teste runs locally on your computer.

- No mandatory ORCATE account.
- No mandatory hosted backend.
- Local audit history.
- Locally stored screenshots and reports.
- Persistent data across application restarts.

Your connected AI agent or external AI provider may process browser observations according to its own privacy policies and usage limits.

Only test websites you own or have permission to evaluate.

Use disposable test accounts and avoid exposing sensitive information during testing.

## Is Teste Free?

The public beta is available as a free download.

Teste does not require mandatory paid hosting.

However, your chosen AI agent or API provider may have separate subscription requirements, usage limits or charges.

## Beta Notice

Teste is currently in public beta.

AI personas are simulated users, not actual human participants. Their observations can help discover usability problems but do not replace human user research or professional accessibility audits.

Windows support remains in beta. Independent API integration is under development.

Please report bugs and suggestions through GitHub Issues.

## About ORCATE

ORCATE builds practical software and resources for developers, AI enthusiasts and creators.

[Visit ORCATE](https://orcate.rudranshjain0123.workers.dev)

---

**Teste — Built by ORCATE.**

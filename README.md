# Ned + Josh Collab

A shared workspace for building together with **Zed**, **AI coding agents**, and **GitHub**.

[Quick start](#quick-start) · [AI setup](#ai-setup) · [GitHub access](#github-access) · [Working independently](#working-independently) · [Collaboration rules](#collaboration-rules)

> [!TIP]
> **The easiest way to start:** install Zed, sign in with GitHub, and join Josh's shared project. No Git installation or separate clone is needed for live collaboration.

## Quick start

### 1. Install Zed

**On any computer:** download and run the installer from **[zed.dev/download](https://zed.dev/download)**.

Prefer a terminal install? Choose the command for your operating system:

**Windows — PowerShell**

```powershell
winget install -e --id ZedIndustries.Zed --accept-source-agreements --accept-package-agreements
```

**macOS — Terminal, with Homebrew already installed**

```sh
brew install --cask zed
```

**Linux — Terminal**

```sh
curl -f https://zed.dev/install.sh | sh
```

The Linux command downloads and runs Zed's official installer. Account sign-in and accepting invitations still require manual clicks.

### 2. Sign in with GitHub

1. Open Zed and **sign in with GitHub**.
2. Ned sends Josh his **GitHub username** so Josh can add him as a contact.

### 3. Connect to the shared project

Open Zed's **Collaboration Panel**:

| Platform | Shortcut |
| --- | --- |
| Windows / Linux | `Ctrl+Shift+C` |
| macOS | `Cmd+Shift+C` |

**Josh — host**

1. Open the `NedJoshCollab` project in Zed.
2. Under **Contacts**, click **+**, search for Ned's GitHub username, and send a request.
3. Once Ned accepts, use the **...** menu beside his name to start a private call.
4. **Share this project** from the call.

**Ned — guest**

1. Accept Josh's contact request.
2. Answer the Zed call.
3. Open the shared **NedJoshCollab** project.

**That's it — changes appear live for both people.** No pushing or pulling is needed to see edits during the shared session.

> [!IMPORTANT]
> Josh's computer hosts the working copy and runs the project. Keep the host computer and shared Zed session online. Have the host handle Git operations so two people or agents aren't changing branches or committing at the same time.

> [!CAUTION]
> Only share with trusted people. Collaborators can access files within the shared project.

Need help? See the official [Zed collaboration guide](https://zed.dev/docs/collaboration).

## AI setup

1. Open Zed's **Agent Panel** using the **✨** icon.
2. Connect your own AI account or model provider.
3. Choose a model and start a coding thread.

AI access and any usage charges are separate from project sharing. Configure credentials locally; **never put API keys in this repository**.

### Automatic tool approval — optional

Open Zed's **Settings**, search for **Tool Permissions**, and set the default to **Allow**.

Alternatively, merge this into your existing **user settings JSON** without replacing other settings:

```json
{
  "agent": {
    "tool_permissions": {
      "default": "allow"
    }
  }
}
```

This is a **personal setting**, not a shared repository setting. Each person chooses it on their own computer.

> [!WARNING]
> Auto-approval lets an agent modify or delete files and run commands. Use it only with projects you trust. Tool-specific rules, built-in protections, and terminal sandbox or network permissions can still prompt or block actions.

External agents may have their own permission settings. See [Zed tool permissions](https://zed.dev/docs/ai/tool-permissions) for details.

## GitHub access

Project repository: **[Parris-Tech-Services/NedJoshCollab](https://github.com/Parris-Tech-Services/NedJoshCollab)**

**Live sharing and GitHub permissions are separate.** To let Ned push code or work independently, a repository administrator should:

1. Open the repository's **Settings → Collaborators and teams**. The label may be **Collaborators**.
2. Invite Ned using his GitHub username and grant **Write** access.
3. Have Ned accept the invitation on GitHub.

**Write access is enough to contribute code** — administrator access isn't needed. If organization policy blocks the invitation, ask an organization owner to grant access.

## Working independently

Want to work when Josh is offline? Install [Git](https://git-scm.com/downloads), accept any required repository invitation, then clone the project:

```sh
git clone https://github.com/Parris-Tech-Services/NedJoshCollab.git
```

Open the resulting `NedJoshCollab` folder in Zed.

| Working together live | Working independently |
| --- | --- |
| Join one shared Zed project. | Use your own local clone. |
| See each other's edits immediately. | Share changes through GitHub. |
| The host handles Git operations. | Each person uses a separate branch and opens a pull request to `main`. |

> [!NOTE]
> A separate clone does **not** synchronize edits live. Joining the shared Zed project and opening your own clone are different workflows.

## Collaboration rules

- **Split the work:** agree on separate tasks and files before starting multiple agents.
- **Avoid collisions:** don't send two agents to rewrite the same file. Take turns on shared configuration and dependency files.
- **Review before sharing:** run the relevant checks and review changes before committing.
- **Publish finished work:** commit and push completed task changes to GitHub by default, unless asked to keep them local. Don't include anyone else's in-progress changes or force-push over their work.
- **Keep Git coordinated:** during a live session, the host commits and pushes reviewed changes.
- **Protect secrets:** use ignored `.env` files and commit only placeholder values in `.env.example`.

`AGENTS.md` gives coding agents the same collaboration rules.

---

**Project status:** no application framework has been chosen yet. Decide what we're building before adding an app scaffold.

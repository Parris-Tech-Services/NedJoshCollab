# NedJoshCollab
Ned — quick setup for coding with Josh
1. Install Zed
Easiest on any computer: download and run the installer from https://zed.dev/download.
Or use an automatic install command for your operating system:
Windows — paste into PowerShell:
winget install -e --id ZedIndustries.Zed --accept-source-agreements --accept-package-agreements
Mac — if Homebrew is already installed:
brew install --cask zed
Linux — paste into Terminal:
curl -f https://zed.dev/install.sh | sh
The Linux command downloads and runs Zed’s official installer.
2. Sign in
Open Zed and sign in with GitHub. Send Josh your GitHub username so he can add you.
Account sign-in and accepting invitations still require your clicks; an installer cannot do those for you.
3. Join Josh’s live project
Open the Collaboration Panel:
Windows/Linux: Ctrl+Shift+C
Mac: Cmd+Shift+C
Accept Josh’s contact request.
Answer his Zed call.
Open the shared NedJoshCollab project.
Done—you’re editing the same live files. No Git installation or repository cloning is needed for this mode. Josh needs to keep his computer and shared Zed session online.
4. Enable your AI assistant
Open Zed’s Agent Panel using the ✨ icon and connect your own AI provider/account. AI access and any usage charges are separate from project sharing.
If you want automatic tool approval, open Settings, search Tool Permissions, and set the default to Allow. This allows broad file editing and command execution; sandbox restrictions may still apply.
Optional: your own independent project copy
For working when Josh is offline, install Git, accept any GitHub repository invitation, then run:
git clone https://github.com/Parris-Tech-Services/NedJoshCollab.git
Open the resulting NedJoshCollab folder in Zed. A separate clone does not sync edits live—use branches and pull requests for independent work.
Josh’s part: keep this project open, add Ned in Collaboration, start a call, and share the project.

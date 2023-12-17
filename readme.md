# Custom Theme for Oh My Posh

This custom theme integrates [Oh My Posh](https://ohmyposh.dev/) with custom fonts from [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts/) for an enhanced PowerShell experience on Windows.

## Installation

### Prerequisites

- [Windows Package Manager](https://github.com/microsoft/winget-cli) (`winget`) installed.
- [Nerd Fonts](https://github.com/ryanoasis/nerd-fonts/) installed.

### Steps

1. **Install Oh My Posh via Windows Package Manager:**

   ```bash
   winget install JanDeDobbeleer.OhMyPosh -s winget
   ```
2. **Install and Apply Nerd Fonts:**

   - Download and install the desired Nerd Font. Follow the instructions provided in the Nerd Fonts repository for installation.

3. **Configure Microsoft.PowerShell_profile.ps1:**

   - Add configurations for Oh My Posh in your PowerShell profile (Microsoft.PowerShell_profile.ps1). Use the following command to open the profile:

   ```powershell
   notepad $PROFILE
   ```

   - Add the following lines to your profile to load Oh My Posh:

   ```powershell
   Import-Module posh-git
   Import-Module oh-my-posh
   Set-Theme YourCustomThemeName
   ```
   Replace YourCustomThemeName with the name of the custom theme you've created.

4. **Font Visibility in PowerShell:**

   - In case the selected font is not visible in PowerShell, refer to the instructions provided in [this link](https://github.com/microsoft/WSL/issues/1517) to troubleshoot and ensure the font is correctly installed and visible.

5. **Bash Style Auto Suggestion for PowerShell**

   - To enable Bash-style auto-suggestions in PowerShell, follow this  [tutorial](https://github.com/microsoft/winget-cli).

**Contributing**

If you'd like to contribute to this project, please fork the repository, make your changes, and submit a pull request.
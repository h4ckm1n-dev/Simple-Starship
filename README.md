# Simple Starship

![Capture d’écran du 2024-04-07 13-53-13](https://github.com/h4ckm1n-dev/Starship-Ultimate/assets/97511408/14bf0f81-1134-4d94-858d-1a0667f46346)

This repository hosts a template for configuring the Starship prompt, a fast, customizable prompt for any shell. Starship works across most shells and operating systems. This template includes a variety of configurations to customize your terminal prompt for a more informative and visually appealing experience.

(Starship Prompt)[https://starship.rs/]

## Configuration overview 

Configuration Overview
The configuration file starship.toml is located in your ~/.config directory. This file controls the appearance and behavior of the Starship prompt. Here's a brief overview of the included configurations:

**Schema**: Get editor completions based on the config schema by specifying the $schema.

**New Line**: Adds a blank line between shell prompts for better readability.

**Command Timeout**: Adjusts the timeout duration for commands.

**Prompt Format**: Customizes the overall format of the prompt.

**Character**: Changes the default prompt symbols for success and error states.

**Username**: Shows the username with customization options for style and always showing it.

**Hostname**: Customizes the hostname display with options for SSH only.

**Local IP**: Displays the local IP address when in an SSH session.

**Directory**: Customizes how the current directory is displayed, including truncation length and symbols.

**Memory Usage**: Shows system memory usage with options for disabling, threshold, symbol, and style.

**Custom Git Repo Name**: Displays the name of the git repository.

**Git Branch**: Shows the current git branch with customization options.

**Git Status**: Displays various git status indicators.

**Git Commit**: Shows the current commit hash.

**AWS**: Displays the AWS profile and region.

**Kubernetes**: Shows the current Kubernetes context and namespace.

**Terraform**: Displays Terraform workspace and version.

**Vagrant**: Shows the Vagrant version.

**Docker Context**: Displays the current Docker context.

**Helm**: Shows the Helm version.

**Programming Languages**: Customization options for Python, Node.js, Ruby, Go, and Lua.

## Enabling Options
To enable or customize these configurations:

Ensure you have Starship installed. Visit Starship's official website for installation instructions.
Open your ~/.config/starship.toml file in your preferred text editor.
Uncomment (remove the # at the beginning of the line) or add the configuration options you wish to change or enable.
Save the file and restart your terminal for the changes to take effect.

## Example: Enabling Memory Usage
To enable the memory usage module with a threshold, ensure your configuration includes:

```bash
[memory_usage]
disabled = false
threshold = -1 # Show for any usage level
symbol = ' '
style = 'bold dimmed red'
```
Starship is highly customizable. For a full list of configuration options, refer to the Starship Configuration page. You can adjust the format, style, disabled flags, and much more for each module to fit your preferences.

Enjoy a more informative and visually appealing terminal experience with Starship!

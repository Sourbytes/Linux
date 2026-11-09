Hyprland Dotfiles

A personal Hyprland configuration repository, maintained primarily as a backup and configuration reference. If you find something useful here and want to use it on your own system, feel free to do so.
This repository contains my Hyprland setup, including the application launcher, status bar, terminal, shell configuration, notification daemon, themes, and other desktop customizations.
The goal is simple: keep the configuration organized, reproducible, and easy to restore after a fresh installation.

---


**Screenshots**

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/a905cbe2-186f-47e0-972d-0aa1672c53d9 "width="100%" alt="Hyprland Screenshot 1"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/067edc3f-86f6-43ea-850b-241f059a75e6 "width="100%" alt="Hyprland Screenshot 2"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/fafdeb6f-4ada-42d3-aa95-2cdef6718877 "width="100%" alt="Hyprland Screenshot 2"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/054cd4c4-ec79-4a79-8c2b-52b7b47e75fb "width="100%" alt="Hyprland Screenshot 4"/>
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center">
      <img src="https://github.com/user-attachments/assets/b9681ec2-c03d-4ddd-86bf-7aa023a81f6c"/>
    </td>
  </tr>
</table>


---


Overview

This setup is built around Hyprland, a dynamic tiling Wayland compositor.

The primary applications and components used in this configuration are:

Component| Application
Window Manager| Hyprland
Application Launcher| Fuzzel
Status Bar| Waybar
Terminal Emulator| Kitty
Shell| Fish
Notification Daemon| SwayNC
Shell Theme| Fish theme configuration
Terminal Theme| Kitty theme configuration

Each application has its own configuration, allowing individual components to be modified without unnecessarily affecting the rest of the desktop environment.

---

Requirements & Dependencies

Before using these dotfiles, make sure the required applications are installed on your system.

1. Hyprland

Hyprland is the core of this setup. It handles window management, workspaces, animations, keybindings, and other compositor-related functionality.

Without Hyprland, well, there isn't much of a Hyprland configuration to talk about.

Install the package:

sudo apt install hyprland

Note: Package availability depends on your distribution and repositories. Use the appropriate installation method for your system.


2. Fuzzel — Application Launcher

Fuzzel is used as the application launcher.

It provides a lightweight and Wayland-native interface for launching installed applications. Its configuration controls the launcher appearance and behavior.

Make sure Fuzzel is installed before using the launcher configuration.

3. Waybar — Status Bar

Waybar provides the desktop status bar.

It is responsible for displaying system information and desktop-related indicators, such as workspaces, clock, and other configured modules.

The Waybar configuration and styling are included in this repository.

4. Kitty — Terminal Emulator

Kitty is the terminal emulator used in this setup.

The repository includes Kitty configuration and theme customizations. These control the terminal's appearance and behavior.

Install Kitty before applying its configuration.


5. Fish — Shell

Fish (Friendly Interactive Shell) is used as the default interactive shell in this configuration.

Fish provides useful interactive features, syntax highlighting, autosuggestions, and a convenient scripting environment.

The repository includes Fish configuration and theme customizations.

Install Fish before applying the shell configuration.


6. SwayNC — Notification Daemon

SwayNC (Sway Notification Center) handles desktop notifications.

It provides notification management and a notification center, with customization options for its appearance and behavior.

The corresponding configuration and styling are included in this repository.

---

Installation

Step 1 — Install Dependencies

Install all the required applications before copying any configuration files.

At minimum, you will need:

- Hyprland
- Fuzzel
- Waybar
- Kitty
- Fish
- SwayNC

Make sure the applications launch correctly before proceeding.

Step 2 — Back Up Existing Configurations

Before replacing anything, back up your existing configuration directory.

cp -r ~/.config ~/.config.backup

This is especially important if you already have customized configurations.

Step 4 — Apply the Configurations

Copy the required configuration directories into your local configuration directory.

For example:

cp -r hypr ~/.config/
cp -r waybar ~/.config/
cp -r kitty ~/.config/
cp -r fish ~/.config/
cp -r swaync ~/.config/
cp -r fuzzel ~/.config/

Adjust the directory names according to the actual repository structure.

Step 5 — Review and Customize

After copying the files, review the configurations before launching everything.

Pay particular attention to:

- Monitor configuration and resolution.
- Keyboard layouts.
- Application launch commands.
- Keybindings.
- Wallpaper paths.
- Terminal and shell settings.
- Theme and font dependencies.
- Any hardcoded paths referencing the original system.

Not every configuration is universally portable. Some adjustments may be necessary depending on your hardware, distribution, and installed applications.

---

Themes & Appearance

This repository also includes theme customizations for the applications used in this setup.

The primary theme-related configurations include:

- Kitty terminal appearance.
- Fish shell theme.
- Waybar styling.
- Fuzzel launcher appearance.
- SwayNC notification styling.
- Hyprland visual settings.

Some visual elements may depend on additional fonts, icons, GTK themes, or other assets.

If something looks different from the screenshots or expected appearance, check whether the required theme dependencies are installed.

---

Important Notes

- These configurations are primarily maintained for personal backup and restoration.
- The setup may reflect my personal hardware, software preferences, and workflow.
- Not every configuration is guaranteed to work out of the box on every distribution.
- Review the configuration files before replacing your existing ones.
- Install all required dependencies before starting the desktop session.
- Feel free to modify, adapt, or reuse any part of the configuration.

A configuration file is supposed to save time, not introduce a new debugging career.

---

Credits

Thanks to the developers and maintainers of the open-source projects used in this setup.

- Hyprland
- Fuzzel
- Waybar
- Kitty
- Fish
- SwayNC

All respective projects retain their original licenses and copyrights.

---

Use it, modify it, break something, fix it, and make it your own.


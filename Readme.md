# Waybar Configuration for my System76 Lemur Pro

This repository contains my custom configuration files for [Waybar](https://github.com/Alexays/Waybar), a highly customizable status bar for Wayland, specifically tailored for use on my System76 Lemur Pro running Pop!_OS with Sway.

## System Information

- **Device:** System76 Lemur Pro
- **Operating System:** Pop!_OS

## Key Features

- **Custom Modules:** Custom modules have been created for displaying system information such as CPU usage, memory usage, battery status, and network status.
- **Responsive Layout:** The bar layout is optimized for the Lemur Pro's screen size, with responsive behavior for different screen resolutions.
- **Theming:** The configuration includes a custom theme that blends well with the Sway environment, ensuring a cohesive visual experience.

## Modules Configured

The following modules are configured in this setup:

- **CPU Usage:** A graphical representation of the CPU load.
- **Memory Usage:** Displays the current memory usage.
- **Battery:** Shows the current battery status with an icon and percentage.
- **Network:** Indicates the status of your network connection, including Wi-Fi signal strength.

## Installation

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/yourusername/waybar-config.git ~/.config/waybar
    ```

2. **Install Dependencies:**

    Ensure you have the necessary packages installed. For Pop!_OS, you can use:

    ```bash
    sudo apt install waybar
    ```

3. **Copy the Configuration Files:**

    Copy the configuration files to your Waybar config directory:

    ```bash
    cp -r ~/.config/waybar/* ~/.config/
    ```

4. **Start Waybar:**

    Waybar should automatically start with Sway. If not, you can manually start it by running:

    ```bash
    waybar
    ```

## Customization

### Config File

- The main configuration file is `~/.config/waybar/config`.
- It is written in JSON format, with comments to explain each section.
- You can modify the order of modules, add new modules, or change the update intervals for existing ones.

### Style File

- The style for Waybar is controlled via the `~/.config/waybar/style.css` file.
- It uses standard CSS, so you can easily change colors, fonts, and layout.
- You can create different styles for different monitors if needed.

### Module Customization

Each module in Waybar has its own settings, which can be customized within the config file. For example:

- **Clock Module:**
  - Modify the date and time format.
- **Battery Module:**
  - Customize icons based on battery percentage.
- **Network Module:**
  - Change the update interval or display format.

## Troubleshooting

- **Waybar doesn't start:** Ensure the configuration syntax is correct. Run Waybar from the terminal to see any error messages:
  
  ```bash
  waybar -l debug


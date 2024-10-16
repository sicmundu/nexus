# Nexus Node Installation Wizard - README

## Introduction

Welcome to the Nexus Node Installation Wizard! This script will guide you through the process of installing, managing, and updating the Nexus Node on your system. The script also provides a management menu to help you manage your node efficiently after installation.

The wizard includes features such as automatic dependency installation, service file creation, and a menu for managing your node's status. You can use this wizard to install a new node, view logs, manage the node's status, and keep the script up-to-date.

## Prerequisites

Before running the installation script, ensure that you have:
- A Linux-based operating system (Ubuntu/Debian recommended).
- Sufficient privileges to run commands as `sudo`.

## Features

- **Automatic Dependency Installation**: Installs all required dependencies automatically.
- **Self-Update Feature**: Automatically checks for newer versions of the script and allows for easy updates.
- **Service Management**: Creates a systemd service for easy management of the Nexus Node.
- **User-Friendly Interface**: Easy-to-use menus with colorful indicators to make navigation intuitive.

## How to Use the Script

### Step 1: Download and Run the Script

To download the latest version of the script:

```bash
curl -O https://github.com/sicmundu/nexus/raw/refs/heads/main/nexus.sh
chmod +x nexus.sh
./nexus.sh
```

### Step 2: Follow the Wizard

The script will guide you through the following options:

1. **Install Node**: If the node is not installed, select this option to install the Nexus Node.
2. **Manage Node**: If the node is already installed, this menu allows you to:
   - Start, stop, or restart the node.
   - View node logs in real-time.
   - Check the current status of the node.
3. **Self-Update**: If a new version of the script is available, you will be prompted to update.

### Step 3: Manage the Nexus Node

After installation, you can manage the Nexus Node using the management menu. Options available include:
- **Start Node**: Start the Nexus Node service.
- **Stop Node**: Stop the Nexus Node service.
- **Restart Node**: Restart the Nexus Node service.
- **View Logs**: View real-time logs for troubleshooting.
- **Check Node Status**: Check if the node is currently running or stopped.

## Script Features Explained

- **Automatic Updates**: The script checks for new versions before running. If an update is available, you will be asked for confirmation before proceeding with the update.
- **Service File Creation**: The script automatically creates a systemd service file for the Nexus Node, which makes managing the node easier and more integrated with your system.
- **Color-coded Interface**: Messages are color-coded for better visual feedback:
  - Green for successful actions.
  - Red for errors or failed actions.
  - Yellow for warnings.
  - Blue for section separators.

## Example Usage

### Main Menu Options

- **Install Node**: Installs all necessary dependencies and the Nexus Node itself.
- **Manage Node**: Once the node is installed, use this to start, stop, or restart the node, and to view logs or check the node's status.
- **Exit**: Exit the wizard.

### Management Menu

- **Start Node**: Start the service for the Nexus Node.
- **Stop Node**: Stop the running Nexus Node service.
- **Restart Node**: Restart the node to apply new configurations.
- **View Logs**: Continuously view logs for monitoring the node.
- **Check Node Status**: See if the node is actively running or not.
- **Return to Main Menu**: Go back to the main options.

## Troubleshooting

- **Execution Failed**: If the script fails to execute a command, it will display a red error message. Check the logs to determine the cause.
- **Node Not Starting**: If the node fails to start, review the logs using the management menu to identify any errors.

## Updating the Script

The script includes a self-update feature that checks the version on the GitHub repository. If a newer version is available, it will prompt you to update. This ensures that you always have the latest features and improvements.

To manually update the script, use the following command:

```bash
./nexus-wizzard.sh
```

The script will check for updates automatically when it starts.

## Uninstalling the Node

To completely remove the Nexus Node from your system:
- **Stop Node** (if running).
- **Delete Node** from the main menu to remove all related files and configurations.

## License

This script is open-source and available under the MIT License.

## Contributions

Contributions are welcome! Feel free to fork the repository and submit pull requests with improvements or new features.

## Support

If you encounter issues or need help, please open an issue on the GitHub repository.

## Disclaimer

This script is provided "as is" without any warranties. Please use it at your own risk.


# Claude Desktop Settings

This repository contains my Claude Desktop configuration files for sharing settings across multiple machines.

## What's Included

- **settings.json** - Core Claude Desktop settings including permissions and preferences
- **agents/** - Custom agent configurations and prompts
- **commands/** - Custom command definitions

## Setup

1. Clone this repository to your Claude settings directory:
   ```bash
   # Backup your existing settings first
   mv ~/.claude ~/.claude.backup
   
   # Clone the repository
   git clone <repository-url> ~/.claude
   ```

2. Restart Claude Desktop to apply the new settings.

## Notes

- Machine-specific files like project references and shell snapshots are ignored via `.gitignore`
- The database file (`__store.db`) is excluded as it contains local state
- Personal todos and analytics data are not shared

## Contributing

Feel free to suggest improvements or report issues with these configurations.
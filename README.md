# My Team Timezone Dashboard

A simple, single-page web application designed to help teams coordinate across multiple timezones. This dashboard provides an at-a-glance view of your team members' local times, with a built-in meeting planner to easily find convenient times for everyone.

This entire application is contained within a single index.html file. It uses browser localStorage to save your tiles, meaning no database or backend is required.

## Features

- Local Time Header: Displays your current local time and timezone at the top of the page.
- Team Tiles: View all team members in a clean grid layout. Each tile shows:
- Team member's name (Title)
- IANA Timezone (e.g., "America/Los_Angeles")
- A large, live-updating digital clock (HH:mm format).
- Automatic Sorting: All tiles are automatically sorted by their UTC offset, from west (e.g., UTC-7) to east (e.g., UTC+3).
- Meeting Planner: Select a time in your local timezone, and the dashboard will instantly display the converted time on every team member's tile.
- Add / Edit / Delete: Easily manage your team list:
- Add: Click "+ Add Tile" to open a modal.
- Edit: Click the pencil icon on any tile to edit its title or timezone.
- Delete: Click the 'x' icon to remove a tile.
- Searchable Timezone Dropdown: The modal features a searchable dropdown menu with all IANA timezones to make selection fast and easy.
- Default Team: The app comes pre-loaded with a default team.
- Restore Team: Click the "Restore Team" button to add back any missing default team members without creating duplicates or removing your custom tiles.
- Persistent Storage: Your dashboard layout (all your added, edited, and deleted tiles) is saved automatically to your browser's localStorage.
- Fully Responsive: The layout adapts to all screen sizes, from mobile phones to desktops.

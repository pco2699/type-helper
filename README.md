# Type Help Puzzle Solver

A drag-and-drop puzzle-solving assistant for the Type Help mystery game. Track character locations across 26 time periods, freeze confirmed answers, and generate formatted output codes.

## Features

- **26 Time Periods** - Switch between time periods with automatic state inheritance
- **Drag-and-Drop Characters** - Move 11 characters between locations with intuitive drag-and-drop
- **Location Management** - Add/remove custom 2-letter location codes
- **Freeze Functionality** - Lock confirmed placements to prevent accidental changes
- **Character Naming** - Assign names to characters for easier tracking
- **Auto-Generated Output** - Automatically generates formatted codes as you work
- **Persistent Storage** - All progress saved to localStorage automatically

## Usage

1. Open `index.html` in a web browser
2. Select a time period from the dropdown
3. Drag characters from the "?? (Undecided)" area to location boxes
4. Click the lock icon to freeze confirmed placements
5. Use "+ Add Location" to add new 2-letter location codes
6. Enter character names at the bottom for easier identification
7. Copy the auto-generated output as needed

## Output Format

```
{timePeriod}-{location}-{character1}-{character2}-...
```

Example:
```
01-KI-1-3
01-EN-2-5-7
```

## Data Persistence

All data is automatically saved to localStorage under the key `typeHelpPuzzleSolver`. Data persists across browser sessions.

To reset all data, open browser DevTools and run:
```javascript
localStorage.removeItem('typeHelpPuzzleSolver');
location.reload();
```

## Deployment

This is a single HTML file with no dependencies. To deploy:

1. Push to GitHub
2. Enable GitHub Pages in Settings > Pages
3. Select "Deploy from branch" > main branch > root folder
4. Access at `https://{username}.github.io/{repo-name}/`

## License

MIT

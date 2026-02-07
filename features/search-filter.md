# Search & Filter

Find any commit, author, or file in seconds with Gitux's powerful search and filter tools.

## Overview

Large repositories can have thousands of commits. Gitux gives you multiple ways to quickly narrow down exactly what you're looking for — whether it's a specific commit message, a particular author's work, commits within a date range, or the history of a single file.

## The Search Bar

The search bar sits above the commit graph. Click **Search & Filter** (or press `Ctrl+F`) to expand it.

```
┌──────────────────────────────────────────────────────────────┐
│ 🔍 Search & Filter ▼  │ Search commits...                    │
├──────────────────────────────────────────────────────────────┤
│ 🔍 Search commit messages...    │ 📄 Search files → history... 📁│
│ 👤 All Authors ▼  FROM [date]  TO [date]    [Clear Filters]  │
└──────────────────────────────────────────────────────────────┘
```

### Collapsed Mode
When collapsed, a quick search input is always visible for fast commit message searching without expanding the full panel.

### Expanded Mode
Click the bar or press `Ctrl+F` to reveal the full filter panel with all options.

## Commit Message Search

Type in the search field to instantly filter commits:

- Matches against **commit messages**
- Also matches **commit hashes** (short or full)
- **Highlights** matching text in the commit graph
- Results update as you type

### Example
Searching for `login` shows only commits with "login" in the message, such as:
- "feat: add login page"
- "fix: login timeout on slow connections"
- "refactor: extract login validation"

## Author Filter

Click the **All Authors** dropdown to filter by a specific contributor:

- Lists all unique authors from loaded commits
- Click an author to show only their commits
- Click **All Authors** to clear the filter
- Active filter is highlighted in accent colour

Great for:
- Reviewing a team member's recent work
- Finding your own commits
- Understanding who worked on what

## Date Range Filter

Use the **From** and **To** date pickers to narrow commits to a time window:

- Click the date field to open the calendar picker
- Set just a **From** date to see everything after that date
- Set just a **To** date to see everything before it
- Set both for a specific range
- Useful for release reviews, sprint retrospectives, or finding "what changed last week"

## File Search

The file search input lets you find any tracked file in the repository:

1. Type a filename or path fragment
2. Matching files appear in a dropdown
3. Use **↑/↓** arrow keys to navigate results
4. Press **Enter** or click to open that file's **complete commit history**

### Example
Type `Login` to see:
- `src/components/Login.tsx`
- `src/tests/Login.test.ts`
- `src/styles/login.css`

Click any result to instantly open the [File History](/features/file-history) panel for that file.

## File Browser

Click the **folder icon** (📁) on the right side of the file search input to open the full file browser modal.

```
┌─────────────────────────────────────┐
│ 📁 Browse Files          142 files  │
├─────────────────────────────────────┤
│ ▶ 📁 src                            │
│   ▶ 📁 components                   │
│     ▶ 📁 CommitGraph                │
│       📄 CommitGraph.tsx        🕐  │
│       📄 CommitRow.tsx          🕐  │
│       📄 SearchFilterBar.tsx    🕐  │
│   ▶ 📁 store                        │
│   📄 App.tsx                    🕐  │
│ ▶ 📁 electron                       │
│ 📄 package.json                 🕐  │
├─────────────────────────────────────┤
│ Click a file to view its history    │
└─────────────────────────────────────┘
```

- **Folders** are sorted first, shown with expand/collapse arrows
- **Files** show a clock icon on hover indicating "view history"
- Click any file to open its full [File History](/features/file-history)
- The tree mirrors your repository's actual directory structure

## Combining Filters

All filters work together. For example:
- Search for `auth` **+** Author: "Jane" **+** From: last month
- This shows only Jane's authentication-related commits from the past month

The status bar shows: **"Showing 12 of 847 commits"** so you always know how many results match.

## Clearing Filters

- Click **Clear Filters** to reset everything at once
- Or clear individual filters (X button on search, reset author dropdown, clear dates)
- The graph instantly returns to showing all commits

## Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+F` | Toggle search & filter panel |
| `Escape` | Clear search text or close panel |
| `↑` / `↓` | Navigate file search results |
| `Enter` | Select file from search results |

## Tips

### Start Broad, Then Narrow
Begin with a text search, then add author or date filters to refine results.

### Use File Search for Quick History
Instead of finding a file in the staging panel or commit details, type its name directly in the file search to jump straight to its history.

### Browse the File Tree
For unfamiliar repositories, use the file browser to explore the project structure and quickly check the history of any file.

### Hash Search
If someone shares a commit hash, paste it into the search field to find that exact commit instantly.

## Related

- [Commit Graph](/features/commit-graph) — The visual history view
- [File History](/features/file-history) — Tracking file changes over time
- [Keyboard Shortcuts](/features/keyboard-shortcuts) — All shortcuts

# GitHub Pages Setup

## Goal

Host the Course Business Manager dashboard as a normal web link that can be opened from any device.

## Files GitHub Pages Will Use

- `index.html` redirects visitors to the dashboard.
- `operations/dashboard.html` contains the dashboard UI.
- `operations/task_board.md` contains the Markdown task board.
- `instructions/work_stream_complexity_map.md` contains the work-stream complexity map.

## Setup Steps

1. Create a new GitHub repository.
2. Upload this project folder to the repository.
3. In GitHub, open the repository settings.
4. Go to **Pages**.
5. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
6. Save.
7. Wait for GitHub Pages to publish the site.
8. Open the published URL.

## Expected URL Format

The dashboard URL will usually look like this:

```text
https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/
```

The root URL opens `index.html`, which redirects to:

```text
https://YOUR_USERNAME.github.io/YOUR_REPOSITORY_NAME/operations/dashboard.html
```

## Update Workflow

When the project changes:

1. Update `operations/task_board.md`.
2. Update the task list inside `operations/dashboard.html`.
3. Commit and push the changes to GitHub.
4. GitHub Pages updates the published dashboard automatically.

## Privacy Note

GitHub Pages from a normal free public repository is public. Do not publish private student data, private sales data, credentials, API keys, or personal contact details in the dashboard.


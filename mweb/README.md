# Railway Node.js Starter

This is a minimal Node.js + Express application structured for deployment to Railway from a GitHub repository.

## Files

- `server.js` — Express server
- `package.json` — dependencies and `npm start` command
- `index.html` — webpage
- `style.css` — styling
- `script.js` — browser JavaScript
- `.gitignore` — excludes local dependencies and secrets

## Deploy from GitHub

1. Create a GitHub repository.
2. Upload these files to the repository root.
3. In Railway, create a new project and choose the GitHub deployment option.
4. Select the repository and deploy.
5. Railway should detect the Node.js project from `package.json` and use the `start` script.

The server listens on `process.env.PORT` and binds to `0.0.0.0`.

## Health check

After deployment, the app exposes:

`/health`

It returns `OK`.

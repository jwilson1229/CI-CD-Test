# CI/CD Pipeline with GitHub Actions & Render

## Overview
This project uses **GitHub Actions** for automated testing and **Render** for deployment.

## Workflow
- **Cypress Tests:** Run automatically on PRs to `develop`.
- **Deployment:** Auto-deploys to Render when `develop` merges into `main`.

## Setup
1. **Clone the repository:**
   ```sh
   git clone <repo-url>
   cd <project-folder>
   ```
2. **Install dependencies:**
   ```sh
   npm install
   ```
3. **Run locally:**
   ```sh
   npm start
   ```

## CI/CD Steps
1. Create a **Render Deploy Hook** and disable auto-deploy.
2. Add `RENDER_DEPLOY_HOOK` as a **GitHub Secret**.
3. Push changes to `develop` → Tests run.
4. Merge `develop` into `main` → Auto-deploy triggers.

## Testing
Run Cypress tests manually:
```sh
npx cypress open
```

## Contribution
1. Create a branch: `git checkout -b feature-branch`
2. Make changes, commit, and push.
3. Open a Pull Request to `develop`.

## License
MIT License.

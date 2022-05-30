![](https://motion4life.github.io/github-actions//workflows/CI/badge.svg?branch=develop&event=push)

# Presentation

### Init template

1. Changed master to main
2. Add develop + github-pages branch
3. Add .github/workflows/example.yml
4. Add CODEOWNERS
5. npm install prettier --save-dev + .prettierrc, .prettierignore
6. npm install semantic-release --save-dev + release.config.js
7. npm install gh-pages --save-dev
8. Add format: scripts
9. Add README badge

### Scripts

```bash
npm run test
npm run test -- --coverage
npm run build
npm run format:check
npm run format:write
npm run deploy
```

### Github settings

Notifications: Actions

### Github repo settings

Pages: GitHub Pages
Branch: Branch protection rules

### Pipeline pull (develop / main)

install dependencies
check code formatting
run automated tests
upload code coverage as an artifact
cache dependendies

### Pipeline merge (develop / main)

install dependencies
check code formatting
run automated tests
upload code coverage as an artifact
build project
upload build as an artifact
create a release (main)
deploy to github pages
cache dependendies

### Overview

1. Simple example (bash)
2. Debug Secrets
3. Actions Marketplace
4. Checkout action
5. Environemt variables
6. Events and Cron jobs
7. Filtering
8. Action env + Job env + Step env
9. Custom secrets
10. Matrix
11. Docker
12. CI-Pipeline

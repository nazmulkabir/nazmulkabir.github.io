# Personal website
Personal website of [Md Nazmul Kabir Sikder](https://nazmulkabir.com)

Build with minification:
hugo --minify
git status
git add .
git commit -m "update collaborator"
git push origin main
Refresh gh-pages worktree and push:
cd /private/tmp/gh-pages
find . -maxdepth 1 -mindepth 1 ! -name '.git' ! -name '.nojekyll' -exec rm -rf {} +
cp -a /Users/nazmul/Library/CloudStorage/OneDrive-VirginiaTech/Codebase/nazmulkabirdotcom/public/. /private/tmp/gh-pages/
git add -A
git commit -m "Publish Hugo build"
git push origin gh-pages

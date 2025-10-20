# Cristian's SNHU Computer Science ePortfolio

This repository powers the [GitHub Pages](https://pages.github.com/) site that will showcase the artifacts and narratives for the SNHU Computer Science capstone. The site is intentionally structured with placeholders so final content can be dropped in quickly once each milestone is complete.

## Repository Structure

- `index.md` – Landing page for the professional self-assessment.
- `artifacts.md` – Overview of enhancement categories with quick links.
- `artifacts/` – Dedicated pages for software design & engineering, algorithms & data structures, and databases enhancements.
- `code-review.md` – Placeholder for the informal code review walkthrough video and supporting resources.
- `_includes/portfolio-nav.html` – Shared navigation bar rendered on every page.
- `assets/css/style.scss` and `_sass/custom.scss` – Custom styling layered on top of the selected GitHub Pages theme.

## Local Development

### Prerequisites

1. Install Ruby 3.1 or newer. On Windows, download the latest [RubyInstaller](https://rubyinstaller.org/) package and, when prompted, run the `ridk install` step so native dependencies can be compiled.
2. Install Bundler if it is not already available:

   ```bash
   gem install bundler
   ```

3. (Windows Git Bash only) Restart Git Bash after installing Ruby so the `bundle` command is added to your `PATH`.

### Run the site locally

From the root of the repository:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000` in a browser. GitHub Pages will automatically build the site using the configuration defined in `_config.yml` when changes are pushed to the `main` branch.

### No-Ruby preview option

If installing Ruby or running `bundle install` is blocked in your environment (for example, Git Bash cannot find the `bundle` command), you can still review the layout using the static HTML snapshots in the `preview/` directory:

1. Open `preview/index.html` directly in a browser to click through the self-assessment, artifacts, and code review placeholders.
2. Alternatively, run a lightweight server from the repository root to mirror the GitHub Pages URLs:

   ```bash
   python -m http.server 4000 --directory preview
   ```

   Then visit `http://localhost:4000/index.html` (or `/artifacts.html`, `/code-review.html`, etc.) to see the same structure you will publish to GitHub Pages.

> The preview files pull the published Tactile theme CSS from GitHub so you can validate spacing, typography, and navigation without completing the Ruby toolchain setup.

## Publish to `CrisxEsco.github.io`

Follow these steps the first time you want to publish (or republish) the site to your GitHub Pages domain:

1. **Create the remote repository**
   * Sign in to GitHub and create a public repository named `CrisxEsco.github.io` under your account.
   * Leave the repository empty—do not initialize it with a README, `.gitignore`, or license—because this project already contains those files.

2. **Connect your local clone to GitHub**
   * From a terminal in this project directory, add the GitHub remote and verify that your `main` branch is up to date:

     ```bash
     git remote add origin git@github.com:CrisxEsco/CrisxEsco.github.io.git
     git branch -M main
     git push -u origin main
     ```

   * If you prefer HTTPS instead of SSH, replace the remote URL accordingly.

   * Working from another branch? Publish it once with:

     ```bash
     git push --set-upstream origin CrisxEsco.github.io
     ```

     After the upstream is set, `git push` will update the branch and you can open a pull request on GitHub before merging to `main`.

3. **Enable GitHub Pages (first publish only)**
   * Open the repository settings on GitHub, scroll to the **Pages** section, and set the source to the `main` branch with the `/ (root)` folder. Save the changes.

4. **Deploy updates**
   * After editing any files, commit them locally and push to `main`. GitHub Pages automatically rebuilds the site within a minute or two. Refresh `https://CrisxEsco.github.io/` to see the updates.

Troubleshooting tips:

- If the site does not appear after pushing, confirm that the Pages settings still point to the `main` branch and check the **Actions** tab for any build errors.
- When using SSH, ensure that your public key is added to your GitHub account and that the SSH agent is running before pushing.

## Next Steps

1. Record and upload the informal code review video, updating `code-review.md` with the embed and resources. Swap the iframe's
   `srcdoc` attribute for a direct `src` pointing to your hosted video (for example, an unlisted YouTube link).
2. Complete each enhancement and replace the placeholder text within the corresponding artifact page.
3. Write the professional self-assessment and update the landing page narrative.
4. Add links to original and enhanced source code, repositories, and documentation as you finalize the portfolio.

Feel free to add additional pages or resources (résumé, contact information, etc.) to further personalize the ePortfolio.

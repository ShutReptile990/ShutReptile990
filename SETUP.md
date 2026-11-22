# MIDNIGHT SKYLINE – setup

1. Create a **public** GitHub repository with the exact same name as your GitHub username (for example `octocat/octocat`).
2. Upload this package's `README.md`, `assets/` folder, and `.github/workflows/profile-3d.yml` to that repository. You can place the generated graph assets later; GitHub Actions creates them.
3. Search and replace `ShutReptile990` in `README.md` with your exact GitHub username. Replace **Your Name**, sample project links, `YOUR_LINKEDIN`, `YOUR_PORTFOLIO_URL`, and `YOUR_EMAIL` as appropriate.
4. In the profile repository, open **Actions → Generate 3D Contribution City → Run workflow**. Allow GitHub Actions to create and commit `profile-3d-contrib/profile-night-rainbow.svg`. Make sure workflow permissions can write repository contents.
5. Refresh your public GitHub profile. The skyline isn't visible until the first successful Action run, and the GitHub stats cards depend on the external stats service.

**Notes**
- The headline and project districts are custom SVG assets stored locally; the 3D contribution block is genuinely generated from your public GitHub activity.
- GitHub sanitizes custom CSS and JavaScript in README files. These designs rely on supported Markdown, HTML and SVG images instead.
- To adjust the theme, edit the SVG files in `assets/`.
- Each theme is independently installable. Do not upload multiple themes to the same repository simultaneously unless you're purposely overwriting one theme with another.
- This is an original recreation inspired by the Contribution City idea, not an export of GitSkins' proprietary template.
- The repository names, project URLs, display name, and tech stack are editable examples. No GitHub account data has been fetched.
- Sources for 3D graph generation: https://github.com/yoshi389111/github-profile-3d-contrib


## Fix for missing images

If the banner shows broken image alt text, `assets/banner.svg` is missing from your GitHub profile repository. Upload the *entire* `assets/` folder with the exact filenames and case (not just the README). Make sure `README.md` and `assets/` are at the same repository root.

If the 3D city image is missing, commit `.github/workflows/profile-3d.yml`, enable Actions write permissions, and run the workflow from Actions. It will generate the separate `profile-3d-contrib/` directory. On GitHub set **Settings → Actions → General → Workflow permissions → Read and write permissions**, if your repository policy allows it.

External stats images may be temporarily rate-limited or blocked by their provider; this is independent of missing local files.

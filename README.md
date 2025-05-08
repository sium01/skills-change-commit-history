<header>

<!--
  <<< Author notes: Course header >>>
  Read <https://skills.github.com/quickstart> for more information about how to build courses using this template.
  Include a 1280×640 image, course name in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Next to "About", add description & tags; disable releases, packages, & environments.
  Add your open source license, GitHub uses the MIT license.
-->

# Remove commit history

Accidental commits can be tricky to remove with Git. In this GitHub Skills course, you'll use BFG Repo-Cleaner to change the history of a Git repository. You can apply what you learn in this course to fully remove sensitive material from your own repository.

</header>

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Step 1: Removing sensitive data

_Welcome to "Change commit history"! :wave:_

We'll start by working with `.env` files. These files usually contain sensitive content. For this course, we'll work on removing that file and all traces in the Git history. The first step is to remove the file from repository. We'll alter the history later.

We'll assume you're using the command line, but you can complete the course using your preferred tooling.

**What is _sensitive content_?** Sensitive content is anything that is checked into your repository history that may put you or your organization at risk. This content usually comes in the form of credentials (i.e., passwords, access keys). The best practice for accidentally exposed sensitive content is to invalidate it (i.e., revoke a personal access token), completely remove it from all repository copies, and take measures to prevent future exposure.

See [Deleting a file on GitHub Docs](https://docs.github.com/en/repositories/working-with-files/managing-files/deleting-files-in-a-repository#deleting-a-file) if you need additional help removing a file.

### :keyboard: Activity: Remove `.env` in the project root directory

1. Open your terminal of choice, clone this repository, and switch to your repository directory.
   ```shell
   git clone <your-repository-url>
   cd <your-repository-name>
   ```
2. Delete `.env` from the root directory.
   ```shell
   git rm .env
   ```
3. Commit the removal of `.env`.
   ```shell
   git commit -m "remove .env file"
   ```
4. Push the removal to GitHub:
   ```shell
   git push
   ```
5. Wait about 20 seconds then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/en/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/change-commit-history) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2024 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>

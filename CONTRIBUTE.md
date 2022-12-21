# Contribution Guidelines

There are quite a few ways you could get involved with the Contributor Experience project. You can:

- join one of our [community calls](docs/about/calendar.qmd);
- join our [Zulip chat](https://contributor-experience.zulipchat.com/join/r3bbxavdymqbyjiu32mtqyqi/)
- share your ideas by [filing issues](https://github.com/contributor-experience/handbook/issues/new), submitting [Pull Requests](https://docs.github.com/en/pull-requests) or commenting on existing discussions;
- address issues filed by other contributors;
- review submitted PRs.

## How do I make a contribution to the Handbook?

Never made an open source contribution before? Wondering how contributions work in our project? Here's a quick rundown!

1. Find an issue that you are interested in addressing or a content page or feature that you would like to add.

2. Fork the [Contributor Experience Handbook repository](https://github.com/contributor-experience/handbook) to your GitHub profile. This means that you will have a copy of the repository `<github-username>/handbook.`

   To fork the repository, you can use the `Fork` button on the GitHub web interface for this repo.

3. Clone the repository to your local machine using:

   ```
   git clone https://github.com/<github-username>/handbook.git.
   ```

   This means you will now have a local copy of all the contents in the GitHub repository in your computer, under the `handbook` folder. You can rename this folder to any names you like - all the git-related information will be unchanged.

4. Add the `upstream` remote

   If you want to submit Pull Requests and share changes to the Handbook back to the community, you need to point git to the correct repos. You can do this by setting your [remote repositories](https://docs.github.com/get-started/getting-started-with-git/managing-remote-repositories).

   By convention, we will use the name `origin` to point to your fork of the repository, and we will call `upstream` the original Contributor Experience Handbook repo. To inform git, you can run the following command:

   ```
    git remote add upstream https://github.com/contributor-experience/handbook.git
   ```

   Now, if you run

   ```
   git remote -v
   ```

   you should see something like:

   ```
   origin  git@github.com:<github-username>/handbook.git (fetch)
   origin  git@github.com:<github-username>/handbook.git (push)
   upstream        git@github.com:contributor-experience/handbook.git (fetch)
   upstream        git@github.com:contributor-experience/handbook.git (push)
   ```

   This means you are all set!

5. (Optional) Pull the latest changes from the main repository if you think your fork is behind:

   ```
   git pull upstream main
   ```

6. Create a new branch and switch to it for your issue fix or content page using:

   ```
   git switch -c <branch-name>
   ```

   It is good practice to create a new branch for each new fix/improvement your are working on. This ensures the history of the changes to the project is more organized. You can name your branch anything - this does not interfere with the commit history.

7. Make the appropriate changes for the issue you are trying to address or the feature that you want to add

   This is when you write, fix existing content or otherwise do your magic ✨

8. Add the changes to the staging area and commit them to the branch you are working on

   ```
   git add <files-to-be-changed>
   git commit -m "<commit message>"
   ```

   where `<commit-message>` is a brief explanation of what you did.

9. Push the changes to the remote repository using:

   ```
   git push origin <branch-name>
   ```

10. Submit a **pull request** to the upstream repository

11. Title the **pull request** with a short description of the changes made

12. Wait for the pull request to be reviewed by a maintainer

13. Make changes to the pull request if the reviewing maintainer recommends them

14. Celebrate your success after your pull request is merged!

---

Thanks for taking the time to contribute! ❤️

Don't forget to leave a star 🌟
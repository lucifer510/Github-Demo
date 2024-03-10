## A Guide to Get Started (used to be the 4 step guide)

1. Check out [Andrei's videos on github](https://www.youtube.com/watch?v=JN63v_czZqI) if you haven't watched it already.

2. On the [GitHub page for this repository](https://github.com/lucifer510/Github-Demo.git), click on the button "Fork."

   ![fork image](https://upload.wikimedia.org/wikipedia/commons/3/38/GitHub_Fork_Button.png)

3. Clone _your forked repository_ to your computer:

   ![code ui](https://docs.github.com/assets/images/help/repository/code-button.png)

   For example, run this command inside your terminal:

   ```bash
   git clone https://github.com/<your-github-username>/Github-Demo.git
   ```

   **Replace \<your-github-username\>!**

   Learn more about [forking](https://help.github.com/en/github/getting-started-with-github/fork-a-repo) and [cloning a repo](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository).

4. Move to project directory:

   ```bash
   cd Github-Demo.git
   ```

5. Before you make any changes, [keep your fork in sync](https://www.freecodecamp.org/news/how-to-sync-your-fork-with-the-original-git-repository/) to avoid merge conflicts:

   ```bash
   git remote add upstream https://github.com/lucifer510/Github-Demo.git
   git pull upstream master
   ```

   If you run into a **merge conflict**, you have to resolve the conflict. There are a lot of guides online, or you can [watch this tutorial](https://www.youtube.com/watch?v=9ZRb01WhuoE&list=PL2HX_yT71umC0SWrtpzaXt0QzwhWyNI4c&index=4).

6. After adding the upstream and checking that all files are up to date, we now will create new branch before editing any files. There are two ways to do so:

   ```bash
   git checkout -b <branch-name>
   ```

   ```bash
   git branch <branch-name>
   git switch <branch-name>
   ```

7. On your computer, open your text editor, and add your name to the `CONTRIBUTORS.md` file.

- ⚠️ **IMPORTANT NOTE #1:** Add your name somewhere in the middle. Not at the top or bottom in order to avoid the chance of you getting a [merge conflict](https://www.youtube.com/watch?v=9ZRb01WhuoE&list=PL2HX_yT71umC0SWrtpzaXt0QzwhWyNI4c&index=4)!
- ⚠️ **IMPORTANT NOTE #2:** Please do **NOT** edit or remove other people from the list, even to fix their indentation etc. This will likely prevent your PR from being merged.

8. Add the changes with `git add`, `git commit` ([write a good commit message](https://chris.beams.io/posts/git-commit/), if possible):

   ```bash
   git add CONTRIBUTORS.md
   git commit -m "Add <your-github-username>"
   ```

   **Replace \<your-github-username\>!**

9. Push your changes _to your repository_:

   ```bash
   git push origin <branch-name>
   ```

10. Go to the GitHub page of _your fork_, and make a pull request:

    ![pull request image](https://docs.github.com/assets/cb-87213/images/help/pull_requests/pull-request-review-edit-branch.png)

    Read more about pull requests on the [GitHub help pages](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).


Finally, open-source projects use the following tools to organize discussion. Reading through the archives will give you a good picture of how the community thinks and works.

**Issue tracker**: Where people discuss issues related to the project.

**Pull requests**: Where people discuss and review changes that are in progress.
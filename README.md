# Outline

1. Installation
   * OSX installation:
     - Standard installation [`http://code.google.com/p/git-osx-installer`](http://code.google.com/p/git-osx-installer)
     - With Macports: `sudo port install git-core +svn +doc +bash_completion +gitweb`
   * Windows installation: [`http://msysgit.github.com/`](http://msysgit.github.com/)
2. Setup
   * Identity 
     - `$ git config --global user.name "Brian Jesse"`
     - `$ git config --global user.email user@example.com`
   * Configuration Files `~/.gitconfig`
3. Cloning
   * `git clone http://github.com/bajesse/git-workshop.git`
   * `cd git-workshop`
4. Checkout a branch
   * `git checkout dev`
5. Create a feature branch
   * `git checkout -b my-feature`
6. Modify files 
7. Check the status
   * `git status`
8. Stage files
   * `git add index.html`
   * `git add style.css`
   * `git status`
9. Commit staged changes
   * `git commit -m 'my message`
10. Check the log
    * `git log`
11. Merge into devel
    * `git checkout dev`
    * `git merge my-feature`
12. Demonstration of push
13. Create a release branch
    * `git checkout -b release-1`
    * Modify branch with bugfixes and commit to release
14. Merge into master and dev
    * `git checkout master`
    * `git merge release-1`
    * `git push origin master`
    * `git checkout dev`
    * `git merge release-1`
    * `git push origin dev`
15. Tagging the release
    * `git checkout master`
    * `git tag 1.0`
16. Managing hotfixes
    * the same as a release branch, but it is branched from master and merged back to dev and master
17. Merge conflict resolution
    * Git will create a new commit when merge conflicts occur
    * Any files that now have merge conflicts will have resolution markers in them
    * Git will also add local, remote, and base versions of the file for you to diff against
    * When you are satisfied with the merge run
      - `$ git add <filename>`
      - `$ git commit`
    * The mergetool may come in handy
      - `$ git config --global merge.tool vimdiff`
      - `$ git mergetool`
18. Other concepts
    * `git help`
    * Creating new repositories with `git init`
    * Ignoring files with `.gitignore`
    * `git stash` and `git stash pop`
    * Adding/removing remote repositories
19. Resources
    * Pro Git (Book)
      - Free online [`http://git-scm.com/book`](http://git-scm.com/book)
    * Try git online
      - [`http://try.github.io/levels/1/challenges/1`](http://try.github.io/levels/1/challenges/1)
    * Git Immersion
      - [`http://gitimmersion.com/lab_01.html`](http://gitimmersion.com/lab_01.html)
    * Check out the presentation
      - [`http://brian-jesse.com/gittalk`](http://brian-jesse.com/gittalk)


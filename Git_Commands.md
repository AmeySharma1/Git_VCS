/* 
 * Topic: Common Git Commands (Core Commands + Internal Working)
 *
 * Explanation:
 * - Git commands help us interact with the Git system to track changes, manage versions, and collaborate.
 * - Instead of mugging commands, understand WHAT happens internally.
 *
 * ------------------------------------------------------------
 * 🔹 1) git init
 * ------------------------------------------------------------
 * - Initializes a new Git repository in your project
 * - Creates a hidden .git folder
 *
 * Internally:
 * - Git creates internal structure to store commits, objects, branches
 *
 * Command:
 */

git init

/*
 * ------------------------------------------------------------
 * 🔹 2) git clone
 * ------------------------------------------------------------
 * - Copies an existing remote repository to your local system
 *
 * Internally:
 * - Downloads complete project + full history
 *
 * Command:
 */

git clone https://github.com/user/repo.git

/*
 * ------------------------------------------------------------
 * 🔹 3) git status
 * ------------------------------------------------------------
 * - Shows current state of working directory and staging area
 *
 * Shows:
 * - Untracked files
 * - Modified files
 * - Staged files
 *
 * Command:
 */

git status

/*
 * ------------------------------------------------------------
 * 🔹 4) git add
 * ------------------------------------------------------------
 * - Moves changes from Working Directory → Staging Area
 *
 * Internally:
 * - Git starts tracking the file
 * - Prepares snapshot for commit
 *
 * Commands:
 */

git add file.js        // add specific file
git add .              // add all files

/*
 * ------------------------------------------------------------
 * 🔹 5) git commit
 * ------------------------------------------------------------
 * - Saves staged changes into repository as a snapshot
 *
 * Internally:
 * - Git creates a commit object
 * - Generates unique SHA-1 hash
 * - Stores metadata (author, time, message)
 *
 * Command:
 */

git commit -m "Initial commit"

/*
 * ------------------------------------------------------------
 * 🔹 6) git log
 * ------------------------------------------------------------
 * - Shows commit history
 *
 * Displays:
 * - Commit hash
 * - Author
 * - Date
 * - Message
 *
 * Command:
 */

git log

/*
 * ------------------------------------------------------------
 * 🔹 7) git diff
 * ------------------------------------------------------------
 * - Shows differences between changes
 *
 * Use cases:
 * - See what changed before committing
 *
 * Command:
 */

git diff

/*
 * ------------------------------------------------------------
 * 🔹 8) git branch
 * ------------------------------------------------------------
 * - Shows or creates branches
 *
 * Commands:
 */

git branch            // list branches
git branch feature    // create new branch

/*
 * ------------------------------------------------------------
 * 🔹 9) git checkout
 * ------------------------------------------------------------
 * - Switch between branches
 *
 * Command:
 */

git checkout feature

/*
 * (Modern alternative)
 */

git switch feature

/*
 * ------------------------------------------------------------
 * 🔹 10) git merge
 * ------------------------------------------------------------
 * - Combines changes from one branch into another
 *
 * Command:
 */

git merge feature

/*
 * ------------------------------------------------------------
 * 🔹 11) git pull
 * ------------------------------------------------------------
 * - Fetch + merge changes from remote repository
 *
 * Internally:
 * - git fetch + git merge
 *
 * Command:
 */

git pull origin main

/*
 * ------------------------------------------------------------
 * 🔹 12) git push
 * ------------------------------------------------------------
 * - Uploads local commits to remote repository (GitHub)
 *
 * Command:
 */

git push origin main

/*
 * ------------------------------------------------------------
 * 🔹 13) git fetch
 * ------------------------------------------------------------
 * - Downloads changes from remote but DOES NOT merge
 *
 * Use case:
 * - Safe way to check updates before merging
 *
 * Command:
 */

git fetch

/*
 * ------------------------------------------------------------
 * 🔹 14) git remote
 * ------------------------------------------------------------
 * - Manages remote repositories
 *
 * Commands:
 */

git remote -v
git remote add origin https://github.com/user/repo.git

/*
 * ------------------------------------------------------------
 * 🔹 15) git rm
 * ------------------------------------------------------------
 * - Removes file from working directory + Git
 *
 * Command:
 */

git rm file.js

/*
 * ------------------------------------------------------------
 * 🔹 16) git mv
 * ------------------------------------------------------------
 * - Renames or moves a file
 *
 * Command:
 */

git mv old.js new.js

/*
 * ------------------------------------------------------------
 * 🔥 MINI FLOW (IMPORTANT)
 *
 * git init
 * → git add
 * → git commit
 * → git push
 *
 * ------------------------------------------------------------
 * Interview Answer:
 * - Git commands are used to manage version control operations such as tracking changes, committing code, branching, and collaboration.
 * - Common commands include git init, git add, git commit, git push, and git pull.
 * - Each command interacts with different parts of Git architecture like working directory, staging area, and repository.
 *
 * ------------------------------------------------------------
 * Common Interview Questions:
 *
 * 1) Difference between git add and git commit?
 * Answer:
 * - git add moves changes to staging area
 * - git commit saves them permanently in repository
 *
 * 2) Difference between git fetch and git pull?
 * Answer:
 * - fetch: only downloads changes
 * - pull: downloads + merges changes
 *
 * 3) What does git clone do?
 * Answer:
 * - Copies a remote repository along with its entire history
 *
 * 4) What is git log used for?
 * Answer:
 * - To view commit history
 *
 * 5) What is difference between git checkout and git switch?
 * Answer:
 * - checkout: older command (used for many purposes)
 * - switch: newer, only for switching branches
 *
 * 6) What happens internally when you commit?
 * Answer:
 * - Git creates a snapshot, assigns a unique hash, and stores metadata in repository
 *
 * 7) What is origin in git push origin main?
 * Answer:
 * - "origin" is the default name of the remote repository
 *
 */

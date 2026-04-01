/* 
 * Topic: Git Architecture (Working Directory, Staging Area, Repository)
 *
 * Explanation:
 * - Git works in three main layers. Understanding this flow is crucial for interviews.
 *
 * 1) Working Directory:
 * - This is your actual project folder where you create/edit files.
 * - Example: You write code in index.js → this is in Working Directory.
 *
 * 2) Staging Area (Index):
 * - This is an intermediate area where you prepare changes before committing.
 * - You decide what changes should go into the next commit.
 * - Think of it as a "selection box" before final save.
 *
 * 3) Repository (.git folder):
 * - This is where Git permanently stores your commits and history.
 * - Located inside hidden ".git" folder in your project.
 *
 * 🔥 FLOW (VERY IMPORTANT):
 *
 * Working Directory  →  Staging Area  →  Repository
 *        (edit)            (add)            (commit)
 *
 * Commands Mapping:
 *
 * - git add      → Moves changes from Working Directory → Staging Area
 * - git commit   → Moves changes from Staging Area → Repository
 *
 * Visual Understanding:
 *
 * Step 1: Create/Edit File
 *   → File is in Working Directory (UNTRACKED / MODIFIED)
 *
 * Step 2: git add file.js
 *   → File moves to Staging Area (READY TO COMMIT)
 *
 * Step 3: git commit -m "message"
 *   → File saved permanently in Repository (VERSION CREATED)
 *
 * File States in Git:
 *
 * - Untracked:
 *   File is new, Git is not tracking it
 *
 * - Modified:
 *   File is changed but not staged
 *
 * - Staged:
 *   File is ready to be committed
 *
 * - Committed:
 *   File is saved in Git history
 *
 * Real-Life Analogy:
 *
 * - Working Directory → Writing answers in exam rough sheet
 * - Staging Area → Selecting final answers
 * - Repository → Submitting answer sheet
 *
 * Key Insight (Interview Gold ⭐):
 * - Git does NOT directly commit from Working Directory
 * - It always goes through the Staging Area
 *
 * Interview Answer:
 * - Git architecture consists of three main areas: Working Directory, Staging Area, and Repository.
 * - The Working Directory is where files are modified, the Staging Area is where changes are prepared, and the Repository stores committed changes permanently.
 * - The git add command moves changes to the staging area, and git commit saves them to the repository.
 *
 * Common Interview Questions:
 *
 * 1) Explain Git workflow.
 * Answer:
 * - Changes are made in Working Directory → staged using git add → committed using git commit to repository.
 *
 * 2) What is Staging Area?
 * Answer:
 * - It is an intermediate area where changes are prepared before committing to the repository.
 *
 * 3) Why do we need Staging Area?
 * Answer:
 * - It allows selective commits (choose specific changes instead of committing everything).
 *
 * 4) Can we commit directly from Working Directory?
 * Answer:
 * - No, changes must first be added to the staging area.
 *
 * 5) What is .git folder?
 * Answer:
 * - It is a hidden folder that stores all Git data including commits, branches, and history.
 *
 * Code:
 *
 * 1) Initialize Repository
 */

git init

/*
 * Explanation:
 * - Creates a new Git repository (.git folder)
 *
 * 2) Create a file (example: index.js)
 */

console.log("Hello Git");

/*
 * 3) Check status
 */

git status

/*
 * Explanation:
 * - Shows file is UNTRACKED
 *
 * 4) Add file to staging
 */

git add index.js

/*
 * Explanation:
 * - Moves file to staging area
 *
 * 5) Commit file
 */

git commit -m "Initial commit"

/*
 * Explanation:
 * - Saves file permanently in repository
 *
 * 6) Modify file again
 */

console.log("Updated code");

/*
 * 7) Check status again
 */

git status

/*
 * Explanation:
 * - File is now MODIFIED (not staged yet)
 */

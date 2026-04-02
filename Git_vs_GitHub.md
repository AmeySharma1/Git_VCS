/* 
 * Topic: Difference Between Git and GitHub
 *
 * Explanation:
 * - Git and GitHub are related but NOT the same thing.
 *
 * - Git:
 *   - Git is a Distributed Version Control System (DVCS).
 *   - It is a tool/software installed locally on your system.
 *   - It helps track changes in code and manage version history.
 *
 * - GitHub:
 *   - GitHub is a cloud-based platform that hosts Git repositories.
 *   - It allows developers to store code online and collaborate with others.
 *
 * 🔥 Core Difference:
 * - Git = Tool (Version Control System)
 * - GitHub = Platform (Hosting + Collaboration)
 *
 * ------------------------------------------------------------
 * 🔹 Deep Understanding (VERY IMPORTANT)
 * ------------------------------------------------------------
 *
 * Git works locally:
 * - You can use Git WITHOUT internet
 * - You can create commits, branches, logs locally
 *
 * GitHub works remotely:
 * - Used to store code on cloud
 * - Requires internet
 * - Enables sharing and collaboration
 *
 * ------------------------------------------------------------
 * 🔹 Responsibilities
 * ------------------------------------------------------------
 *
 * Git handles:
 * - Tracking file changes
 * - Managing commits
 * - Branching and merging
 * - Maintaining history
 *
 * GitHub handles:
 * - Remote storage (backup)
 * - Collaboration between developers
 * - Pull Requests (PR)
 * - Code reviews
 * - Issues and project management
 *
 * ------------------------------------------------------------
 * 🔹 Real-World Analogy
 * ------------------------------------------------------------
 *
 * - Git:
 *   Like MS Word on your laptop → you write and save files locally
 *
 * - GitHub:
 *   Like Google Drive → you upload files to share with others
 *
 * ------------------------------------------------------------
 * 🔹 Workflow Together
 * ------------------------------------------------------------
 *
 * Step 1: Write code locally
 * Step 2: Use Git to track changes (add, commit)
 * Step 3: Push code to GitHub
 * Step 4: Team members pull code from GitHub
 *
 * Commands Flow:
 *
 * git add → git commit → git push (to GitHub)
 * git pull ← (from GitHub)
 *
 * ------------------------------------------------------------
 * 🔹 Key Differences Table
 * ------------------------------------------------------------
 *
 * Feature         | Git                          | GitHub
 * ------------------------------------------------------------
 * Type            | Tool (Software)              | Platform (Service)
 * Location        | Local system                 | Cloud (Remote server)
 * Internet        | Not required                 | Required
 * Purpose         | Version control              | Hosting + collaboration
 * Installation    | Installed locally            | Used via web/app
 *
 * ------------------------------------------------------------
 * 🔹 Important Note (Interview Trap 🚨)
 *
 * - GitHub is NOT the only platform for Git
 * - Other platforms exist:
 *   - GitLab
 *   - Bitbucket
 *
 * So:
 * - Git works independently
 * - GitHub is just one service built on Git
 *
 * ------------------------------------------------------------
 * Interview Answer:
 * - Git is a distributed version control system used to track changes in source code locally.
 * - GitHub is a cloud-based platform that hosts Git repositories and provides collaboration features like pull requests and code reviews.
 * - In short, Git manages code history, while GitHub helps teams collaborate and store code remotely.
 *
 * ------------------------------------------------------------
 * Common Interview Questions:
 *
 * 1) Difference between Git and GitHub?
 * Answer:
 * - Git is a version control system, while GitHub is a platform for hosting Git repositories and collaboration.
 *
 * 2) Can we use Git without GitHub?
 * Answer:
 * - Yes, Git works completely locally without any remote platform.
 *
 * 3) Can we use GitHub without Git?
 * Answer:
 * - No, GitHub is built on Git, so Git knowledge is required.
 *
 * 4) Is GitHub a VCS?
 * Answer:
 * - No, GitHub is not a VCS. Git is the actual VCS.
 *
 * 5) Name alternatives to GitHub.
 * Answer:
 * - GitLab, Bitbucket
 *
 * 6) What is the role of GitHub in a team?
 * Answer:
 * - It enables collaboration, code sharing, version control backup, and code review through pull requests.
 *
 * ------------------------------------------------------------
 * Code:
 *
 * 1) Local Git Workflow
 */

git init
git add .
git commit -m "Initial commit"

/*
 * Explanation:
 * - All above steps happen locally using Git
 *
 * 2) Connect to GitHub and push
 */

git remote add origin https://github.com/user/repo.git
git push origin main

/*
 * Explanation:
 * - Code is now uploaded to GitHub (remote server)
 *
 * 3) Another developer pulls code
 */

git pull origin main

/*
 * Explanation:
 * - Code is downloaded from GitHub to local system
 */

/* 
 * Topic: Version Control System (VCS)
 *
 * Explanation:
 * - A Version Control System (VCS) is a tool that helps developers track and manage changes in code over time.
 * - It allows multiple developers to work on the same project without overwriting each other's work.
 * - Every change made to the code is stored as a "version", so you can go back to any previous state if needed.
 *
 * - Think of it like:
 *   Google Docs history OR game save checkpoints 🎮
 *   → You can go back to previous versions anytime
 *
 * Why VCS is Important:
 * - Tracks history of changes (who changed what and when)
 * - Enables collaboration among multiple developers
 * - Helps in reverting back to stable versions if bugs occur
 * - Prevents data loss
 * - Maintains different versions of the same project
 *
 * Types of Version Control Systems:
 *
 * 1) Centralized VCS (CVCS):
 * - Example: SVN (Subversion)
 * - Has a central server where all code is stored
 * - Developers pull code from server and push changes back
 *
 * Disadvantages:
 * - If server goes down → no work possible
 * - Requires internet connection
 * - Single point of failure
 *
 * 2) Distributed VCS (DVCS):
 * - Example: Git
 * - Every developer has a complete copy of the repository (including history)
 *
 * Advantages:
 * - Works offline
 * - No single point of failure
 * - Faster operations (local commits)
 * - Better branching and merging support
 *
 * Key Concepts:
 *
 * - Repository (Repo):
 *   A folder that contains project files + version history
 *
 * - Commit:
 *   A snapshot of changes saved in the repository
 *
 * - Version:
 *   A specific state of the project at a given time
 *
 * - Branch:
 *   A separate line of development
 *
 * - Merge:
 *   Combining changes from different branches
 *
 * Real-World Example:
 * - Imagine 3 developers working on a website:
 *   Dev A → working on login feature
 *   Dev B → working on UI
 *   Dev C → fixing bugs
 *
 * Without VCS:
 * ❌ Code overwrite issues
 * ❌ No history
 *
 * With VCS:
 * ✅ Everyone works safely
 * ✅ Changes tracked
 * ✅ Easy merging
 *
 * Interview Answer:
 * - A Version Control System is a tool that helps track and manage changes in source code over time.
 * - It allows multiple developers to collaborate efficiently by maintaining a history of changes and enabling version management.
 * - There are two types: Centralized (like SVN) and Distributed (like Git), where Git is more efficient due to local repositories and better branching support.
 *
 * Common Interview Questions:
 *
 * 1) What is Version Control System?
 * Answer:
 * - A system that tracks changes in files over time and allows reverting to previous versions.
 *
 * 2) Why do we need VCS?
 * Answer:
 * - To manage code changes, enable collaboration, maintain history, and avoid conflicts.
 *
 * 3) Difference between Centralized and Distributed VCS?
 * Answer:
 * - Centralized: Single central server (risk of failure)
 * - Distributed: Each developer has full copy (more reliable)
 *
 * 4) What problems does VCS solve?
 * Answer:
 * - Code conflicts
 * - Data loss
 * - Lack of history tracking
 * - Collaboration issues
 *
 * 5) What is a repository?
 * Answer:
 * - A storage location containing project files and their version history.
 *
 * Code:
 *
 * (No actual code here since VCS is a conceptual topic,
 * but we will use Git commands in upcoming topics)
 */

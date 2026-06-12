## What is version control?

Version Control is a program or set of programs that trcks changes to a collection of files.
Similar in games there's a version of a game.

With a VCS, you can:

- See all the changes made to your project, when the changes were made, and who made them.
- Include a message with each change to explain the reasoning behind it.
- Retrieve past versions of the entire project or of individual files.
- Create branches, where changes can be made experimentally. This feature allows several different sets of changes (for example, features or bug fixes) to be worked on at the same time, possibly by different people, without affecting the main branch. Later, you can merge the changes you want to keep back into the main branch.
- Attach a tag to a version—for example, to mark a new release.

## Git Terminology



    Working tree: The set of nested directories and files that contain the project that's being worked on.

    Repository (repo): The data store, contained in a hidden directory named .git at the top level of a working tree, where Git keeps all the history and metadata for a project. Repositories are almost always referred to as repos. A bare repository is one that isn't part of a working tree; it's used for sharing or backup. A bare repo is usually a directory with a name that ends in .git—for example, project.git.

    Hash: A number produced by a hash function that represents the contents of a file or another object as a fixed number of digits. Git traditionally uses SHA-1 hashes that are 160 bits long, though modern versions of Git also support SHA-256 (256 bits). One advantage to using hashes is that Git can tell whether a file has changed by hashing its contents and comparing the result to the previous hash. If the file time-and-date stamp is changed, but the file hash isn’t changed, Git knows the file contents aren’t changed.

    Object: A Git repo contains four types of objects, each uniquely identified by a hash. A blob object contains an ordinary file. A tree object represents a directory; it contains names, hashes, and permissions. A commit object represents a specific version of the working tree. An annotated tag object stores metadata, such as a name, message, and optional signature, and usually points to a commit, though it can point to other Git objects as well. Git also supports lightweight tags, which are references rather than objects.

    Commit: When used as a verb, commit means to make a commit object. This action takes its name from commits to a database. It means you are committing the changes you have made so that others can eventually see them, too.

    Branch: A branch is a named series of linked commits. The most recent commit on a branch is called the head. The default branch, which is created when you initialize a repository, is called main on GitHub and many other platforms. The head of the current branch is named HEAD. Branches are an incredibly useful feature of Git because they allow developers to work independently (or together) in branches and later merge their changes into the default branch.

    Remote: A remote is a named reference to another Git repository. When you clone a repo, Git creates a remote named origin that points to the repository you cloned from. origin is the default remote for push and pull operations.

    Commands, subcommands, and options: Git operations are performed by using commands like git push and git pull. git is the command, and push or pull is the subcommand. The subcommand specifies the operation you want Git to perform. Commands frequently are accompanied by options, which use hyphens (-) or double hyphens (--). For example, git reset --hard.

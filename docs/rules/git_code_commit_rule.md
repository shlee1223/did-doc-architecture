# Commit Message Guidelines

## 1. Commit Message Structure

Commit messages are generally composed of a title / body / footer, with a single line of space separating each section.

- **type**: Indicates what the commit pertains to, represented by a keyword
- **subject**: The title of the commit message
- **body**: The body of the commit message (optional)
- **footer**: The footer of the commit message (optional)

```c#
Type: Subject

Body

Footer
```

### 1.1. type

- **feat**: Add new feature
- **fix**: Bug fix
- **build**: Modify build-related files
- **ci**: Modify CI-related settings
- **docs**: Documentation (adding, modifying, or deleting documents)
- **style**: Style (code formatting, adding semicolons: no change to business logic)
- **refactor**: Code refactoring
- **test**: Tests (adding, modifying, or deleting test code: no change to business logic)
- **chore**: Miscellaneous changes (e.g., modifying build scripts)

### 1.2. subject

- Titles written in English should not exceed 50 characters and should not use periods.
- Titles include the commit type.
- Use the imperative mood for titles, avoiding past tense.
- Separate title and body with a blank line.
- The first letter of the title should be capitalized.
- Include issue numbers in the title if related to an issue.

Examples: English title cases
```c#
# Add : Add
# Remove : Remove
# Simplify : Simplify
# Update : Update
# Implement : Implement
# Prevent : Prevent
# Move : Move
# Rename : Rename
```

### 1.3. body

- Do not exceed 72 characters per line
- Write according to what and why, rather than how
- Necessary when describing explanations or reasons for commits

### 1.4. footer

- Used for adding **reference information** such as the issue it came from

### 1.5. Example

```c#
feat: Summarize changes in around 50 characters or less
More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789

```

### 1.6. Summary

| Type | Subject | Body (Optional) | Footer (Optional) |
|------|---------|------------------|---------------------|
| feat: Add new feature | Title should not exceed 50 characters. | Body should not exceed 72 characters per line. | Write the issue tracker ID. |
| fix: Bug fix | Do not use periods or special characters. | Provide as much detail as possible regardless of length. | Write in the format "Type: #IssueNumber". |
| docs: Documentation update | When writing in English, place the base form of the verb at the beginning and capitalize the first letter (avoid using past tense). | Explain what was changed or why it was changed rather than how it was changed. | Separate multiple issue numbers with commas (,). |
| style: Code formatting, missing semicolons, changes without code modifications | | | Fixes: If the issue is still unresolved |
| refactor: Code refactoring | | | Resolves: If the issue is resolved |
| test: Add or update test code, refactor test code | | | Ref: If there are related issues |
| chore: Build task updates, package manager updates, parts unrelated to production code (.gitignore, build.gradle, etc.) | | | Related to: Issue number related to the commit (if still unresolved) |
| comment: Add or change comments | | | ex) Fixes: #45 Related to: #34, #23 |
| remove: Delete files or folders | | | |
| rename: Rename files or folders | | | |

## 2. Reserved Keywords Usage

### 2.1. Reserved Keywords

When writing commit messages in English, reserved keywords can be used to automatically close issues by making certain features work. Reserved keywords can function regardless of their position in the commit message:

- **fix / fixes / fixed**
  - Used for issues related to code changes
  - Generally used for fixing bugs or issues related to feature changes
- **resolve / resolves / resolved**
  - Used for issues not directly related to code changes
  - Generally used for resolving technical problems or meeting requirements
- **close / closes / closed**
  - Used to close issues
  - More general than the above keywords and used to complete or resolve issues regardless of code changes

### 2.2. Examples

- When you push the branch after a commit, the issue will be automatically closed with the message below.
- Issue closing depends on the branch to which the commit belongs.
- If the default branch is **master**:
  - Committing and pushing to the master branch will close the issue.
  - Committing to other branches will close the issue when the branch is merged into the remote master branch.

```c#
# Example of closing a single issue in the title
Close #31 - refactoring wrap-up

* This is the wrap-up of refactoring main code.
* main.c
  * removed old comments
  * fixed rest indentations
  * method extraction at line no. 35

# Example of closing multiple issues in the body
Update policy 16/04/02

* This closes #128 - cab policy, closes #129 - new hostname, and fixes #78 - bug on logging.
* cablist.txt: changed ACL due to policy update delivered via email on 16/04/02, @mr.parkyou
* hostname.properties: cab hostname is updated
* BeautifulDeveloper.java: logging problem on line no. 78 is fixed. The `if` statement is never happening. This deletes the `if` block.
```
# Writing Good Git Commit Messages

Good commit messages matter.
They make it easier to understand **why** changes were made, simplify debugging, and help future maintainers (including you). A `git diff` shows *what* changed, but the commit message explains *why*.

Bad logs are confusing. Good logs save time and improve collaboration.

---

## The 7 Rules of a Great Commit Message

1. **Separate subject from body with a blank line**

   * Subject: short summary.
   * Body: optional, for context.
   * Example:

     ```
     Fix typo in user guide

     Corrected spelling of "configuration" in introduction.
     ```

2. **Limit subject line to \~50 characters**

   * Keeps it readable and consistent.
   * If it’s too long, you might be committing too much at once.

3. **Capitalize the subject line**

   * ✅ `Add login validation`
   * ❌ `add login validation`

4. **Do not end subject with a period**

   * ✅ `Fix broken test case`
   * ❌ `Fix broken test case.`

5. **Use imperative mood** (like giving a command)

   * ✅ `Add error handling for null values`
   * ❌ `Added error handling for null values`
   * Think: *“If applied, this commit will…”*

6. **Wrap the body at 72 characters**

   * Makes it easy to read in terminals and tools.

7. **Use the body to explain *what* and *why*, not *how***

   * Code shows *how*. Message explains the reason.
   * Example:

     ```
     Simplify user session handling

     Replaced manual token cleanup with a scheduled task. 
     This prevents memory leaks and makes sessions easier to manage.
     ```

---

## Example of a Proper Commit

```
Add validation to signup form

Ensure that emails follow the correct format and passwords 
are at least 8 characters long. This prevents invalid data 
from being stored and improves user experience.

Resolves: #42
```

---

## Practical Tips

* **Atomic commits**: Commit one logical change at a time.
* **Small, frequent commits**: Easier to review and rollback.
* **Use the command line**: More control, less clutter.
* **Reference issues/PRs**: Helps track changes.

---

👉 **Bottom line:** Good commit messages = better collaboration, faster debugging, and cleaner history.



# Git & GitHub Basics

## What is source code management?
A way to track, organize, and manage changes to code over time.

## What is Git?
A version control system that helps you track changes and manage code history locally.

## What is GitHub?
A cloud platform that hosts Git repositories and makes collaboration easier.

## What is the difference between Git and GitHub?
- **Git** = the tool for version control (runs on your computer).  
- **GitHub** = an online service to store and share Git repositories.  

---

## How to create a repository
1. On GitHub, click **New Repository**.  
2. Name it, choose visibility (public/private), and create.  
3. Clone it to your computer with:  
   ```bash
   git clone <repo-url>
```

---

## What is a README?

A file (`README.md`) that explains what the project is about, how to set it up, and how to use it.

## How to write good READMEs

* Project title and description
* Installation/setup instructions
* Usage examples
* Contribution guide
* License information

---

## How to commit

```bash
git add <file>
git commit -m "Your message here"
```

## How to write helpful commit messages

* Be clear and concise.
* Use the present tense (e.g., "Add search function").
* Explain why the change was made if needed.

---

## How to push code

```bash
git push origin main
```

## How to pull updates

```bash
git pull origin main
```

---

## How to create a branch

```bash
git checkout -b new-feature
```

## How to merge branches

1. Switch to main:

   ```bash
   git checkout main
   ```
2. Merge your branch:

   ```bash
   git merge new-feature
   ```

---

## How to work as collaborators on a project

* Add collaborators in GitHub repo settings.
* Each person clones the repo.
* Use branches and pull requests to manage changes.

---

## Which files should and should not appear in your repo

**Should appear**: source code, README, configuration files, docs.
**Should not appear**: passwords, API keys, build artifacts, OS/system files (use `.gitignore` to exclude them).


---

# Basic Formatting of Markdown

## Headings

# A first-level heading
## A second-level heading
### A third-level heading


## Styling text


| Style                  | Syntax                 | Keyboard shortcut                            | Example                                      | Output                          |
|-------------------------|------------------------|----------------------------------------------|----------------------------------------------|---------------------------------|
| **Bold**               | `** **` or `__ __`    | Command+B (Mac) or Ctrl+B (Windows/Linux)    | `**This is bold text**`                      | **This is bold text**           |
| *Italic*               | `* *` or `_ _`        | Command+I (Mac) or Ctrl+I (Windows/Linux)    | `_This text is italicized_`                  | _This text is italicized_       |
| ~~Strikethrough~~      | `~~ ~~` or `~ ~`      | None                                         | `~~This was mistaken text~~`                 | ~~This was mistaken text~~      |
| Bold + Nested Italic   | `** **` and `_ _`     | None                                         | `**This text is _extremely_ important**`     | **This text is _extremely_ important** |
| All Bold + Italic      | `*** ***`             | None                                         | `***All this text is important***`           | ***All this text is important*** |
| Subscript              | `<sub> </sub>`        | None                                         | `This is a <sub>subscript</sub> text`        | This is a <sub>subscript</sub> text |
| Superscript            | `<sup> </sup>`        | None                                         | `This is a <sup>superscript</sup> text`      | This is a <sup>superscript</sup> text |
| Underline              | `<ins> </ins>`        | None                                         | `This is an <ins>underlined</ins> text`      | This is an <ins>underlined</ins> text |

## Quoting text

Text that is not a quote

`> Text that is a quote`

**Result**:
> text that is a quote

## Quoting code

Use `git status` to list all new or modified files that haven't yet been committed.

To format code or text into its own distinct block, use triple backticks.

Some basic Git commands are:
```
git status
git add
git commit
```

## Supported code colors

| Color | Syntax        | Example              | Output |
|-------|---------------|----------------------|--------|
| HEX   | `#RRGGBB`     | `#0969DA`            | <span style="color:#0969DA;">●</span> |
| RGB   | `rgb(R,G,B)`  | `rgb(9, 105, 218)`   | <span style="color:rgb(9,105,218);">●</span> |
| HSL   | `hsl(H,S,L)`  | `hsl(212, 92%, 45%)` | <span style="color:hsl(212,92%,45%);">●</span> |


## Links

This site was built using [GitHub Pages](https://pages.github.com/).

## Section Links

```
# Example headings

## Sample Section

## This'll be a _Helpful_ Section About the Greek Letter Θ!
A heading containing characters not allowed in fragments, UTF-8 characters, two consecutive spaces between the first and second words, and formatting.

## This heading is not unique in the file

TEXT 1

## This heading is not unique in the file

TEXT 2

# Links to the example headings above

Link to the sample section: [Link Text](#sample-section).

Link to the helpful section: [Link Text](#thisll-be-a-helpful-section-about-the-greek-letter-Θ).

Link to the first non-unique section: [Link Text](#this-heading-is-not-unique-in-the-file).

Link to the second non-unique section: [Link Text](#this-heading-is-not-unique-in-the-file-1).
```

## Images

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://myoctocat.com/assets/images/base-octocat.svg)

## Lists

```
- George Washington
* John Adams
+ Thomas Jefferson
```

- George Washington
* John Adams
+ Thomas Jefferson


```
1. James Madison
2. James Monroe
3. John Quincy Adams
```

1. James Madison
2. James Monroe
3. John Quincy Adams

### Nested Lists

```
1. First list item
   - First nested list item
     - Second nested list item
```

1. First list item
   - First nested list item
     - Second nested list item

## Task Lists

```
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
```

- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:


# Right-Engineering, Right-Documenting

Finding balance is key:  
- Too much = rigid, hard to maintain.  
- Too little = chaos, confusion.  

---

## Right-Documenting

### Why it matters
- Write for **future developers** (including your future self).  
- Helps others understand decisions, structure, and code quickly.  

### What to document
- **Architecture**: high-level choices.  
- **Comments**:  
  - Functions → purpose + usage.  
  - Inside functions → short step-by-step notes.  
- **Names**: clear and unambiguous.  
- **Indentation**: keep code readable.  
- **Commits**: clear Git messages.  
- **README.md**: intro, setup, license, contribution guide.  

### Over-documenting (risks)
- Repeating info already online.  
- Docs too long to read quickly.  
- Hard to keep updated → becomes outdated or ignored.  

### Under-documenting (risks)
- Code looks like spaghetti.  
- Open-source projects stall.  
- Delays when maintainers are unavailable.  
- Teams redo work because nothing was shared.  

---

## Right-Engineering

### Key idea
Balance **simplicity** and **future-proofing**.  

### Analogy
- **Naive thrower** → fine for small tasks, fails at scale.  
- **Over-engineered catapult** → elegant but rigid, breaks with new needs.  

### Risks
- **Under-engineering** → impractical when needs grow.  
- **Over-engineering** → too rigid, costly to change.  

### Best practice
- Keep it **simple enough to stay flexible**.  
- Engineer it **enough to be maintainable**.  

---

### Example: To-Do List API Project

# Initial documentation
## **README.md**


### To-Do List API

A simple REST API to manage to-do items.

### Setup
1. Clone the repo
2. Install dependencies: `npm install`
3. Run: `npm start`

#### Endpoints
- `GET /todos` → list all to-dos
- `POST /todos` → create new to-do
- `PUT /todos/:id` → update a to-do
- `DELETE /todos/:id` → delete a to-do


## **Architecture.md**

### Architecture

- Express.js handles routing.
- MongoDB stores todos.
- `controllers/` → logic for each route.
- `models/` → database schema.
- `routes/` → API endpoints.


## **Code Example**

```js
// controllers/todoController.js

/**
 * Get all todos
 * @route GET /todos
 * @returns {Array} List of todos
 */
exports.getTodos = async (req, res) => {
  const todos = await Todo.find();
  res.json(todos);
};
```

---

### Adding a new function: Search To-Dos

When you add a new endpoint, also update the docs.

#### **New code with comment**

```js
/**
 * Search todos by keyword
 * @route GET /todos/search?q=keyword
 * @param {String} q - keyword to search
 * @returns {Array} List of matching todos
 */
exports.searchTodos = async (req, res) => {
  const { q } = req.query;
  const todos = await Todo.find({ text: { $regex: q, $options: "i" } });
  res.json(todos);
};
```

### **Update README.md**


#### Endpoints
- `GET /todos` → list all to-dos
- `POST /todos` → create new to-do
- `PUT /todos/:id` → update a to-do
- `DELETE /todos/:id` → delete a to-do
- `GET /todos/search?q=keyword` → search todos by keyword


---

✅ This way:

* High-level docs (README, architecture) guide newcomers.
* Code comments explain purpose and usage.
* New functions are documented in both code **and** README.


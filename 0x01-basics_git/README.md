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


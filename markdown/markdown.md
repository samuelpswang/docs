# Markdown Cheat Sheet

- [Markdown Cheat Sheet](#markdown-cheat-sheet)
  - [FAQs](#faqs)
  - [Basic Syntax](#basic-syntax)
    - [Block Elements](#block-elements)
    - [Inline Elements](#inline-elements)
    - [Misc](#misc)
    - [Diagrams](#diagrams)
  - [Extended Syntax](#extended-syntax)
    - [Block Elements](#block-elements-1)
    - [Inline Elements](#inline-elements-1)
    - [Misc](#misc-1)
    - [Diagrams](#diagrams-1)
  - [Github-Flavord Markdown](#github-flavord-markdown)
    - [Keywords](#keywords)
    - [Issue/Pull Request Links](#issuepull-request-links)
    - [Commit Links](#commit-links)
    - [Misc](#misc-2)
  - [References](#references)

## FAQs

| Question | Answer |
| --- | --- |
| Where is markdown used? | Since markdown is a lightweight markup language, it is widely used in software developement (particularly in writing documentation). |
| Why is markdown called markdown? | "Markdown" is a wordplay on "markup", which is basically saying it is a language that provides styling to text. |
| What about using HTML in my markdown document? | Yes, you can use HTML in your markdown and it will generally work, but pure markdown linters will throw warnings. |

## Basic Syntax

### Block Elements

| Item | Syntax | Remarks |
| --- | --- | --- |
| Heading | `# heading-1`, `## heading-2`, ...  | Number of `#` corresponds to the level of heading. Max 6 levels.|
| Paragraph | null | Just start on a new line. |
| Block Quotes | `> blockquote` | |
| Ordered List | `1. item`, `2. item`, ... | Only numbers with `.` after will work. Indent for different levels. |
| Unordered List | `- item` | Indent for different levels. |
| Horizontal Line | `---` | |

### Inline Elements

| Item | Syntax | Remarks |
| --- | --- | --- |
| Bold | `**bolded-text**` | |
| Italic | `*italicized-text*`| |
| Code | `` `code` `` | Use ` `` ` for around code to escape ` ` `. |
| Link | `[displayed-link-name](link-address)` | |
| Image | `![alt-text](image-address)`| Internet URLs and relative file paths both work. |

### Misc

- Wrap each block with blank lines.
- Indent with 2 spaces.
- Insert block under list, indent it the same level as the list item.
- Unify syntax, although multiple symbols may do the same thing, it is good practice to use only one type for one kind of feature.
- See Code Block 1 for examples.

### Diagrams

Code Block 1: Basic Syntax Example

```markdown
# Heading Level 1

I'm a paragraph. I am **bold**. I am *italicized*.

1. I am a ordered list.
  1. Sub-item-1.
  2. Sub-item-2.

- I am an unordered list.
  - Sub-item-1.
  - Sub-item-2.

> I am a block quote.

`I am a line of code`

```

## Extended Syntax

### Block Elements

| Item | Syntax | Remarks |
| --- | --- | --- |
| Task List | See Code Block 2. | |
| Table | See Code Block 3. | |
| Fenced Code Block | See Code Block 4. | |
| Definition List | See Code Block 5. | Don't work in VSCode render. |
| Footnote | See Code Block 6. | |

### Inline Elements

| Item | Syntax | Remarks |
| --- | --- | --- |
| Strikethrough | `~~text~~` |  |
| Highlight | `==text==` | Don't work in VSCode render. |
| Subscript | `text^superscript^` | Don't work in VSCode render. |
| Superscript | `text~subscript~` | Don't work in VSCode render. |
| Emoji | `:emoji-code:` | Don't work in VSCode render. |

### Misc

- If you want to escape ` ``` ` in your code block, use ` ```` ` on the outer block.

Code Block 2: Task List

```markdown
- [ ] tasklist-item
  - [x] sub-tasklist-item-1
  - [ ] sub-tasklist-item-2
```

### Diagrams

Code Block 3: Table Syntax

```markdown
| Header 1  | Header 2  | ... |
| --------- | --------- | --- |
| Row1 Col1 | Row1 Col2 | ... |
| Row2 Col1 | Row2 Col2 | ... |
| ...       | ...       | ... |
```

Code Block 4: Fenced Code Block Syntax

````markdown
```language
This is my first line of code.
This is my second line of code.
```
````

Code Block 5: Definition List Syntax

```markdown
Term
: Definition-1.
: definition-2.
```

Code Block 6: Footnote Syntax

```markdown
This is a line of text[^1].

[^1]: This is a footnote.
```

## Github-Flavord Markdown

### Keywords

| Item | Syntax | Remarks |
| --- | --- | --- |
| Duplicate | `duplicate of` | Automatically closes issue or pull request, only use on duplicates. |
| Close | `close`, `closes`, `closed` | Automatically closes issue or pull request. |
| Fix | `fix`, `fixes`, `fixed` | Automatically closes issue or pull request, used usually on issues. |
| Resolve | `resolve`, `resolves`, `resolved` | Automatically closes issue or pull request, used usually on issues. |

### Issue/Pull Request Links

| Item | Syntax | Remarks |
| --- | --- | --- |
| Issue / Pull Request (URL) | `issue-url` | Rendered as `#issue-number`. |
| Issue / Pull Request (Number) | `#issue-number` | Rendered as `#issue-number`. |
| Organization Repo Issue / Pull Request (Number) | `username/repo-name#issue-number` | |
| User Repo Issue / Pull Request (Number) | `organization/repo-name#issue-number` | |

### Commit Links

| Item | Syntax | Remarks |
| --- | --- | --- |
| Commit (URL) | `commit-url` | Rendered as `first-seven-digits-of-sha`. |
| Commit (SHA Value) | `full-sha-value` | Rendered as `first-seven-digits-of-sha`. |
| Commit (User & SHA Value) | `username@full-sha-value` | Rendered as `username@first-seven-digits-of-sha`. |
| Commit (User, Repo & Sha Value) | `username/repo@full-sha-value` | Rendered as `username/repo@first-seven-digits-of-sha`.|

### Misc

- To diplay diagrams on Github markdown, use the mermaid libray. See [https://mermaid-js.github.io/mermaid/#/](https://mermaid-js.github.io/mermaid/#/).
- To insert specific lines of code from a Github repository, navigate to file and copy its permanant file code. See [https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-a-permanent-link-to-a-code-snippet).

## References

[1]: Docs.github.com. 2022. [online] Available at: <https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting> [Accessed 4 May 2022].

[2]: Markdownmonster.west-wind.com. 2022. Escape Markdown Fenced Code Blocks - Markdown Monster Documentation. [online] Available at: <https://markdownmonster.west-wind.com/docs/_5eg1brc0z.htm> [Accessed 4 May 2022].

[3]: Github.github.com. 2022. GitHub Flavored Markdown Spec. [online] Available at: <https://github.github.com/gfm/> [Accessed 4 May 2022].

[4]: Markdownguide.org. 2022. Markdown Cheat Sheet | Markdown Guide. [online] Available at: <https://www.markdownguide.org/cheat-sheet/> [Accessed 4 May 2022].

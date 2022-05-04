# Markdown Cheat Sheet

- [Markdown Cheat Sheet](#markdown-cheat-sheet)
  - [FAQs](#faqs)
  - [Basic Syntax](#basic-syntax)
  - [Extended Syntax](#extended-syntax)
  - [Github-Flavord Markdown](#github-flavord-markdown)
  - [References](#references)

## FAQs

| Question | Answer |
| --- | --- |
| Where is markdown used? | Since markdown is a lightweight markup language, it is widely used in software developement (particularly in writing documentation). |
| Why is markdown called markdown? | "Markdown" is a wordplay on "markup", which is basically saying it is a language that provides styling to text. |
| What about using HTML in my markdown document? |  |

## Basic Syntax

**Block Elements**

| Item | Syntax | Remarks |
| --- | --- | --- |
| Heading | `# heading-1`, `## heading-2`, ...  | Number of `#` corresponds to the level of heading. Max 6 levels.|
| Paragraph | null | Just start on a new line. |
| Block Quotes | `> blockquote` | |
| Ordered List | `1. item`, `2. item`, ... | Only numbers with `.` after will work. Indent for different levels. |
| Unordered List | `- item` | Indent for different levels. |
| Horizontal Line | `---` | |

**Inline Elements**

| Item | Syntax | Remarks |
| --- | --- | --- |
| Bold | `**bolded-text**` | |
| Italic | `*italicized-text*`| |
| Code | \``code`\` | Use `\` for escape character. |
| Link | `[displayed-link-name](link-address)` | |
| Image | `![alt-text](image-address)`| Internet URLs and relative file paths both work. |

**Note**

- Wrap each block with blank lines.
- Insert block under list, indent it the same level as the list item.
- Unify syntax, although multiple symbols may do the same thing, it is good practice to use only one type for one kind of feature.
- See Code Block 1 for examples.

Code Block 1: Basic Syntax Example

```markdown
# Heading Level 1

I'm a paragraph. I am **bold**. I am *italicized*.

1. I am a ordered list.
  1. Sub-item #1.
  2. Sub-item #2.

- I am an unordered list.
  - Sub-item #1.
  - Sub-item #2.

> I am a block quote.

`I am a line of code`

```

## Extended Syntax

**Block Elements**

| Item | Syntax | Remarks |
| --- | --- | --- |
| Task List | See Code Block 2. | |
| Table | See Code Block 3. | |
| Fenced Code Block | See Code Block 4. | |
| Definition List | See Code Block 5. | Doesn't work in VSCode render. |
| Footnote | See Code Block 6. | |

**Inline Elements**

| Item | Syntax | Remarks |
| --- | --- | --- |
| Strikethrough | `~~text~~` |  |
| Highlight | `==text==` | Doesn't work in VSCode render. |
| Subscript | `text^superscript^` | Doesn't work in VSCode render. |
| Superscript | `text~subscript~` | Doesn't work in VSCode render. |
| Emoji | `:emoji-code:` | Doesn't work in VSCode render. |

**Note**

- If you want to escape ` ``` ` in your code block, use ` ```` ` on the outer block.

Code Block 2: Task List

```markdown
- [ ] tasklist-item
  - [x] sub-tasklist-item-1
  - [ ] sub-tasklist-item-2
```

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
term
: definition-1
: definition-2
```

Code Block 6: Footnote Syntax

```markdown
This is a line of text[^1].

[^1]: This is a footnote.
```

## Github-Flavord Markdown

TODO:

## References

[1]: Markdownguide.org. 2022. Markdown Cheat Sheet | Markdown Guide. [online] Available at: <https://www.markdownguide.org/cheat-sheet/> [Accessed 4 May 2022].

[2]: Markdownmonster.west-wind.com. 2022. Escape Markdown Fenced Code Blocks - Markdown Monster Documentation. [online] Available at: <https://markdownmonster.west-wind.com/docs/_5eg1brc0z.htm> [Accessed 4 May 2022].

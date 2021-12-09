# GitHub Markdown
Overview of the Markdown rendering on GitHub.


## Headings

You can use up to up to six levels by writing `#` at the start of a line. The number of hashtags defines the hierarchy of the heading. The first two headings render with a horizontal separator.

```Markdown
# First level
## Second level
### Third level
#### Fourth level
##### Fifth level
###### Sixth level
```

### Linking to Headings
In Markdown documents, each heading has its name as the identifier which you can [link to](#linking-to-headings) via a fragment.

```Markdown
[link to](#linking-to-headings)
```

## Emphasize
Emphasize text with different meanings.

### Bold
Use double astersik or double underscore before and after text to denote **bold**.

```Markdown
**bold**
__bold__
```

### Italic
Use single asterisk or underscore before and after text to denote *italic*.

```Markdown
*italic*
_italic_
```

### Strikethrough
Use double tildes before and after text to ~~strikethrough~~.

```Markdown
~~strikethrough~~
```

## Paragraphs
Use a blank line to separate one or more lines of text.

```Markdown
a paragraph

anoter paragraph
```

## Line Breaks
Use a backslash or two or more spaces at the and of a line, then type return to define a line break.

```Markdown
test line\
test line
```

## Code

### Inline Code Block
Use a backtick before and after text to denote as `inline code`.

```Markdown
`code`
```

### Fenced Code Block
Use three backticks in a separate line before and after `code` or add at least four spaces to the start of a line.

````Markdown
```
code
```
````

````Markdown
    code
````

### Syntax Highlighting
Add syntax highlighting by specifying a language next to the backticks before a fenced code block.

````Markdown
```javascript
function markdownRocks() {
  return true
}
```
````

### Escaping Backticks

Inline code blocks can be escaped using double backticks. Fenced code blocks using backticks can be escaped using three tildes `~~~` or four backticks `` ```` ``.

## Blockquotes
Add a greater-than sign in front of a paragraph.

> To create a blockquote.

```Markdown
> a quoted pragraph
> 
> another quoted paragraph
```

### Nested Blockquotes
Add two greater-than signs in front of the paragraph you want to nest.

> a quoted paragraph
>> a quoted paragraph inside a quotation

```Markdown
> a quoted paragraph
>> a quoted paragraph inside a quotation
```

## Lists

### Numbered List
Add a figure followed by period, then a space and your content for each line item. The figure of the first item defines the sequence, figures of the following lines won't be considered.

1. numbered list item
2. numbered list item
3. numbered list item

```Markdown
1. numbered list item
2. numbered list item
3. numbered list item
```

### Bulleted Lists
Add an asterisk, dash or plus sign followed by period, then a space and your content for each line item.

* bulleted list item
* bulleted list item
* bulleted list item

```Markdown
* bulleted list item
* bulleted list item
* bulleted list item
```

### Task Lists
Add a dash followed by a space, then brackets ==with a space in between==, then another space and your content for each task.

- [ ] Unfinished task list item
- [x] Finished task list item

```Markdown
- [ ] Unfinished task list item
- [x] Finished task list item
```

### Nesting Lists
Add two spaces to indent a list item and another two spaces for every next level. You can use up to ten levels. Mixing numbered and bulleted lists is possible.

* first level
  * second level

```Markdown
* first level
  * second level

1. first level
  1. second level

* first level unordered list item
  1. second level ordered list item
```

## Links
Add the text in brackets, then add the path or URL in parentheses.

```Markdown
[this is a link](http://github.com/)
```

## Images
Add an exclamation mark, followed by alt text in brackets, and the path or URL to the image asset in parentheses. GitHub automatically adds a link to image leading to the image url.

```Markdown
![alt text](http://github.com/image.jpg)
```

_For accessibility reasons, make sure the alt text describes the image content precisely!_

### Linking images
Add a link to an image by enclosing the Markdown for the image in brackets, and then add the link in parentheses.

```Markdown
[![alt text](http://github.com/image.jpg)](http://github.com/image.jpg)
```

### Specifying Theme Context
Add the dark color mode image as a fragment to the url.

```Markdown
![alt text](http://github.com/image.jpg#dark-color-mode=http://github.com/image.jpg)
```

## Footnotes

Add a footnote in square brackets preceded by a caret and an identifier[^1]. The footnote content can be added by using the before mentioned construct followed by colon and then the content.

[^1]: Identifiers can be numbers or words without spaces or tabs.

```Markdown
Text with a footnote[^1].

[^1]: The footnote can be defined anywhere in the document but will be rendered at the end.
```

## Tables
Create a table by denoting each cell with pipe characters. Use three or more hyphens in the second row to create each column, this is mandatory. 

| column 1 | column 2 |
|---|---|
| cell | cell | 
| cell | cell | 

```Markdown
| column 1 | column 2 |
|---|---|
| cell | cell | 
| cell | cell | 
```

### Alignment
Add a colon to the left, right, or on both side of the hyphens in the second row to align text of the columns accordingly.

| column 1 | column 2 | column 3 |
|:--- | :---:| ---:|
| left | center | right |
| left | center | right |

```Markdown
| column 1 | column 2 | column 3 |
|:--- | :---:| ---:|
| left | center | right |
| left | center | right |
```

### Formatting Text
You can [emphasize](#Emphasize) text, add [links](#Links), [images](#Images) and [inline code blocks](#Inline-Code-Blocks) in tables.

## Horizontal Rules
Use three or more asterisks, dashes, or underscores alone on a line.

---

```Markdown
---
***
___
```

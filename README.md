# MARKDOWN CHEAT SHEET

![GitHub Repo Stars](https://img.shields.io/github/stars/Kernix13/markdown-cheatsheet?style=for-the-badge)
![GitHub Watchers](https://img.shields.io/github/watchers/Kernix13/markdown-cheatsheet?style=for-the-badge)
![GitHub Forks](https://img.shields.io/github/forks/Kernix13/markdown-cheatsheet?style=for-the-badge)
![GitHub Commit Activity](https://img.shields.io/github/commit-activity/y/Kernix13/markdown-cheatsheet?style=for-the-badge)

<!-- ![GitHub Contributors](https://img.shields.io/github/contributors/Kernix13/markdown-cheatsheet?style=for-the-badge) -->

![GitHub Issues](https://img.shields.io/github/issues/Kernix13/markdown-cheatsheet?style=for-the-badge)

<!-- ![GitHub Search Hits](https://img.shields.io/github/search/Kernix13/markdown-cheatsheet/markdown?style=for-the-badge) -->

<!-- <span><img alt="GitHub forks" src="https://img.shields.io/github/forks/Kernix13/markdown-cheatsheet?style=for-the-badge"></span>
<span><img alt="GitHub commit activity" src="https://img.shields.io/github/commit-activity/y/Kernix13/markdown-cheatsheet?style=for-the-badge"></span>
<span><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/Kernix13/markdown-cheatsheet?style=for-the-badge"></span> -->

Use this markdown cheat sheet as a guide for writing your markdown files. If you like it then clone or fork it, or at least click the **star** button.

> FYI: if you are using the Vs Code extension `Prettier - Code formatter`, then you want to create a `.prettierignore` file and add markdown files (see my file) because it _WILL_ mess with your markdown.

I'm breaking up all the markdown syntax into 8 categories:

1. Basics
1. Styles
1. Miscellaneous
1. Links
1. Lists
1. Code
1. Hidden
1. Visual Elements

**NOTE**: To view markdown> in VS Code hit <kbd>CTRL</kbd>+<kbd>SHIFT</kbd> + <kbd>V</kbd> or click the preview button at top right in line with the file name tabs.

<div id="back-to-top"></div>

## ~~A Literal~~ <ins>Table</ins> of _Contents_

|                             Category | Element                                       | Accepts styles? |
| -----------------------------------: | :-------------------------------------------- | :-------------: |
|                   [Basics](#basics): | [Paragraphs](#paragraphs)                     |       Yes       |
|                                      | [Special characters](#special-characters)     |      `N/A`      |
|                   [Styles](#styles): | [Bold](#bold)                                 |      `N/A`      |
|                                      | [Italic](#italic)                             |      `N/A`      |
|                                      | [Strike thru](#strike-thru)                   |      `N/A`      |
|                                      | [Underline](#underline)                       |      `N/A`      |
|     [Miscellaneous](#miscellaneous): | [Headings](#headings)                         |       Yes       |
|                                      | [Blockquotes](#blockquotes)                   |       Yes       |
|                                      | [Alerts](#alerts)                             |       Yes       |
|                                      | [Tables](#tables)                             |       Yes       |
|                                      | [Horizontal rules](#horizontal-rules)         |       No        |
|                                      | [Descriptions](#descriptions)                 |      Yes\*      |
|                                      | [Frontmatter and YAML](#frontmatter-and-yaml) |       No        |
|                     [Links](#links): | [External](#external)                         |       Yes       |
|                                      | [Anchor](#anchor)                             |       Yes       |
|                                      | [Footnotes](#footnotes)                       |       Yes       |
|                                      | [At mentions](#at-mentions)                   |      `N/A`      |
|                     [Lists](#lists): | [Unordered](#unordered)                       |       Yes       |
|                                      | [Ordered](#ordered)                           |       Yes       |
|                                      | [Nested](#nested)                             |       Yes       |
|                                      | [Tasks](#tasks)                               |       No        |
|                       [Code](#code): | [Inline](#inline)                             |      Yes\*      |
|                                      | [Tab](#tab)                                   |       No        |
|                                      | [Generic](#generic)                           |       No        |
|                                      | [Language block](#language-block)             |       No        |
|                                      | [Diff](#diff)                                 |       No        |
| [Hidden Elements](#hidden-elements): | [Comments](#comments)                         |       No        |
|                                      | [Spoiler](#spoiler)                           |       Yes       |
|                                      | [Details](#details)                           |       No        |
| [Visual Elements](#visual-elements): | [Images](#images)                             |       No        |
|                                      | [Math](#math)                                 |       No        |
|                                      | [Emojis](#emojis)                             |       No        |
|                                      | [Shields](#shields)                           |       No        |
|                                      | [Devicons](#devicons)                         |       No        |
|                                      | [Mermaid Diagrams](#mermaid-diagrams)         |       No        |
|                                      | [HTML entities](#html-entities)               |      Yes\*      |
|                        [HTML](#html) | [Block elements](#block-elements)             |        -        |
|                                      | [Inline elements](#inline-elements)           |        -        |
|                                      | [HTML tag examples](#html-tag-examples)       |        -        |
|                                      | [CSS Styles](#css-styles)                     |        -        |
|                                      | [Buttons](#buttons)                           |        -        |
|              [Resources](#resources) | N/A                                           |        -        |

<!-- ~~`<cite>`~~ -->

---

## Basics

This is a short section on basic paragraphs, the symbols used in Markdown and how to escape them.

### Paragraphs

Since paragraphs are a thing of their own, let's cover that one first:

**Paragaphs**: Just use regular text but make sure to hit the <kbd>ENTER</kbd> key twice. Sometimes if you only hit <kbd>ENTER</kbd> once, the text will de displayed as the element directly above it _and_ there will not be a line break.

### Special characters

Here are the characters you will use in Markdown. They will be covered in each section after this one:

````
# Hash tags for headines and anchor links
@ at symbol for at mentions
[] for links, checked lists / tasks, and footnotes
() for links
! for images
^ for footnote links
x or X for tasks lists
` and ``` for inline code and codeblocks respectively
* and ** for italic and bold respectively
_ underscore for italics
~~ 2 tildes for strikethrough
| for setting tables cells
|| double pipes for spoiler text on Discord
: with dashes - for table cell alignments, for footnotes, and emojis
* or - and a space for unordered lists
1., 2., 3., etc. for numbered lists
* and + for diff code blocks
> for blockquotes
> > for indented / nested blockquotes
3 - or * for horizontal rules
<!-- for comments in markdown -->
\ to escape most of the characters above, as in...
\* escape asterisk,
\| escape pipe, etc...
" for titles in links and images
````

**NOTE**: Some of the symbols have different effects when used in _Math Expressions_. See that section for information on those.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Styles

This category deals with the styling of words and can be used with every category with a few exceptions. You may not have thought of it but you can apply these effects to all or some of the words in:

- Headings
- Links
- Lists (Not Tasks)
- Blockquotes
- Table cell values
- HTML entities (except strikethrough)
- Hidden (Spoiler only)

These do not work for the obvious ones (Horizontal Rules, Images, and Emojis), and for all options in the Code category except inline code.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Bold

**Bold**: use either 2 **asterisks** or 2 **underscores** before and after the text for bold styling. The preferred syntax is to use asterisks for bold:

```markdown
**two asterisks**
**two underscores**
```

The two underscores is being converted to asterisks in the block above (asterisks preferred), so let's try it in an inline code block: `__two underscores__`.

### Italic

**Italic**: use a _single asterisk_ or _underscore_ before and after the text for italic styling. The preferred syntax is to use an underscore for italics:

```markdown
_single asterisk_
_single underscore_
```

Here is an inline example with a single asterisk: `*single asterisk*` (underscores preferred).

**_Bold and Italic_**: use either **_3 asterisks_** or **_2 asterisks and 1 underscore_** for bold and italic text. The preffered syntax is the latter:

```markdown
**_3 asterisks_**
**_2 asterisks and and 1 underscore_**
```

### Strike thru

**Strikethrough**: use two tildes `~~` (~~) before and after text that you want to display as ~~strikethrough~~:

```
~~double tildes~~
```

If you want, you can also do **~~bold strikethrough~~**, _~~italic strikethrough~~_, and **_~~bold italic strikethrough~~_**.

### Underline

This can only be done with the `<ins>` HTML element. This is **_NOT_** part of Markdown.

The links on GitHub are blue, bold and underlined (<ins>on hover</ins>). The `<ins>` HTML element underlines text and has normal font color and normal font-weight. No one familiar with GitHub will confuse it for a link. It's another styling effect that I find more useful than srikethrough.

This is <ins>text underlined</ins> with the `ins` HTML tag.

```markdown
This is <ins>text underlined</ins> with the `ins` HTML tag.
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Miscellaneous

The elements in this category are all unique and do not fit into any of the other category:

- Headings
- Blockquotes
- Descriptions
- Tables
- Horizontal rule
- Frontmatter

All elements in this category allow the text effects listed above except for horizontal rules and Frontmatter, and with an exception for descriptions.

### Headings

There are 6 headings just like in HTML. Use a single hashtag for H1 and 6 hashtags for H6. The top title of this docuement is an H1 with a single hash, this section (**Miscellaneous**) uses 2 hashtags, and this sub-section (**Headings**) uses 3 hashtags.

**NOTE**: There is an automatic horizontal rule added when you use syntax for H1 and H2.

```markdown
# MARKDOWN CHEAT SHEET (Heading 1)

## Misc (Heading 2)

### Headings (heading 3)

### Heading 4 (you most likely will not use H5 or H6)
```

Here is an example of using Bold, Italic, and Strikethrough in a heading:

```markdown
## ~~A Literal~~ <ins>Table</ins> of _Contents_
```

As you can see, strikethrough and italic worked on the heading, but using bold did not increase the font weight for headings because they are already bold.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Blockquotes

This is a nice effect which adds a border-left and padding-left to offset it from normal text:

> Use a **greater** than _sign_ (>) to quote a team member
>
> Create a <ins>space</ins> like above using > with no text (~~ignore~~)

```markdown
> Use a **greater** than _sign_ (>) to quote a team member
>
> Create a <ins>space</ins> like above using > with no text (~~ignore~~)
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

#### Alerts

Alerts are used to highlight important text with colours and icons. There is support for five distinct kinds of alerts. They have syntax similar to blockquotes but include syntax for images which is what displays the specific icons for each alert type:

```md
> [!NOTE]
> Essential details that users should not overlook, even when browsing quickly.

> [!TIP]
> Additional advice to aid users in achieving better outcomes.

> [!IMPORTANT]
> Vital information required for users to attain success.

> [!WARNING]
> Urgent content that requires immediate user focus due to possible risks.

> [!CAUTION]
> Possible negative outcomes resulting from an action.
```

> [!NOTE]
> Essential details that users should not overlook, even when browsing quickly.

> [!TIP]
> Additional advice to aid users in achieving better outcomes.

> [!IMPORTANT]
> Vital information required for users to attain success.

> [!WARNING]
> Urgent content that requires immediate user focus due to possible risks.

> [!CAUTION]
> Possible negative outcomes resulting from an action.

### Tables

Here is a generic table but the Table of Contents above is another version. The pipes create the columns, the colons with dashes create the alignment:

- A colon on the left of the dashes is left-aligned,
- A colon on the right is right-aligned,
- And a colon on both ends is centered

| Left aligned Content  | Center aligned Content | Right aligned Content |
| :-------------------- | :--------------------: | --------------------: |
| Content Left          |     Content Center     |         Content Right |
| Content Left          |     Content Center     |         Content Right |
| _Italic_              |        **Bold**        |     ~~Strikethrough~~ |
| <ins>Underlined</ins> |     Content Center     |         Content Right |

<br>

```markdown
| Left aligned Content  | Center aligned Content | Right aligned Content |
| :-------------------- | :--------------------: | --------------------: |
| Content Left          |     Content Center     |         Content Right |
| Content Left          |     Content Center     |         Content Right |
| _Italic_              |        **Bold**        |     ~~Strikethrough~~ |
| <ins>Underlined</ins> |     Content Center     |         Content Right |
```

Combination HTML and markdown table

```markdown
<table>
<tr>
<th>Heading 1</th>
<th>Heading 2</th>
</tr>
<tr>

<td>

| A   | B   | C   |
| --- | --- | --- |
| 1   | 2   | 3   |

</td><td>

| A   | B   | C   |
| --- | --- | --- |
| 1   | 2   | 3   |

</td></tr> </table>
```

<table>
<tr>
<th>Heading 1</th>
<th>Heading 2</th>
</tr>
<tr>

<td>

| A   | B   | C   |
| --- | --- | --- |
| 1   | 2   | 3   |

</td><td>

| A   | B   | C   |
| --- | --- | --- |
| 1   | 2   | 3   |

</td></tr> </table>

Boxed

```markdown
<table><tr><td>The quick brown fox jumps over the lazy dog.</td></tr></table>
```

<table><tr><td>The quick brown fox jumps over the lazy dog.</td></tr></table>

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Horizontal rules

Use 3 asterisks or 3 dashes with or without a space to create a horizontal rule:

---

```
- - -
---
* * *
***
```

**NOTE**: Make sure to hit <kbd>ENTER</kbd> twice if you intend to use 3 asterisks without spaces or it will set the text above it to an H3 tag. Directly below this paragraph is an HTML `<hr>` tag which looks identical to the HR at the top of this section.

<hr>

HR's look good for visual breaks. You could also use other keyboard symbols like periods:

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Descriptions

The following are HTML tags, **_NOT_** a part of markdown, but they do give you a nice indentation for visual variety.

The text in the tags can only be styled with the HTML tags related to bold, italic, strikethrough, or _underline_. As you can see, I used the `ins`, `b`, `em`, and `s` tags in the example below:

- `dl`: description list, the wrapper element for the other two
- `dt`: description term, that which you are defining or highlighting
- `dd`: description details, the actual definition or explanantion

<dl>
  <dt>Description <ins>List</ins></dt>
  <dd>Represents a description list. The <ins><b><em>dl</em></b></ins> element encloses a list of groups of terms (specified using the <ins><b><em>dt</em></b></ins> element) and descriptions (provided by <ins><b><em>dd</em></b></ins> elements). Common uses for this element are to implement a glossary or to display metadata (a list of key-value pairs) (<s>ignore</s>).</dd>
</dl>

```markdown
<dl>
  <dt>Description <ins>List</ins></dt>
  <dd>Represents a description list. The <ins><b><em>dl</em></b></ins> element encloses a list of groups of terms (specified using the <ins><b><em>dt</em></b></ins> element) and descriptions (provided by <ins><b><em>dd</em></b></ins> elements). Common uses for this element are to implement a glossary or to display metadata (a list of key-value pairs) (<s>ignore</s>).</dd>
</dl>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Frontmatter and YAML

Frontmatter in markdown files is not something you will use in general, but you should at least be aware of it. The actual syntax for markdown frontmatter (or _front matter_) is YAML syntax.

What is YAML? That is not pertinent to this repo, but GitHub actions are written in YAML.

Check out the file in this repo named [frontmatter.md](https://github.com/Kernix13/markdown-cheatsheet/blob/master/frontmatter.md) for an example of how it displays at the top of the file, as well as a description of what frontmatter is, and notes on syntax and YAML.

In that file I use frontmatter and it looks like it prints out as if it was a table. It has just 2 rows: 1st) the keys which become the table headers, and 2nd) the values in the first row. What is interesting is how the _tags_ are output with borders. I did not use nesting in that example, but I would assume that would output differently.

Here is an error I got when I tried nesting:

> ERROR: `Error in user YAML: (<unknown>): did not find expected '-' indicator while parsing a block collection at line 4 column 3`

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Links

This category accepts all text effects and includes:

- External links
- Anchor links (same page)
- Footnote links

### External

**External Links**: The syntax is to use square brackets around the link text and parentheses for the URL. You can also add an additional title for the link by adding a space after the URL and adding the link title in double quotes:

Here is a link to my [Beginner Git Commands](https://github.com/Kernix13/beginner-git-commands) repositiory. And here is the syntax:

```markdown
[Link text](URL 'Optional link title')
[Beginner Git Commands](https://github.com/Kernix13/beginner-git-commands 'Basic Git commands repo')
```

**NOTE**: Only use a title if it adds information. Don't set the title text to be the same as the link text.

Here is a bold, italic and strikethrough link:

- **[Google](https://google.com)**
- _[Google](https://google.com)_
- ~~[Google](https://google.com)~~
- <ins>[Google](https://google.com)</ins>

Why would you use a strikethorugh effect on a link? I'm not sure. For a page under construction, being moved, etc?

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Anchor

**Same page anchor links**: This can be done in at least two ways. For all the links in the table of contents above I use the simpler method. But for the **Back to Top** link I use an actual `<a>` tag.

For the simple links, use the same syntax as for **External Links** above with 2 exceptions for the URL part:

1. Precede the _URL_ with a hashtag
1. Use the exact same text as where you are linking to but...
   1. All the text needs to be in lowercase, and
   1. All words need to be connected with a dash (no spaces)

Here is an example for the _Strike thru_ section:

```markdown
[Strike thru](#strike-thru)
```

Here is the code for the anchor link using an HTML `<a>` and a `<div>` tag. I actually changed my 'Back to Top' link to be an `<a>` link inside of a `<div>` so that I could align the link to the right and use an HTML entity for an arrow up:

```html
<!-- element with id at top of page -->
<div id="back-to-top"></div>

<!-- The link you click to go back to top -->
<div align="right">
  &#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a>
</div>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Footnotes

**Footnote links**: I assume footnotes would be useful in a very technical or long README file. Use square brackets where you want a footnote link to appear and use a caret symbol (^) followed by the number of the footnote.

Then below that add the same syntax followed by a colon and the note itself - none of that will display on the page. That will make the footnote text appear at the bottom of your file:

Footnote.[^1]

Some other important footnote.[^2]

Use this for where you want the link: `[^1]`

Here is the actual footnote syntax:

```markdown
[^1]: This is footnote number one.
[^2]: Here is the second footnote.
```

[^1]: This is footnote number one.
[^2]: Here is the second footnote.

### At mentions

At mentions do not seem to work as links. This is an at mention test:

@Kernix13: Hello. This does not work in a markdown file, but it does create a link in Issues and PRs, and maybe in other areas as well. I need to do more research into this. Like Hidden text, this may only work on different platforms like Discord.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Lists

This category has:

- Unordered lists
- Ordered lists
- Nested lists
- Task lists

You can use all text effects but with one exception: None of the effects work for Task lists.

### Unordered

**Unordered lists**: You can use either an asterisk (`*`) or a dash (`-`) followed by a space to make a bulleted list. I prefer using a dash since you do not need to use the <kbd>SHIFT</kbd> key:

- _List item 1_
- **List item 2**
- List ~~item 3~~

```markdown
- _List item 1_
- **List item 2**
- List ~~item 3~~
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Ordered

**Ordered lists**: use a number followed by a period (1., 2., 3. etc.) and then a space to create an ordered list:

1. Ordered **item 1**
1. Ordered _item 2_
1. Ordered ~~item 3~~

```markdown
1. Ordered **item 1**
1. Ordered _item 2_
1. Ordered ~~item 3~~
```

**NOTE**: By using "1." for each list item, you can cut & paste to change the order of items and the numbering will change to match the new order.

Does this make sense? You can use both unordered and ordered together -> bullets with roamn numerals, or numbers with bullets:

1. - What?
1. - Really?
1. - Why?

- 10. What is this
- 15. Again?
- 20. Any use cases?

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Nested

**Nested list**: Use the <kbd>SPACEBAR</kbd> key to align the dash or asterisk directly beneath the first character in the parent list item above it to create a nested list:

- List item 1
- List item 2
  - Child item 1
  - Child item 2
    - Third level item
- List item 3

```markdown
- List item 1
- List item 2
  - Child item 1
  - Child item 2
    - Third level item
- List item 3
```

For a nested ordered list, do the same as for nested unordered lists - align the number to be below the first character of the parent item:

1. Ordered item 1
1. Ordered item 2
   1. Child item 1
   1. Child item 2
      1. Third level item
      1. Third level item 2
      1. Third level item 3
         1. Fourth level 1
         1. Fourth level 2
         1. Fourth level 3
1. Ordered item 3

```markdown
1. Ordered item 1
1. Ordered item 2
   1. Child item 1
   1. Child item 2
      1. Third level item
      1. Third level item 2
      1. Third level item 3
         1. Fourth level 1
         1. Fourth level 2
         1. Fourth level 3
1. Ordered item 3
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Tasks

You can create what looks like checkboxes and display completed tasks with a checkmark. It takes the form of an unordered list with the first characters being a set of square brackets which **_MUST_** have a space in them. For a completed task, add either a lower or uppercase "X":

- [ ] Incomplete _task_
- [x] Completed **task**
  - [ ] Incomplete ~~subtask~~
  - [x] Completed subtask

```markdown
- [ ] Incomplete _task_
- [x] Completed **task**
  - [ ] Incomplete ~~subtask~~
  - [x] Completed subtask
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Code

This category deals with inline code and various typs of code blocks and none of them accept Styles with the exception of `inline` and language code blocks using _markdown_ as the language:

- Inline code
- Generic code blocks
- <kbd>TAB</kbd> code blocks
- Code language blocks
- `Diff` code blocks

### Inline

Use a `single backtick` before and after text to display it as inline code:

```markdown
`single backtick`
```

Here are examples on inline as **`bold`**, _`italic`_, and ~~`strikethrough`~~. There is also a way to show language syntax highlighting (see _Language block_ section below) for inline code, but I think you need to use a package called `highlight.js`.

### Tab

It took me a while how to show the 3 backticks for a code block (next section). For that and other tricky markdown that will not dispay, hit the <kbd>TAB</kbd> button twice then enter your code:

    This is a **code** _block_ made by ~~hitting~~ TAB 2 X's

### Generic

To add code that requires more than 1 line then use 3 backticks, hit <kbd>ENTER</kbd>, add your code block, hit <kbd>ENTER</kbd> again and add 3 more back ticks.

    ```
    *, *::before, *::after {
      box-sizing: border-box;
    }
    ```

```
*, *::before, *::after {
  box-sizing: border-box;
}
```

**From GitHub docs**: _To display triple backticks in a fenced code block, wrap them inside quadruple backticks_.

However, you can also hit <kbd>TAB</kbd> twice:

    ```
    TAB twice to show the triple backticks
    ```

    ````
    ```
    Triples inside quadruples - TAB x 2 is easier
    ```
    ````

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Language block

This is what you want to use for code blocks. To highlight parts of your code add the language after the opening triple backticks. You'll have to do your own research but so far I've used the following languages: `md` or `markdown`, `html`, `css`, `js` or `javascript`, `jsx`, `php`, `xml`, `python`, `sql`, `bash` or `shell` or `sh`, and `apacheconf` (for Apache servers). I tried using `node` and `npm` for my node-npm repo but it had no effect.

    ```css
    rules here
    ```

**CSS**:

```css
a {
  text-decoration: none;
}
```

**HTML**:

```html
<img href="http://somewhere.com" />
```

**JavaScript**:

```js
console.log(${variable})
```

**PHP**:

```php
<?php the_content(); ?>
```

Here is a new one that I found on [Discord Markdown Text 101](https://gist.github.com/matthewzring/9f7bbfd102003963f9be7dbcf7d40e51) with a language prefix of `fix`. I assume this works on Discord but itdoes not work on GitHub:

```fix
everything is blue
= light blue after equal sign (but not in VS Code)
```

    ```fix
    everything is blue
    = light blue after equal sign (but not in VS Code)
    ```

Here is the full list of supported languages and code syntax highlighting.

Check out the article [Languages Supported by Github Flavored Markdown](https://www.rubycoloredglasses.com/2013/04/languages-supported-by-github-flavored-markdown/) from 12-8-2020. Also check out the [highlight.js](https://github.com/highlightjs/highlight.js/blob/main/SUPPORTED_LANGUAGES.md) repo:

```markdown
actionscript3
apache
applescript
asp
brainfuck
c
cfm
cjs
clojure
cmake
coffee-script, coffeescript, coffee
cpp - C++
cs
csharp
css
csv
bash, sh, zsh
diff
elixir
erb - HTML + Embedded Ruby
go
haml
http
java
javascript
js
json
jsx
less
lolcode
make - Makefile
markdown
matlab
nginx
objectivec
pascal
PHP
Perl
python
profile - python profiler output
rust
salt, saltstate - Salt
shell, sh, zsh, bash - Shell scripting
scss
sql
svg
swift
rb, jruby, ruby - Ruby
smalltalk
vim, viml - Vim Script
volt
vhdl
vue
xml - XML and also used for HTML with inline CSS and Javascript
yaml
```

I've also noticed that `ini` and `TOML` as the language block language also show syntax highlighting.

For terminal commands like for NPM, use `bash`, `sh`, or `zsh`.

Trying to find a language to style terminal errors or errors & warnings in DevTools is difficult. The best languages I found for that are `c++` and `python`. The syntax highlighting isn't perfect but it at least has some highlighting.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Diff

This is really nice for highlighting text or code that was changed. Use `diff` after the opening triple backticks. Then use a minus sign (`-`) for what was changed, and a plus symbol (`+`) for the new version:

```diff
- this code or text is the old version
+ this is what it was changed to
```

````
```diff
- this code or text is the old version
+ this is what it was changed to
```
````

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Hidden Elements

This is an odd category with 3 effects, one of which you have probably only seen on Discord:

- Comments
- Spoiler text
- Details

Only Spoiler text accepts text effects.

### Comments

This is a nice way to add a comment in the editor view of your markdown file. This would be good for teams members editing a documentation page. The best way is to use HTML syntax:

<!-- There is a comment here that you can't see -->

```markdown
<!-- There is a comment here that you can't see -->
```

Comments used in language code blocks will match the language. You can use the `CTRL+/` shortcut. For example, in JavaScript or PHP you will get `//` using that shortcut, or `/* */` in CSS, `#` in bash files, and `<!-- -->` in HTML.

### Spoiler

On Discord you may sometimes see a black rectangle that reveals text or code when you click on it. Use double pipes before and after the word(s)/code that you want to conceal:

```markdown
||Spoiler text|| in Discord
```

**NOTE**: This does not work on Slack or here on GitHub.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Details

This isn't a markdown thing but it is another example of using HTML tags in a Markdown file. It has the same effect as an accordian. I'm not sure why you would use this but here is how you would do it:

<details>
  <summary>Title 1</summary>
  <p>Some hidden content goes here</p>
</details>
<details>
  <summary>Title 2</summary>
  <p>Same stuff here</p>
</details>

```html
<details>
  <summary>Title 1</summary>
  <p>Some hidden content goes here</p>
  Here is some more without a paragraph tag
</details>
<details>
  <summary>Title 2</summary>
  <p>Same stuff here</p>
</details>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Visual Elements

The five sections below deal with adding visual-based elements to your markdown file that require some kind of extra code/syntax: `images`, `math expressions`, `emojis`, `shields`, `diagrams`, and `HTML entities`.

### Images

Images use the same syntax as **Links** except for the addition of an exclamation mark (`!`) immediately before the opening square bracket. You can also use the optional title text. The example image below shows the dimensions but that is just an example. It's up to you to decide the image sizes you want for your files:

<br />

![picture alt text](./markdown-image.png 'Title is optional')

    ![picture alt](./markdown-image.png 'Title is optional')

raw.githubusercontent: I noticed that you can paste images into parts of GitHub. You can do it in a markdown file, but then you will have to pull the changes. I've also seen it done in `Pull requests` and `Issues` tabs. Here is an example:

```html
<img
  src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg"
/>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Math

Finally, per GitHub:

> ...math expressions can be rendered in Markdown on GitHub using $$ as a delimiter for code blocks with math content or the $ delimiter for inline math expressions.

1. Use a single dollar sign (`$`) at the beginning and end of an inline math expression.
2. Use 2 dollar sign (`$$`) at the beginning and end for a block of math expressions.

Inline example: this `$(ax^2 + bx + c = 0)$` renders as $(ax^2 + bx + c = 0)$.

Inline exception: use `\$` to escape, and therefore use, a dollar sign in an equation (`$(\$4.00 - \$1.50 = \$2.50)$`): $(\$4.00 - \$1.50 = \$2.50)$

Inline exception 2: use `<span>$</span>` for inline use of dollar sign before a math expression.

Block example: `$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$` renders as:

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

Block example 2: This `$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$` renders as:

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

Here are the important symbols to know:

- `^` = exponent, e.g. $a^3$
- `{ }` = required for certain expressions such as square root
- `\pm` = plus\minus symbol: $\pm$
- `\sqrt` = square root symbol: $\sqrt{b}$
- `\over` = division: $a \over b$
- `\leq` = less than or equal to: $\leq$
- `\geq` = greater than or equal to: $\geq$
- `\ne` = not equal to: $ \ne $
- `\sum` = Sigma, summation symbol: $\sum$
- `\val` = sub-script value: $a_i$
- `\{val=num}^n` = start val and max (n) val for sum
- `\Omega` and `\omega` = greek Omega or omega
- `\int` = interval
- `\bmod` and `\pmod` = modular operators
- `\frac` = fractions
- `\binom` = binomial coefficient

Not sure for the following: `\left`, `\right`, `\forall`, `\partial`, `\rho`, `\nabla`, `\cdot`, `\vec`, `\mathrm`, `\in`, ...

For some reason the symbols in the lists above are not all displaying (?)

#### Examples for Greek letters

Greek letters are commonly used in mathematics, and they are very easy to type in math mode. You just have to type the name of the letter after a backslash: if the first letter is lowercase, you will get a lowercase Greek letter, if the first letter is uppercase (and only the first letter), then you will get an uppercase letter. Note that some uppercase Greek letters look like Latin ones.

Use `\alpha, \Alpha, \beta, \Beta, \gamma, \Gamma, \pi, \Pi, \phi, \varphi, \mu, \Phi, \Omega, \omega` for $\alpha \beta \gamma \Gamma \pi \Pi \phi \varphi \mu \Phi \Omega \omega \Theta \theta$, etc.

#### Examples for Operators

An operator is a function that is written as a word: e.g. trigonometric functions (sin, cos, tan), logarithms and exponentials (log, exp), limits (lim), as well as trace and determinant (tr, det).

Use `\lim\limits_{x \to \infty} \exp(-x) = 0` for $\lim\limits_{x \to \infty} \exp(-x) = 0$

#### Examples of Powers and indices

Powers and indices are equivalent to superscripts and subscripts in normal text mode. The caret character (`^`) is used to raise something, and the underscore (`_`) is for lowering. For example, use `k_{n+1} = n^2 + k_n^2 - k_{n-1}` for $k_{n+1} = n^2 + k_n^2 - k_{n-1}$.

For powers with more than one digit, surround the power with `{ }`: use `n^{22}` for $n^{22}$.

An underscore (`_`) can be used with a vertical bar (`{\displaystyle |}|`) to denote evaluation using subscript notation: use `f(n) = n^5 + 4n^2 + 2 |_{n=17}` for $f(n) = n^5 + 4n^2 + 2 |_{n=17}$.

#### Examples of Fractions and Binomials

A fraction is created using the `\frac{numerator}{denominator}` command. Use `\frac{n!}{k!(n-k)!} = \binom{n}{k}` for $$\frac{n!}{k!(n-k)!} = \binom{n}{k}$$

You can embed fractions within fractions using `\frac{\frac{1}{x}+\frac{1}{y}}{y-z}`:

$$\frac{\frac{1}{x}+\frac{1}{y}}{y-z}$$

The `\tfrac` and `\dfrac` commands force the use of the respective styles, `\textstyle` and `\displaystyle`. Similarly, the `\tbinom` and `\dbinom` commands typeset the binomial coefficient.

For relatively simple fractions, especially within the text, it may be more aesthetically pleasing to use powers and indices instead: `^3/_7` for $^3/_7$

If you use them throughout the document, usage of `xfrac` package is recommended. This package provides `\sfrac` command to create slanted fractions. If fractions are used as an exponent, curly braces have to be used around the `\sfrac` command.

Check out the Wikipedia article [LaTeX/Mathematics](https://en.wikibooks.org/wiki/LaTeX/Mathematics) for more information. Or click on the following links for specific sections not covered above:

- [Multiplication of two numbers](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Multiplication_of_two_numbers)
- [Roots](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Roots)
- [Sums and integrals](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Sums_and_integrals)
- [Brackets, braces and delimiters](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Brackets,_braces_and_delimiters)
- [Matrices and arrays](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Matrices_and_arrays)
- [Adding text to equations](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Adding_text_to_equations)
- [Formatting mathematics symbols](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Formatting_mathematics_symbols)
- [Color](https://en.wikibooks.org/wiki/LaTeX/Mathematics#Color)

Color example: try `k = {\color{red}x} \mathbin{\color{blue}-} 2` for $k = {\color{red}x} \mathbin{\color{blue}-} 2$

Other links:

- [MathJax](https://www.mathjax.org/)
- GitHub blog post [Math support in Markdown](https://github.blog/2022-05-19-math-support-in-markdown/)

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Emojis

I'm not a huge fan of emojis, but here are some that I would consider using. The syntax is the emoji code in between colons:

```markdown
:Emoji_code:
```

Approval: :+1:, :smile:, :ok_hand:, :white_check_mark:, :heavy_check_mark:, :star:, :star2:, :heart:, :exclamation:

```markdown
:+1:, :smile:, :ok_hand:, :white_check_mark:, :heavy_check_mark:,
:star:, :star2:, :heart:, :exclamation:
```

Disapproval, questions, problems: :-1:, :question:, :grey_question:, :x:, :boom:, :bomb:, :astonished:, :warning:, :interrobang:

```markdown
:-1:, :question:, :grey_question:, :x:, :boom:, :bomb:, :astonished:,
:warning:, :interrobang:
```

Directional: :point_right:, :point_left:, :arrow_left:, :arrow_right:, :arrow_up:, :arrow_down:

```markdown
:point_right:, :point_left:, :arrow_left:, :arrow_right:, :arrow_up:, :arrow_down:
```

Time, alarms: :bell:, :no_bell:, :hourglass:, :alarm_clock:, :watch:, :calendar:

```markdown
:bell:, :no_bell:, :hourglass:, :alarm_clock:, :watch:, :calendar:
```

Weather/nature: :sunny:, :cloud:, :snowflake:, :zap:, :high_brightness: 💧 ☔ ⭐ 🌡️ ❄️ ⛄ 🌱 🐚 🍁 🍃 🌲 🌳

```markdown
:sunny:, :cloud:, :snowflake:, :zap:, :high_brightness: :droplet: :umbrella: :star: :thermometer: :snowflake: :snowman: :seedling: :shell: :maple_leaf: :leaves: :evergreen_tree: :deciduous_tree:
```

Office/Business: :scissors:, :pushpin:, :paperclip:, :phone:, :copyright:, :email: 💻 📞 📫 💵 💳 🔗 📎 💲 ✏️

```markdown
:scissors:, :pushpin:, :paperclip:, :phone:, :copyright:, :email: :computer: :telephone_receiver: :mailbox: :dollar: :credit_card: :link: :paperclip: :heavy_dollar_sign: :pencil2:
```

Miscellaneous/playful: :alien:, :green_heart:, :blue_heart:, :purple_heart:, :mushroom:, :pizza:, :beer:, :icecream:, :sound:, :speaker:, :lock:, :guitar:, :one:, :two: (and other #'s), <br>
:link:, :speech_balloon:, :mag:, :mag_right:, :key:, :bulb: 👤 🐱 🐶 🦴 🌐 🌎 🎃 👻 🎅 🎄 🎁 🎈 🔦 🚽 🔧 🔨 ⛺ ⛵ ⚓ 🚀 ✈️ 🔥 💀 🚩 ♾️ 📐 🍷 💭

```markdown
:alien:, :green_heart:, :blue_heart:, :purple_heart:, :mushroom:, :pizza:, :beer:,
:icecream:, :sound:, :speaker:, :lock:, :guitar:, :one:, :two: (and other #'s),
:link:, :speech_balloon:, :mag:, :mag_right:, :key:, :bulb: :bust_in_silhouette: :cat: :dog: :bone: :globe_with_meridians: :earth_americas: :jack_o_lantern: :ghost: :santa: :christmas_tree: :gift: :balloon: :flashlight: :toilet: :wrench: :hammer: :tent: :sailboat: :anchor: :rocket: :airplane: :fire: :skull: :triangular_flag_on_post: :infinity: :triangular_ruler: :wine_glass: :thought_balloon:
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Shields

Check the file `shields.md` for a full list.

[Shields.io](https://shields.io/) generates shields/badges for different apects of your repo. Here are the shields I have for my [WriterAssist](https://github.com/Kernix13/WriterAssist) repo with descriptions above the badges:

```md
GitHub commit activity:
![GitHub commit activity](https://img.shields.io/github/commit-activity/y/Kernix13/WriterAssist?style=flat-square)
GitHub contributors:
![GitHub contributors](https://img.shields.io/github/contributors/Kernix13/WriterAssist?style=flat-square)
GitHub all releases:
![GitHub all releases](https://img.shields.io/github/downloads/Kernix13/WriterAssist/total?style=flat-square)
GitHub language count:
![GitHub language count](https://img.shields.io/github/languages/count/Kernix13/WriterAssist?style=flat-square)
GitHub top language:
![GitHub top language](https://img.shields.io/github/languages/top/Kernix13/WriterAssist?style=flat-square)
license
![GitHub](https://img.shields.io/github/license/Kernix13/WriterAssist?style=flat-square)
```

In the beginning just add what you can, even if the values are `0`, though some shields with a `null` value will display a zero, others will not even display the badge. Here are the badges I think are good for beginners:

- **Analysis badges**: GitHub language count, GitHub top language, and GitHub search hit counter
- **Size badge**: GitHub repo file count
- **Downloads badge**: GitHub all releases
- **Funding badge**: GitHub sponsors (probably not for beginners)
- **Issue tracking badges**: GitHub issue/pull request detail, GitHub issues, GitHub closed issues, ...and many more, (_what is hacktoberfest?_)
- **License badge**: GitHub license
- **Social badges**: GitHub followers, forks, repo stars, users stars, watchers, ...
- **Version badge**: GitHub manifest version
- **Activity badges**: GitHub contributors, GitHub commit activity, GitHub last commit, GitHub release date,
- **Other badges**: GitHub discussions, GitHub package.json dynamic (keywords)

Shield.io will build the links for you, but here is the breakdown of the structure:

```markdown
https://img.shields.io/github/ + Label/ + user/ + repo + ?options
```

You do not have to go to the shields website if you want shields for a repo that you already. Just change the repo part of the link. As of 8/26/2022 I have 3 shields for this repo. Here they are following the sequence above with `constant` standing for the string `https://img.shields.io/github/`:

```markdown
<!-- Forks -->

constant + forks/Kernix13/markdown-cheatsheet?style=flat-square

<!-- Commits -->

constant + commit-activity/y/Kernix13/markdown-cheatsheet?style=flat-square

<!-- Contributors -->

constant + contributors/Kernix13/markdown-cheatsheet?style=flat-square
```

For the `?style=` part of the link, I like `flat-square` and `for-the-badge` (much larger). You can also choose _Copy HTML_ to get an `img` tag instead of a markdown link. I actually switched from the markdown syntax to an `img` tag inside of `<span>` tags to get them to display inline:

```markdown
<span><img alt="GitHub forks" src="https://img.shields.io/github/forks/Kernix13/markdown-cheatsheet?style=for-the-badge"></span>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Devicons

Devicons are the language and web tool icons you see mostly in people's profile README files. Check out [Devicons on GitHub](https://github.com/devicons/devicon/tree/master/icons) for the full list languages and tools and let me know if you find another/better list:

```markdown
<!-- img src example -->

https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg

<!-- full example on an img tag inside a link tag -->

<a href="https://getbootstrap.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a>
```

You will have to find all the language and tool icons that you want for your markdown files. Here are examples of Bootstrap and CSS3 devicons in 1) an `img` tag inside an `a` tag, 2) an `img` tag only, and 3) an `img` tag inside a `span` tag:

#### Devicons in an anchor and image tag

<a href="https://getbootstrap.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a>
<a href="https://getbootstrap.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" alt="vs code" width="40" height="40"/> </a>

#### Devicons in an image tag only

<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/>
<img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" alt="vs code" width="40" height="40"/>

#### Devicons in a span and image tag

<span> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </span>
<span> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vscode/vscode-original.svg" alt="vs code" width="40" height="40"/> </span>

They are all inline except for the sole `img` tags. I think a span tag with `align="left"` or `center` would be best, although you could do `right` to have them stand out or as a visual change to the normal left alignment.

When you see a profile README with language/tool icons that you would like to use, then go into the markdown to get a copy of the `src` and then add it to your profile README. Or go to the devicons repo linked above, search for your languages/tools in the icons folder and go into that folder. Click on an image, and if you like the image click the `Raw` button and copy the URL in the address bar to use as the `src` attribute.

**NOTE 1**: The link attribute `target="_blank"` does not open links in a new tab.

**NOTE 2**: You need to set the `width` and `height` for the devicon's `img` tags. Currently I have 40 or 48 pixels for my devicons. Find the pixel size that works for you.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Mermaid Diagrams

This is a new markdown element I just became aware of. Check out [Mermaid on GitHub](https://github.com/mermaid-js/mermaid#readme) for more information or go to their [docs page](https://mermaid.js.org/intro/). But it's basically a language code block that remders various diagrams with very specific syntax. And the diagrams have buttons for, zoom in/out, position change, and popout box. Check this out:

      graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;

```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

Or this

flowchart LR

    A[Hard] -->|Text| B(Round)
    B --> C{Decision}
    C -->|One| D[Result 1]
    C -->|Two| E[Result 2]

```mermaid
flowchart LR

A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

As I learn more I will add more but this is really cool! Check out my file `mermaid.md` for in-depth notes.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### HTML entities

This actually is not a markdown thing but it's nice having a list for use in your README files. This would be helpful if you have a client needing work with a science website, math site, music site, etc.

Bold, Italic and strikethough work for some of the elements below but not for all of them. And strikethorugh works the least of all. It's up for you to test them. Here is my list:

<br>

**Business & Financial**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&copy;` | &copy; | Copyright |
| `&#8471;` | &#8471; | Sound Copyright |
| `&trade;` | &trade; | Trademark |
| `&reg;` | &reg; | Registered TM |
| `&dollar;` | &dollar; | Dollar |
| `&cent;` | &cent; | Cent |
| `&pound;` | &pound; | Pound |
| `&euro;` | &euro; | Euro |
| `&#9993;` | &#9993; | Envelope |
| `&check;` | &check; | Check mark |
| `&#9998;` | &#9998; | Pencil |
| `&#10002;` | &#10002; | Pen tip |
| `&#9990;` | &#9990; | Phone |
| `&#9986;` | &#9986; | Scissors |
| `&#9888;` | &#9888; | Warning |

<br>

**Directional**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&larr;` | &larr; | Left arrow |
| `&rarr;` | &rarr; | Right arrow |
| `&uarr;` | &uarr; | Up arrow |
| `&darr;` | &darr; | Down arrow |
| `&#8598;` | &#8598; | Northwest arrow |
| `&#8599;` | &#8599; | Northeast arrow |
| `&#8600;` | &#8600; | Southeast arrow |
| `&#8601;` | &#8601; | Southwest arrow |
| `&#9650;` | &#9650; | Up triangle |
| `&#9660;` | &#9660; | Down triangle |
| `&#9654;` | &#9654; | Right triangle |
| `&#9664;` | &#9664; | Left triangle |
| `&#10146;` | &#10146; | Arrowhead |
| `&#10139;` | &#10139; | Drafting point |

<br>

**Math and science**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&deg;` | &deg; | Degree |
| `&plusmn;` | &plusmn; | Plus minus |
| `&sup2;` | 3&sup2; | Supercript 2 |
| `&#8322;` | H&#8322;O | Subscript 2 |
| `&#8323;` | NO&#8323;| Subscript 3 |
| `&frac14;` | &frac14; | 1/4 fraction |
| `&frac38;` | &frac38; | 3/8 fraction |
| `&times;` | &times; | Multiplication |
| `&divide;` | &divide; | Division |
| `&minus;` | &minus; | Subtraction |
| `&empty;` | &empty; | Empty |
| `&Phi;` | &Phi; | Phi |
| `&pi;` | &pi; | Pi |
| `&#8486;` | &#8486; | Omega |
| `&sum;` | &sum; | Sum, Sigma |
| `&radic;` | &radic; | Square root |
| `&infin;` | &infin; | Infinity |
| `&sim;` | &sim; | Proportional |
| `&asymp;` | &asymp; | Approximately |
| `≠` | ≠ | Not equal |
| `&le;` | &le; | Less or equal to |
| `&ge;` | &ge; | Greater or equal |
| `&ang;` | &ang; | Angle |
| `&angmsd;`| &angmsd; | Measured angle |
| `&or;` | &or; | Down angle |

**NOTE**: For subscripts 0 thru 9, change the last number, e.g.:

Zero&#8320; code = `&#8320;` so change 8320 to 8321 for subscript 1 (One&#8321;), change 8320 to 8322 for subscript 2 (Two&#8322;), etc.

<!--
http://thenewcode.com/1005/Writing-Musical-Notation-on-Web-Pages-The-Basics
-->

<br>

**Music**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&#9837;`| &#9837; | Music flat |
| `&#9838;`| &#9838; | Music natural |
| `&#9839;`| &#9839; | Music sharp |
| `&#119082;`| &#119082; | Double Sharp |
| `&#119083;`| &#119083; | Double flat |
| `&#119070;`| &#119070; | G-clef |
| `&#119073;`| &#119073; | C-clef |
| `&#119074;`| &#119074; | F-clef |
| `&#119092;`| &#119092; | Common time |
| `&#119093;`| &#119093; | Cut time |
| `&#248;`| &#248; | Half-diminished 7th |
| `&#119132;`| &#119132; | Breve |
| `&#119133;`| &#119133; | Whole note |
| `&#119134;`| &#119134; | Half note |
| `&#9833;`| &#9833; | Quarter note |
| `&#119135;`| &#119135; | Quarter note |
| `&sung;`| &sung; | 8th note |
| `&#9834;`| &#9834; | 8th note |
| `&#119136;`| &#119136; | 8th note |
| `&#9835;`| &#9835; | Beamed 8th note |
| `&#119137;`| &#119137; | 16th note |
| `&#9836;`| &#9836; | Beamed 16th note |
| `&#119094;`| &#119094; | Octave |
| `&#119057;` | &#119057; | Fermata |
| `&#119058;` | &#119058; | Breath mark |
| `&#119059;` | &#119059; | Caesura |
| `&#119046;` | &#119046; | Left repeat |
| `&#119047;` | &#119047; | Right repeat |
| `&#119048;` | &#119048; | Repeat |
| `&#119049;` | &#119049; | Dal Segno |
| `&#119050;` | &#119050; | Da Capo |
| `&#119051;` | &#119051; | Segno |
| `&#119052;` | &#119052; | Coda |
| `&#119183;` | &#119183; | Piano |
| `&#119184;` | &#119184; | Mezzo |
| `&#119185;` | &#119185; | Forte |
| `&#119186;` | &#119186; | Crescendo |
| `&#119187;` | &#119187; | Decrescendo |
| `&#119040;` | &#119040; | Single barline |
| `&#119041;` | &#119041; | Double barline |
| `&#119042;` | &#119042; | Final barline |
| `&#119217;` | &#119217; | Glissando up |
| `&#119218;` | &#119218; | Glissando down |
| `&#119188;` | &#119188; | Grace note |
| `&#119191;` | &#119191; | Turn |
| `&#119192;` | &#119192; | Inverted turn |
| `&#119081;` | &#119081; | Full measure rest |
| `&#119098;` | &#119098; | Dbl whole note rest |
| `&#119099;` | &#119099; | Whole rest |
| `&#119100;` | &#119100; | Half rest |
| `&#119101;` | &#119101; | Quarter rest |
| `&#119102;` | &#119102; | Eigth rest |
| `&#119103;` | &#119103; | Sixteenth rest |
| `&#119060;` | &#119060; | Brace |
| `&#119061;` | &#119061; | Bracket |
| `&#119163;` | &#119163; | Accent |
| `&#119164;` | &#119164; | Staccato |

<br>

**Miscellaneous**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&spades;` | &spades; | Spade |
| `&clubs;` | &clubs; | Club |
| `&hearts;` | &hearts; | Heart |
| `&diams;` | &diams; | Diamond |
| `&star;`| &star; | Star |
| `&#9812;`| &#9812; | King |
| `&#9813;`| &#9813; | Queen |
| `&#9814;`| &#9814; | Rook |
| `&#9815;`| &#9815; | Bishop |
| `&#9816;`| &#9816; | Knight |
| `&#9817;`| &#9817; | Pawn |
| `&starf;`| &starf; | Filled star |
| `&female;`| &female; | Female |
| `&male;`| &male; | Male |
| `&para;` | &para; | Paragraph |
| `&#167;` | &#167; | Selection sign |
| `&#9992;` | &#9992; | Airplane |
| `&#10007;` | &#10007; | Ballot X |
| `&#10008;` | &#10008; | Heavy Ballot X |
| `&#9728;` | &#9728; | Black Sun |
| `&#9788;` | &#9788; | White Sun |
| `&#x2601;` | &#x2601; | Cloud |
| `&#10052;` | &#10052; | Snowflake |
| `&#x2602;` | &#x2602; | Umbrella |
| `&not;` | &not; | Negation |
| `&macr;` | &macr; | Spacing Macron |
| `&laquo;` | &laquo; | Left quote |
| `&raquo;` | &raquo; | Right quote |
| `&ndash;` | &ndash; | En dash |
| `&mdash;` | &mdash; | Em dash |
| `&#8416;` | &#8416; | Circle slash |
| `&#9752;` | &#9752; | Shamrock |
| `&#9774;` | &#9774; | Peace symbol |
| `&#10084;` | &#10084; | Heavy heart |

<br>

**Astrology**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&oplus;` | &oplus; | Earth |
| `&#9793;` | &#9793; | Earth |
| `&#9737;` | &#9737; | Sun |
| `&#9790;` | &#9790; | Moon |
| `&#9800;`| &#9800; | Aries |
| `&#9801;`| &#9801; | Taurus |
| `&#9802;`| &#9802; | Gemini |
| `&#9803;`| &#9803; | Cancer |
| `&#9804;`| &#9804; | Leo |
| `&#9805;`| &#9805; | Virgo |
| `&#9806;`| &#9806; | Libra |
| `&#9807;`| &#9807; | Scorpio |
| `&#9808;`| &#9808; | Sagittarius |
| `&#9809;`| &#9809; | Capricorn |
| `&#9810;`| &#9810; | Aquarius |
| `&#9811;`| &#9811; | Pisces |
| `&#9791;`| &#9791; | Mercury |
| `&#9792;`| &#9792; | Venus|
| `&female;`| &female; | Venus|
| `&#9794;`| &#9794; | Mars |
| `&male;`| &male; | Mars |
| `&#9795;`| &#9795; | Jupiter |
| `&#9796;`| &#9796; | Saturn |
| `&#9797;`| &#9797; | Uranus |
| `&#9798;`| &#9798; | Neptune |
| `&#9799;`| &#9799; | Pluto |
| `&#9738;`| &#9738; | Ascending node |
| `&#9739;`| &#9739; | Descending node |
| `&#9740;`| &#9740; | Conjunction (0&deg;) |
| `&#9914;`| &#9914; | Semi-sextile (30&deg;) |
| `&ang;`| &ang; | Semi-square (45&deg;) |
| `&#9913;`| &#9913; | Sextile (60&deg;) |
| `&#9744;`| &#9744; | Square (90&deg;) |
| ``| | Trine (120&deg;) | | `&#9915;`| &#9915; | Quincunx (150&deg;) | | `&#9741;`| &#9741; | Opposition (180&deg;) |

<br>

**Esoteric**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&#8501;`| &#8501; | Aleph |
| `&#8502;`| &#8502; | Bet/Beth |
| `&#8503;`| &#8503; | Gimel |
| `&#8504;`| &#8504; | Dalet/Daleth |
| `&#9764;`| &#9764; | Caduceus Staff |
| `&#9877;`| &#9877; | Staff of Aesculapius |
| `&#9765;`| &#9765; | Ankh |
| `&#9766;`| &#9766; | Orthodox Cross |
| `&#9767;`| &#9767; | Chi Rho |
| `&#9768;`| &#9768; | Cross or Lorraine |
| `&#9769;`| &#9769; | Cross of Jerusalem |
| `&#9775;`| &#9775; | Yin Yan, Ying Yang |
| `&#9776;`| &#9776; | Heaven I-Ching |
| `&#9777;`| &#9777; | Lake |
| `&#9778;`| &#9778; | Fire |
| `&#9779;`| &#9779; | Thunder |
| `&#9780;`| &#9780; | Wind |
| `&#9781;`| &#9781; | Water |
| `&#9782;`| &#9782; | Mountain |
| `&#9783;`| &#9783; | Earth |
| `&#9866;`| &#9866; | Yang |
| `&#9867;`| &#9867; | Yin |
| `&#9868;`| &#9868; | Greater Yang |
| `&#9869;`| &#9869; | Greater Yin |
| `&#9870;`| &#9870; | Lesser Yang |
| `&#9871;`| &#9871; | Lesser Yin |
| `&#9784;`| &#9784; | Wheel of Dharma |
| `&#10017;`| &#10017; | Seal of Solomon |
| `&#10029;`| &#10029; | Pentagram |

NOTE: I ned to get the number ranges for the categories of entities. Check out the first entry of HTML symbols on W3Schools called [UTF-8 General Punctuation](https://www.w3schools.com/charsets/ref_utf_punctuation.asp).

<br>

**Hotkey list**:
| Key | Symbol |
| --- | --- |
| Option | ⌥ |
| Control | ⌃ |
| Command | ⌘ |
| Shift | ⇧ |
| Caps Lock | ⇪ |
| Tab | ⇥ |
| Esc | ⎋ |
| Power | ⌽ |
| Return | ↩ |
| Delete | ⌫ |

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## HTML

<!-- STOPPED EDITS/REVISIONS HERE DEC 18, 2022 -->

The one thing I want to look into is using videos, animated GIFs, more HTML tags in my markdown files, and also column layouts using tables.

I used a GitHub generator for my Profile README. In there are `<p>`, `<a>`, and `<img>` tags. In the Details section above, there are `<details>`, `<summary>`, and `<p>` tags. I found this gist called <q>[HTML Tags You Can Use on GitHub](https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2)</q>. That document mentions some tags you can use.

I tested every HTML tag that made sense. I skipped tags like `section`, `header`, `nav`, etc. Here is a breakdown of that testing.

### Block elements

NOTE: I should not have pushed `index.html` because I was only using to test the syntax for some HTML tags.

_Duplicates markdown_: `blockquote`, `h1` thru `h6`, `hr`, `ol` `ul` `li`, `pre`, `table`

_No markdown equivalent_: `details` with `summary`, `dl` `dt` `dd` (indent), `div`, and `span`.

> Is **align** an attribute? How do I find similar attributes like that?

**Attributes**:

> Is `align` an actual attribute or is it inline CSS?

I have only found that the `align` attribute works, other than the obvious ones like `href` and `src`. Below are the HTML elements that worked when I used `align` though they may work for other elements:

- `blockquote`: align (center, right)
- `h1` thru `h4`: align (center, right)
- `h5` and `h6`: align (center, right), very small font size!
- `div`: align (center, right)
- `p`: align (center, right)
- `pre`: align (center, right) - looks odd
- `ul`, `ol`, `li`: align (center, right) - looks odd

<blockquote align="center">Testing alignment</blockquote>

<pre align="center">
<code>testing align="center" in a pre block </code>
</pre>

Unless there is a way to display the tags differently, then I do not see the point of using `pre`, `table`, `lists`, or `blockquote`. Especially the `table` tag since there are a lot of tags you need to enter.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Inline elements

> `img` tags display as block level unless nested in table cells or `<span>` tags

_Duplicates markdown_: `<a>`, `code`, `img` (width, align [center, right]), `b` and `strong` (display as Bold), `del` and `s` (display as Strikethrough), `em` and `i` and `var` (display as Italic).

_No markdown equivalent_: `br` (line break), `ins` and `u` (underline), `sup` and `sub` (superscript and subscript), `samp` (Monospaced font), `q` (quotes), `kbd` (keyboard keys), `span`.

**Attributes notes**:

- `a`: target="\_blank" does not work
- `img`: align, width, and height all work

Some _Global attributes_ that may have a use: id, draggable, **style**, **title**, tabindex, contenteditable, autofocus.

> What is **_align_**? Do all these accept inline CSS?

The only tags worth using IMO:

- `a` for anchor links with HTML entities in the link text
- `headings` align center or right
- `p` for align center or right
- `div` as visual dividers using dash (-) or underscore (\_) or equals (=) or other characters. But can't you just use the characters instead?
- `br` for line breaks of paragrpah text or as a alternate spacer to `div`
- `img` to set width and height and align center or right
- `ins` for underline (`u` is actually better but does not display on GitHub)
- `kbd` for keyboard keys
- `samp` for monospaced font as a styling choice
- `sup` and `sub` for superscript and subscript
- `dl` `dt` `dd` maybe for the indentation of the definition

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

#### HTML tag examples

The large gap above the title is from 2 `<br>` tags. Use only one for a normal separation.

| HTML Tag |                     Result                     |
| :------- | :--------------------------------------------: |
| `ins`    |           <ins>underlined text</ins>           |
| `u`      |         <u>No underline on GitHub</u>          |
| `kbd`    | <kbd>CTRL</kbd>+<kbd>C</kbd>, <kbd>ENTER</kbd> |
| `samp`   |      <samp>This is monospaced font</samp>      |
| `sup`    |                 2<sup>3</sup>                  |
| `sub`    |                 H<sub>2</sub>O                 |

<h3 align="center">H3 tag with align="center"</h3>
<p align="center">Paragraph tag with align="center"</p>
<h3 align="right">H3 tag with align="right"</h3>
<p align="right">Paragraph tag with align="right"</p>

> I think an H2 heading that is center aligned would look great but not a paragraph. When would align right look good?

Here is an example of an HTML entity in an `<a>` tag: <a href="#html-entities">&uarr; HTML Entities Section</a><br>
Here is an example of an Emoji in an `<a>` tag: <a href="#emojis">:smile: Emoji section</a>

**NOTE**: For my anchor links (same page) in my [Beginner Git Commands](https://github.com/Kernix13/beginner-git-commands) repo, I wanted to use a downward arrow that points to the right for my H3 sections. I could not do that with `[text](#text)` so I had to use an `<a>` tag. In that same repo I use a `div` tag with underscores with spaces between them for a visual separation between the start of H2 sections and the end of the section above. Here is an example of an H3 with the arrow entity code with an `id` for the anchor link in the Table of Contents:

    <h3 id="commands-after-initial-push">&#10551; Commands after initial push</h3>

And here are 2 images with `width="200px"` in a table. The first has `align="right"` and the second has `align="left"`:

|                                                                   |                                                                  |
| :---------------------------------------------------------------: | :--------------------------------------------------------------: |
| <img src="./graphic-design-tips.jpg" width="200px" align="right"> | <img src="./graphic-design-tips.jpg" width="200px" align="left"> |

It appears if you want to get 2 or more images/graphics on a row, you need to put them in table cells or nest them in `<span>` tags. Note that the actual href values are to my website but they are linking to github and are links that open in a new page. Here is the image with a `title`, and a `<div>` tag with `align="center"` though you could use `align="right"` as well:

<div align="center"><img src="./graphic-design-tips.jpg" width="200px" title="Image example"></div>

<br>

**`dl`, `dt`, and `dd`** example (use for indentation):

<dl>
  <dt>Markdown Cheat Sheet</dt>
  <dd>A quick source for making your readme files look great!</dd>
</dl>

```markdown
<dl>
  <dt>Markdown Cheat Sheet</dt>
  <dd>A quick source for making your readme files look great!</dd>
</dl>
```

Pertaining to spacers in between sections, I am experimenting with 8-16px high PNG files with a gradient. I have one of those in my _Beginner Git Commands_ repo. I want to make one with the gradient colors used for dark and light mode here on GitHub.

Also, let's look at the small font-size for H5 and H6 tags (Markdown version). Regular paragraph size in markdown equals the font-size for `h4` or `###`. Where/when would using these be useful? H6 or 6 hashes is slightly larger than the footnote text at the bottom.

#### How about H4 as a comparison

##### Really small H5 heading

###### Even smaller text for an H6

Here is code to copy instead of having to type it out each time:

```
<h3 align="center">Heading3</h3>

<p align="right">Paragraph</p>

<img src="link.png" width="200px" title="title" align"center" alt="whatever">

<div align="center"><img src="link.png" width="200px" title="Image example"></div>
```

I will be adding notes here on how to add videos to markdown files on GitHub. Here is some examples that I got from [bobbyhadz.com](https://bobbyhadz.com/blog/embed-video-into-github-readme-markdown). I haven't added a link to a valid thumbnail but the video links to the 10:00 minute _Buck Bunny video_ and it opens in a new tab:

[![Watch the video](./markdown-image.png)](https://player.vimeo.com/external/194837908.sd.mp4?s=c350076905b78c67f74d7ee39fdb4fef01d12420&profile_id=164)

[<img src="./markdown-image.png" width="600" height="300"
/>](https://player.vimeo.com/external/194837908.sd.mp4?s=c350076905b78c67f74d7ee39fdb4fef01d12420&profile_id=164)

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

#### CSS Styles

If all of the above is not enough to differentiate your markdown files from a plain vanilla MD file, then you can also add CSS. You can not add a style sheet but you can add HTML as seen above. Which means you can add a `<style>` tag or add inline CSS.

Here is an example of a style tag:

```html
<style>
  .red {
    color: red;
    font-weight: 700;
    font-size: 1.5rem;
  }
  .flex {
    display: flex;
    justify-content: space-between;
  }
  .flex-child {
    background-color: #777;
    padding: 0.5em 1em;
    margin: 0.75em auto;
  }
</style>

<div class="red">Markdown css styles</div>

<div class="flex">
  <p class="flex-child">Box 1</p>
  <p class="flex-child">Box 2</p>
  <p class="flex-child">Box 3</p>
</div>
```

<style>
.red {
    color: red;
    font-weight:700;
    font-size: 1.5rem;
}
.flex {
  display: flex;
  justify-content: space-between;
}
.flex-child {
  background-color: #777;
  padding: 0.5em 1em;
  margin: 0.75em auto;
}
</style>

<div class="red">
    Markdown css styles
</div>

<div class="flex">
<p class="flex-child">
    Box 1
</p>
<p class="flex-child">
    Box 2
</p>
<p class="flex-child">
    Box 3
</p>
</div>

> _**BAD NEWS**: You can not use a `<style>` tag on GitHub, however the above works in VS Code on in the browser using the extension Markdown Preview Plus. That means it should work in other scenarios or platforms._

I could try and add the CSS as inline CSS for the div and paragraph tags, but I'm not that interested in spending time on that. I want my markdown files to look good and to have visual separation but I'd rather spend my time writing actual CSS for my projects. However, if you have a client that wants more CSS then you can experiment with inline CSS.

## Buttons

```markdown
<kbd>cmd + shift + p</kbd>
```

<kbd>cmd + shift + p</kbd>

Button with padding:

```markdown
<kbd> <br> cmd + shift + p <br> </kbd>
```

<kbd> <br> cmd + shift + p <br> </kbd>

Button as a link:

```markdown
<kbd>[Markdown-Cheatsheet](https://github.com/Kernix13/markdown-cheatsheet)</kbd>
```

<kbd>[Markdown-Cheatsheet](https://github.com/Kernix13/markdown-cheatsheet)</kbd>

Button as a link with padding:

```markdown
<kbd> <br> [Markdown-Cheatsheet](https://github.com/lifeparticle/Markdown-Cheatsheet) <br> </kbd>
```

<kbd> <br> [Markdown-Cheatsheet](https://github.com/lifeparticle/Markdown-Cheatsheet) <br> </kbd>

Button as a link without underlin:

```markdown
[<kbd>Markdown-Cheatsheet</kbd>](https://github.com/Kernix13/markdown-cheatsheet)
```

[<kbd>Markdown-Cheatsheet</kbd>](https://github.com/Kernix13/markdown-cheatsheet)

## Resources

1. [Daring Fireball](https://daringfireball.net/projects/markdown/basics 'Detailed markdown syntax') - more markdown documentation
1. [Complete list of github markdown emojis](https://dev.to/nikolab/complete-list-of-github-markdown-emoji-markup-5aia) - Emojis list
1. [GitHub emoji list](https://gist.github.com/rxaviers/7360908) - Emojis list
1. [Emoji Cheat Sheet](https://github.com/ikatyang/emoji-cheat-sheet) - Excellent!
1. [Emoji list](https://github.com/caiyongji/emoji-list) - there are a lot here as well
1. [HTML Entities](https://www.toptal.com/designers/htmlarrows/symbols/) - Excellent!
1. [HTML Entities2](http://mcdlr.com/8/) - maybe only a few unique vs the above link
1. [Shields.io](https://shields.io/) - Shields for your projects
1. [Devicons on Github](https://github.com/devicons/devicon/tree/master/icons): scan the list for icons you want to use.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

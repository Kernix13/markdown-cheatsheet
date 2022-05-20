# MARKDOWN CHEAT SHEET

Use this markdown cheat cheat as a guide for writing your markdown files. If you like it then clone or fork it, or at least click the **star** button. You can also check out the [Markdown Cheat Sheet article](https://kernixwebdesign.com/website/code/markdown-cheat-sheet-beginners/) I wrote, though it is not as inclusive as this guide.

I'm breaking up all the markdown syntax into 8 categories:

1. Basics
1. Styles
1. Miscellaneous
1. Links
1. Lists
1. Code
1. Hidden
1. Visual

**NOTE**: To view markdown> in VS Code hit <kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+`V` or click the preview button at top right in line with the file name tabs.

<div id="back-to-top"></div>

## ~~A Literal~~ <ins>Table</ins> of _Contents_

|                             Category | Element                                                             | Accepts styles? |
| -----------------------------------: | :------------------------------------------------------------------ | :-------------: |
|               **[Basics](#basics)**: | [Paragraphs](#paragraphs)                                           |     **Yes**     |
|                                      | [Special characters](#special-characters)                           |      `N/A`      |
|               **[Styles](#styles)**: | [Bold](#bold)                                                       |      `N/A`      |
|                                      | [Italic](#italic)                                                   |      `N/A`      |
|                                      | [Strike thru](#strike-thru)                                         |      `N/A`      |
|                                      | [Underline](#underline)                                             |      `N/A`      |
| **[Miscellaneous](#miscellaneous)**: | [Headings](#headings)                                               |     **Yes**     |
|                                      | [Blockquotes](#blockquotes)                                         |     **Yes**     |
|                                      | [Descriptions](#descriptions)                                       |    **Yes\***    |
|                                      | [Tables](#tables)                                                   |     **Yes**     |
|                                      | [Horizontal rules](#horizontal-rules)                               |       No        |
|                 **[Links](#links)**: | [External](#external)                                               |     **Yes**     |
|                                      | [Anchor](#anchor)                                                   |     **Yes**     |
|                                      | [Footnotes](#footnotes)                                             |     **Yes**     |
|                                      | [At mentions](#at-mentions)                                         |      `N/A`      |
|                 **[Lists](#lists)**: | [Unordered](#unordered)                                             |     **Yes**     |
|                                      | [Ordered](#ordered)                                                 |     **Yes**     |
|                                      | [Nested](#nested)                                                   |     **Yes**     |
|                                      | [Tasks](#tasks)                                                     |       No        |
|                   **[Code](#code)**: | [Inline](#inline)                                                   |    **Yes\***    |
|                                      | [Tab](#tab)                                                         |       No        |
|                                      | [Generic](#generic)                                                 |       No        |
|                                      | [Language block](#language-block)                                   |       No        |
|                                      | [Diff](#diff)                                                       |       No        |
|                                      | [Math](#math)                                                       |       No        |
|               **[Hidden](#hidden)**: | [Comments](#comments)                                               |       No        |
|                                      | [Spoiler](#spoiler)                                                 |     **Yes**     |
|                                      | [Details](#details)                                                 |       No        |
|               **[Visual](#visual)**: | [Images](#images)                                                   |       No        |
|                                      | [Emojis](#emojis)                                                   |       No        |
|                                      | [HTML entities](#html-entities)                                     |    **Yes\***    |
|                  **[Notes](#notes)** | [Block level HTML tags that work](#block-level-HTML-tags-that-work) |        -        |
|                                      | [Inline HTML tags that work](#inline-HTML-tags-that-work)           |        -        |
|                                      | [HTML tag examples](#html-tag-examples)                             |        -        |
|          **[Resources](#resources)** | N/A                                                                 |        -        |

<!-- ~~`<cite>`~~ -->

---

## Basics

This is a short section on basic paragraphs, the symbols used in Markdown and how to escape them, and @mentions.

### Paragraphs

Since paragraphs are a thing of their own, let's cover that one first:

**Paragaphs**: Just use regular text but make sure to hit the <kbd>ENTER</kbd> key twice. Sometimes if you only hit <kbd>ENTER</kbd> once, the text will de displayed as the element directly above it or there will not be a line break.

### Special characters

Here are the characters you will use in Markdown. They will be covered in each section after this one:

````
# Hast tags for headines and anchor links
@ for at mentions
[] for links, checked lists / tasks, and footnotes
() for links
! for images
^ for footnote links
x or X for tasks lists
` and ``` for inline code and codeblocks
* and ** for italic an bold
_ underscore for italics
~~ for strikethrough
| for tables
: with dashes - for table cell alignments, for footnotes, and emojis
|| double pipes for spoiler text on Discord
- and a space for unordered lists
1, 2, 3, etc. for numbered lists
- and + for diff code blocks
> for blockquotes
3 - or * for horizontal rules
" for titles to links
<!-- for comments -->
\ to escape most of the characters above

\* escape asterisk,
\| escape pipe, etc...
````

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Styles

This category deals with the styling of individual words and can be used with every category with a few exceptions. You may not have thought of it but you can apply these effects to all or some of the words in:

- Headings
- Links
- Lists (Not Tasks)
- Blockquotes
- Table cell values
- HTML entities (except strikethrough)
- Hidden (Spoiler only)

These do not work for the obvious ones (Horizontal Rules, Images, and Emojis), and for all elements in the Code category except inline code.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Bold

**Bold**: use either 2 **asterisks** or 2 **underscores** before and after the text for bold styling. The preferred syntax is to use asterisks for bold:

    **two asterisks**
    __two underscores__

### Italic

**Italic**: use a _single asterisk_ or _underscore_ before and after the text for italic styling. The preferred syntax is to use an underscore for italic:

    *single asterisk*
    _single underscore_

**_Bold and Italic_**: use either **_3 asterisks_** or **_2 asterisks and 1 underscore_** for bold and italic text. The preffered syntax is the latter:

    ***3 asterisks***
    **_2 asterisks and and 1 underscore_**

### Strike thru

**Strikethrough**: use two tildes (~~) before and after text that you want to display as ~~strikethrough~~:

    ~~double tildes~~

If you want, you can also do **~~bold strikethrough~~**, _~~\_italic strikethrough_~~, and \*\*\*~~bold italic strikethrough~~\*\*\*.

### Underline

This can only be done with the `<ins>` HTML tag. This is **_NOT_** part of Markdown.

The links on GitHub are blue, bold and underlined (<ins>on hover</ins>). The `<ins>` HTML tag underlines text and has normal font color and normal font-weight. No one familiar with GitHub will confuse it for a link. It's another styling effect that I find more useful than srikethrough.

This is <ins>text underlined</ins> with the `ins` HTML tag.

```
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

All elements in this category accept text effects except for horizontal rule, and with an exception for descriptions.

### Headings

There are 6 headings just like in HTML. Use a single hashtag for H1 and 6 hashtags for H6. The top title of this docuement is an H1 with a single hash, this section (**Misc**) uses 2 hashtags, and this sub-section (**Headings**) uses 3 hashtags.

**NOTE**: There is an automatic horizontal rule added when you use syntax for H1 and H2.

    # MARKDOWN CHEAT SHEET (Heading 1)
    ## Misc (Heading 2)
    ### Headings (heading 3)
    ### Heading 4 (you most likely will not use H5 or H6)

Here is an example of using Bold, Italic, and Strikethrough in a heading:

    ## ~~A Literal~~ <ins>Table</ins> of _Contents_

As you can see, strikethrough and italic worked on the heading, but using bold did not increase the font weight for the word `Table`.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Blockquotes

This is a nice effect but I don't know why you would use it on GitHub:

> Use a **greater** than _sign_ (>) to quote a team member
>
> Create a <ins>space</ins> like above using > with no text (~~ignore~~)

    > Use a **greater** than _sign_ (>) to quote a team member
    >
    > Create a <ins>space</ins> like above using > with no text (~~ignore~~)

<br />

### Descriptions

The following are HTML tags, **_NOT_** a part of markdown. But they do give you a nice indentation for visual variety.

The text in the tags can only be styled with the HTML tags related to bold, italic, strikethrough, or _underline_. As you can see, I used the `ins`, `b`, `em`, and `s` tags in the example below:

- `dl`: description list, the wrapper element for the other two
- `dt`: description term, that which you are defining or highlighting
- `dd`: description details, the actual definition or explanantion

<dl>
  <dt>Description <ins>List</ins></dt>
  <dd>Represents a description list. The <ins><b><em>dl</em></b></ins> element encloses a list of groups of terms (specified using the <ins><b><em>dt</em></b></ins> element) and descriptions (provided by <ins><b><em>dd</em></b></ins> elements). Common uses for this element are to implement a glossary or to display metadata (a list of key-value pairs) (<s>ignore</s>).</dd>
</dl>

```
<dl>
  <dt>Description <ins>List</ins></dt>
  <dd>Represents a description list. The <ins><b><em>dl</em></b></ins> element encloses a list of groups of terms (specified using the <ins><b><em>dt</em></b></ins> element) and descriptions (provided by <ins><b><em>dd</em></b></ins> elements). Common uses for this element are to implement a glossary or to display metadata (a list of key-value pairs) (<s>ignore</s>).</dd>
</dl>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

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

```
| Left aligned Content | Center aligned Content | Right aligned Content |
| :-----------         | :-----------:          | -----------: |
| Content Left         | Content Center         | Content Right |
| Content Left         | Content Center         | Content Right |
| *Italic*             | **Bold**               | ~~Strikethrough~~ |
| <ins>Underlined</ins> | Content Center        | Content Right |
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Horizontal rules

Use 3 asterisks or 3 dashes with or without a space to create a horizontal rule:

---

    - - -
    ---
    * * *
    ***

**NOTE**: Make sure to hit <kbd>ENTER</kbd> twice if you intend to use 3 asterisks witout spaces or it will set the text above it to an H3 tag.

<hr>

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Links

This category accepts all text effects and includes:

- External links
- Anchor links (same page)
- Footnote links

### External

**External Links**: The syntax is to use square brackets around the link text and parentheses for the URL. You can also add an additional title for the link by adding a space after the URL and adding the link title in double quotes:

Here is a link to my [Beginner Git Commands](https://github.com/Kernix13/beginner-git-commands) repositiory. And here is the syntax:

    [Link text](URL "Optional link title")

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

    [Strike thru](#strike-thru)

Here is the code for the anchor link using an HTML `<a>` tag:

    <a id="back-to-top"></a>

Here is the matching link for the above:

    [Back to Top](#back-to-top)

I actually changed my 'Back to Top' link to be an `<a>` link inside of a `<div>` so that I could align the link to the right and use an HTML entity for an arrow up:

```
<div id="back-to-top"></div>
<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Footnotes

**Footnote links**: I assume footnotes would be useful in a very technical or long README file. Use square brackets where you want a footnote link to appear and use a caret symbol (^) followed by the number of the footnote.

Then below that add the same syntax followed by a colon and the note itself - none of that will display on the page. That will make the footnote text appear at the bottom of your file:

Footnote.[^1]

Some other important footnote.[^2]

Use this for where you want the link:

```
[^1]
```

Here is the actual footnote syntax:

    [^1]: This is footnote number one.
    [^2]: Here is the second footnote.

[^1]: This is footnote number one.
[^2]: Here is the second footnote.

### At mentions

At mentions do not seem to work as links. This is an at mention test:

@Kernix13: Hello. This does not work in a markdown file, but it does create a link in Issues and PRs, and maybe in other areas as well.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Lists

This category has:

- Unordered lists
- Ordered lists
- Nested lists
- Task lists

You can use all text effects but with some exceptions: None of the effects work for Task lists, and you don't seem to be able to use VS Code shortcuts (<kbd>SHIFT+_</kbd>, etc) - you have to manually type `_`, `\_`or`~`.

### Unordered

**Unordered lists**: You can use either an asterisk or a dash followed by a space to make a bulleted list. I prefer using a dash since you do not need to use the <kbd>SHIFT</kbd> key:

- list item 1
- list item 2

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Ordered

**Ordered lists**: use a number followed by a period (1., 2., 3. etc.) and then a space to create an ordered list:

1. Ordered **item** 1
1. Ordered _item_ 2
1. Ordered ~~item 3~~

```
1. Ordered item 1
1. Ordered item 2
1. Ordered item 3
```

**NOTE**: By using "1" for each list item, you can cut & paste to change the order of items and the numbering will change to match the new order.

Does this make sense? You can use both unordered and ordered together -> bullets with roamn numerals, or numbers with bullets:

1. - What?
1. - Really?
1. - Why?

- 10. What is this
- 15. Again?
- 50. Any use cases?

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Nested

**Nested list**: Use the <kbd>SPACEBAR</kbd> key to align the dash or asterisk directly beneath the first character in the parent list item to create a nested list:

- list item 1
- list item 2
  - child item 1
  - child item 2
- list item 3

```
- list item 1
- list item 2
  - child item 1
  - child item 2
- list item 3
```

For a nested ordered list, do the same as for nested unordered lists - align the number to be below the first character of the parent item:

1. Ordered item 1
1. Ordered item 2
   1. Child item 1
   1. Child item 2
1. Ordered item 3

```
1. Ordered item 1
1. Ordered item 2
   1. Child item 1
   1. Child item 2
1. Ordered item 3
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Tasks

You can create what looks like checkboxes and display completed tasks with a checkmark. It takes the form of an unordered list with the first characters being a set of square brackets which **_MUST_** have a space in them. For a completed task, add either a lower or uppercase "X":

- [ ] incomplete task
- [x] completed task
  - [ ] incomplete subtask
  - [x] complete subtask

```
- [ ] incomplete task
- [x] completed task
  - [ ] incomplete subtask
  - [x] completed subtask
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Code

This category deals with inline code and various typs of code blocks and none of them accept Styles with the exception of `inline` and 'math expressions`:

- Inline code
- Code blocks
- <kbd>TAB</kbd> code blocks
- Code highlighting blocks
- `Diff` code blocks
- Math Expressions

### Inline

Use a `single backtick` before and after text to display it as inline code:

    `single backtick`

Here are examples on inline as **`bold`**, _`italic`_, and ~~`strikethrough`~~.

### Tab

It took me a while how to show the 3 backticks for a code block (next section). For that and other tricky markdown that will not dispay, hit the <kbd>TAB</kbd> button twice then enter your code:

    This is a code block made by hitting TAB 2 X's

### Generic

To add code that requires more than 1 line then use 3 backticks, hit <kbd>ENTER</kbd>, add your code block, hit <kbd>ENTER</kbd> again and add 3 more back ticks.

    ```
    *, *::before, *::after {
            box-sizing: border-box;
        }
    ```

```
a {
  text-decoration: none;
}
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Language block

This is what you want to use for code blocks. To highlight parts of your code add the language after the opening triple backticks. You'll have to do your own research but so far the following language bbreviations work: `md`, `html`, `css`, `js` or `javascript`, `jsx`, `php`, `xml`, `python`, `sql`, and `apacheconf` (for Apache servers). I tried using `node` and `npm` for my node-npm repo but it had no effect.

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

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Diff

This is really nice for highlighting text or code that was changed. Use `diff` after the opening triple backticks. Then use a minus sign (-) for what was changed, and a plus symbol (+) for the new version:

```diff
- this code or text is the old version
+ this is what it was changed to
```

    ```diff
    - this code or text is the old version
    + this is what it was changed to
    ```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Math

Finally, per GitHub:

> ...math expressions can be rendered in Markdown on GitHub using $$ as a delimiter for code blocks with math content or the $ delimiter for inline math expressions.

1. Use a single dollar sign (`$`) at the beginning and end of an inline math expression.
2. Use 2 dollar sign (`$$`) at the beginning and end for a block of math expressions.

Inline example: this `$(ax^2 + bx + c = 0)$` renders as $(ax^2 + bx + c = 0)$.

Inline exception: use `\$` to escape, and therefore use, a dollar sign in an equation.

Inline exception 2: use `<span>$</span>` for inline use of dollar sign before a math expression.

Block example: `$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$` renders as:

$$ x = {-b \pm \sqrt{b^2-4ac} \over 2a} $$

Block example 2: This `$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$` renders as:

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

Here are the important symbols to know:

- ^ = exponent, e.g. $a^3$
- { } = required for certain expressions such as square root
- \pm = plus\minus symbol: $\pm$
- \sqrt = square root symbol: $\sqrt{b}$
- \over = division: $a \over b$
- \leq = less than or equal to: $\leq$
- \geq = greater than or equal to: $\geq$
- \ne = not equal to: $ \ne $
- \sum = Sigma, summation symbol: $\sum$
- \_val = sub-script value: $a_i$
- \_{val=num}^n = start val and max (n) val for sum
- \left = not sure, see summation above
- \right = not sure, see summation above

For some reason the symbols are not showing...

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

---

## Hidden

This is an odd category with 3 effects, one of which you have probably only seen on Discord:

- Comments
- Spoiler text
- Details

Only Spoiler text accepts text effects.

### Comments

This is a nice way to add a comment in the editor view of your markdown file. This would be good for teams members editing a documentation page. The best way is to use HTML syntax:

<!-- There is a comment here that you can't see -->

    <!-- There is a comment here that you can't see -->

### Spoiler

On Discord you may sometimes see a black rectangle that reveals text or code when you click on it. Use double pipes before and after the word(s)/code that you want to conceal:

    ||Spoiler text|| in Discord

**NOTE**: This does not work on Slack or here on GitHub.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Details

This isn't a markdown thing but it is another example of using HTML tags in a Markdown file. It has the same effect as an accordian. I'm not sure why you would use this but here is how you would do it:

<details>
  <summary>Title 1</summary>
  <p>Some hidden content goes here</p>
  Here is some more without a paragraph tag
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

## Visual

The three sections below deal with adding visual elements to your markdowb file: `images`, `emojis`, and `HTML entities`.

### Images

Images use the same syntax as **Links** except for the addition of an exclamation mark immediately before the opening square bracket. You can also use the optional title text:

![picture alt text](https://via.placeholder.com/150 "Title is optional")

    ![picture alt](https://via.placeholder.com/150 'Title is optional')

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Emojis

I'm not a huge fan of emojis, but here are some that I would consider using. The syntax is the emoji code in between colons:

    :Emoji_code:

Approval: :+1:, :smile:, :ok_hand:, :white_check_mark:, :heavy_check_mark:, :star:, :star2:, :heart:, :exclamation:

    :+1:, :smile:, :ok_hand:, :white_check_mark:, :heavy_check_mark:,
    :star:, :star2:, :heart:, :exclamation:

Disapproval, questions, problems: :-1:, :question:, :grey_question:, :x:, :boom:, :bomb:, :astonished:, :warning:, :interrobang:

    :-1:, :question:, :grey_question:, :x:, :boom:, :bomb:, :astonished:,
    :warning:, :interrobang:

Directional: :point_right:, :point_left:, :arrow_left:, :arrow_right:, :arrow_up:, :arrow_down:

    :point_right:, :point_left:, :arrow_left:, :arrow_right:, :arrow_up:, :arrow_down:

Time, alarms: :bell:, :no_bell:, :hourglass:, :alarm_clock:, :watch:, :calendar:

    :bell:, :no_bell:, :hourglass:, :alarm_clock:, :watch:, :calendar:

Weather: :sunny:, :cloud:, :snowflake:, :zap:, :high_brightness:

    :sunny:, :cloud:, :snowflake:, :zap:, :high_brightness:

Office/Business: :scissors:, :pushpin:, :paperclip:, :phone:, :copyright:, :email:

    :scissors:, :pushpin:, :paperclip:, :phone:, :copyright:, :email:

Miscellaneous/playful: :alien:, :green_heart:, :blue_heart:, :purple_heart:, :mushroom:, :pizza:, :beer:, :icecream:, :sound:, :speaker:, :lock:, :guitar:, :one:, :two: (and other #'s), <br>
:link:, :speech_balloon:, :mag:, :mag_right:, :key:, :bulb:

```emoji
:alien:, :green_heart:, :blue_heart:, :purple_heart:, :mushroom:, :pizza:, :beer:,
:icecream:, :sound:, :speaker:, :lock:, :guitar:, :one:, :two: (and other #'s),
:link:, :speech_balloon:, :mag:, :mag_right:, :key:, :bulb:
```

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

## Notes

The one thing I want to look into is using videos, animated GIFs, more HTML tags in my markdown files, and also column layouts using tables.

I used a GitHub generator for my Profile README. In there are `<p>`, `<a>`, and `<img>` tags. In the Details section above, there are `<details>`, `<summary>`, and `<p>` tags. I found this gist called <q>[HTML Tags You Can Use on GitHub](https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2)</q>. That document mentions some tags you can use.

I tested every HTML tag that made sense. I skipped tags like `section`, `header`, `nav`, etc. Here is a breakdown of that testing.

### Block level HTML tags that work

_Duplicates markdown_: `blockquote`, `h1` thru `h6`, `hr`, `ol` `ul` `li`, `pre`, `table`

_No markdown equivalent_: `details` with `summary`, `dl` `dt` `dd` (indent), `div`, `fieldset` with or without `legend`.

> Is **align** an attribute? How do I find similar attributes like that?

**Attributes**:

- `blockquote`: global
- `h1` thru `h4`: global, align (center, right)
- `h5` and `h6`: Same as above, very small font size!
- `ol`, `ul`: global
- `li`: global
- `pre`: global
- `table`: global
- `details`, `summary`: global
- `dl`, `dt`, `dd`: global
- `div`: global, align (left, center, right)
- `p`: global, align (left, center, right)

Unless there is a way to display the tags differently, then I do not see the point of using `pre`, `table`, `lists`, or `blockquote`. Especially the `table` tag since there are a lot of tags you need to enter.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Inline HTML tags that work

_Duplicates markdown_: `a`, `b` and `strong` (display as Bold), `code`, `del` and `s` (display as Strikethrough), `em` and `i` and `var` (display as Italic), `img` (width, align [center, right])

_No markdown equivalent_: `br` (line break), `ins` (underline), `sup` and `sub` (superscript and subscript), `samp` (Monospaced font), `q` (quotes), `kbd` (keyboard keys), `span`

**Attributes**:

- `a`: target="\_blank" did not work
- `b`, `strong`: global
- `br`: global
- `code`: global
- `del`, `s`: na, global
- `em`, `i`, `var`: global
- `img`: align, width
- `ins`: na
- `kbd`: global
- `q`: global
- `samp`: global
- `span`: global
- `sub`, `sup`: global

Some _Global attributes_ that may have a use: id, draggable, **style**, **title**, tabindex, contenteditable, autofocus.

> What is **_align_**? Do all these accept inline CSS?

The only tags worth using IMO:

- `a` for anchor links with HTML entities in the link text, `target="_blank"` doesn't work
- `headings` align center or right
- `p` for align center or right
- `div` as visual dividers using dash (-) or underscore (\_) or equals (=) or other characters. But can't you just use the characters instead?
- `br` for line breaks of paragrpah text or as a alternate spacer to `div`
- `img` to set width and height and align of center or right
- `ins` for underline
- `kbd` for keyboard keys
- `samp` for monospaced font as a styling choice
- `sup` and `sub` for superscript and subscript
- `dl` `dt` `dd` maybe for the indentation of the definition

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

<br><br>

#### HTML tag examples

The large gap above the title is from 2 `<br>` tags. Use only one for a normal separation.

| HTML Tag |                     Result                     |
| :------- | :--------------------------------------------: |
| `ins`    |           <ins>underlined text</ins>           |
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

|                                                                                                                        |                                                                                                                       |
| :--------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------: |
| <img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg" width="200px" align="right"> | <img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg" width="200px" align="left"> |

I don't know of another method to get images on a row other than using a table. Note that the actual href values are to my website but they are linking to github and are links that pen in a new page (???)Here is the image with a `title`, and a `<div>` tag with `align="center"` though you could use `align="right"` as well:

<div align="center"><img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg" width="200px" title="Image example"></div>

<br>

**`dl`, `dt`, and `dd`** example (use for indentation):

<dl>
  <dt>Markdown Cheat Sheet</dt>
  <dd>A quick source for making your readme files look great!</dd>
</dl>

```
<dl>
  <dt>Markdown Cheat Sheet</dt>
  <dd>A quick source for making your readme files look great!</dd>
</dl>
```

Pertaining to spacers in between sections, I am experimenting with 8-16px high PNG files with a gradient. I have one of those in my _Beginner Git Commands_ repo. I want to make one with the gradient colors used for dark and light mode here on GitHub.

Also, let's look at the small font-size for H5 and H6 tags (Markdown version). Where/when would using these be useful?

#### How about H4 as a comparison

##### Really small H5 heading

###### Even smaller text for an H6

Finally, here is code to copy instead of having to type it out each time:

```
<h3 align="center">Heading3</h3>

<p align="right">Paragraph</p>

<img src="link.png" width="200px" title="title" align"center" alt="whatever">

<div align="center"><img src="link.png" width="200px" title="Image example"></div>
```

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Resources

1. [Daring Fireball](https://daringfireball.net/projects/markdown/basics "Detailed markdown syntax") - more markdown documentation
1. [Complete list of github markdown emojis](https://dev.to/nikolab/complete-list-of-github-markdown-emoji-markup-5aia) - Emojis list
1. [GitHub emoji list](https://gist.github.com/rxaviers/7360908) - Emojis list
1. [Emoji Cheat Sheet](https://github.com/ikatyang/emoji-cheat-sheet) - Excellent!
1. [Emoji list](https://github.com/caiyongji/emoji-list) - there are a lot here as well
1. [HTML Entities](https://www.toptal.com/designers/htmlarrows/symbols/) - Excellent!
1. [HTML Entities2](http://mcdlr.com/8/) - maybe only a few unique vs the above link
1. [Shields.io](https://shields.io/) - Shields for your projects

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

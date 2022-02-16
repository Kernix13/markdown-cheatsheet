# MARKDOWN CHEAT SHEET

Use this markdown cheat cheat as a guide for writing your markdown files. If you like it then clone or fork it, or at least click the **star** button. You can also check out the [Markdown Cheat Sheet article](https://kernixwebdesign.com/website/code/markdown-cheat-sheet-beginners/) I wrote, though it is not as inclusive as this guide.

I'm breaking up all the markdown syntax into 6 categories:

1. Text effects
1. Links
1. Lists
1. Code 
1. Hidden
1. Unique

I'll explain what those mean in each section. But the point is that the first one (Text Effects) can be applied to all or some of the elements in each category with the exception of the Code category. That will make sense when you read each category descripion and notes.

**NOTE**: To view markdown in VS Code hit CTRL+SHIFT+V or click the preview button at top right in line with the file name tabs.

<a id="back-to-top"></a>

## Table of contents
1. [Text effects](#text-effects)
   1. [Bold text](#bold-text)
   1. [Italic text](#italic-text)
   1. [Strikethrough text](#strikethrough-text)
1. [Links](#links)
   1. [External links](#external-links)
   1. [Anchor links](#anchor-links)
   1. [Footnote links](#footnote-links)
1. [Lists](#lists)
   1. [Unordered lists](#unordered-lists)
   1. [Ordered lists](#ordered-lists)
   1. [Nested lists](#nested-lists)
   1. [Task lists](#task-lists)
1. [Code](#code)
   1. [Inline code](#inline-code)
   1. [Code blocks](#code-blocks)
   1. [Tab code blocks](#tab-code-blocks)
   1. [Code highlighting blocks](#code-highlighting-blocks)
   1. [Diff code blocks](#diff-code-blocks)
1. [Hidden](#hidden)
   1. [Comments](#comments)
   1. [Discord hidden text](#discord-hidden-text)
   1. [Hidden content](#hidden-content)
1. [Unique](#unique)
   1. [Headings and paragraphs](#headings-and-paragraphs)
   1. [Blockquotes](#blockquotes)
   1. [Tables](#tables)
   1. [Horizontal rules](#horizontal-rules)
   1. [Images](#images)
   1. [Emojis](#emojis)
   1. [HTML entities](#html-entities)
1. [Notes](#notes)
1. [Other markdown resources](#other-markdown-resources)

- - - 

## Text effects

This category deals with the styling of individual words and can be used with every category except the Code category.

You can apply these effects to all or some of the words in:

- Headings
- Blockquotes
- Table cell values
- HTML entities (except strikethrough)

These do not work for the obvious ones (Horizontal Rules, Images, and Emojis), and for all elements in the Code category.

### Bold text

**Bold**: use either 2 **asterisks** or 2 __underscores__ before and after the text for bold styling. The preferred syntax is to use asterisks for bold:

    **two asterisks**
    __two underscores__

###  Italic text

**Italic**: use a *single asterisk* or _underscore_ before and after the text for italic styling. The preferred syntax is to use an underscore for italic:

    *single asterisk*
    _single underscore_

**_Bold and Italic_**: use either 3 asterisks or 2 asterisks and 1 underscore for bold and italic text. The preffered syntax is the latter:

    ***3 asterisks***
    **_2 asterisks and and 1 underscore_**

### Strikethrough text

**Strikethrough**: use two tildes (~~) before and after text that you want to display as ~~strikethrough~~:

    ~~double tildes~~

If you wanted to you could also do **~~bold strikethrough~~**, _~~_italic strikethrough_~~, and ***~~bold italic strikethrough~~***.

[Back to Top](#back-to-top "Table of contents")

- - - 

## Links

This category accepts all text effects and includes:

- External links
- Anchor links (same page)
- Footnote links

### External links

**External Links**: The syntax is to use square brackets around the link text and parentheses for the URL. You can also add an additional title for the link by adding a space after the URL and adding the link title in double quotes:

Here is a link to my [Beginner Git Commands](https://github.com/Kernix13/beginner-git-commands) repositiory. And here is the syntax:

    [Link text](URL "Optional link title")

**NOTE**: Only use a title if it adds information. Don't set the title text to be the same as the link text.

[Back to Top](#back-to-top "Table of contents")

### Anchor links

**Same page anchor links**: This can be done in at least two different ways. For all the links in the table of contents I use the simpler method. But for the **Back to Top** link I use an actual `<a>` tag.

For the simple links use the same syntax as for Links above with 2 exceptions for the URL part:

- precede the URL with a hashtag
- use the exact same text as where you are linking to with
  - But all the text needs to be in lowercase
  - all words need to be connected with a dash (no spaces)  

Here is an example for this section:

    [Intermediate markdown](#intermediate-markdown)

Here is the code for the anchor link using an HTML `<a>` tag:

    <a id="back-to-top"></a>

Here is the matching link for the above:

    [Back to Top](#back-to-top)

[Back to Top](#back-to-top "Table of contents")

### Footnote links

**Footnote links**: I assume footnotes would be useful in a very technical or long README file. Use square brackets where you want a footnote link to appear and use a caret symbol (^) followed by the number of the footnote. Then below that area add the same syntax followed by a colon and the note itself. That will make the footnote text appear at the bottom of your file: 

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

[Back to Top](#back-to-top "Table of contents")

- - - 

## Lists

This category has:

- Unordered lists
- Ordered lists
- Nested lists
- Task lists

You can use all text effects but with some exceptions: None of the effects work for Task lists, and you don't seem to be able to use VS Code shortcuts - you have to manually type *, _ or ~. 

### Unordered lists

**Unordered lists**: You can use either an asterisk or a dash followed by a space to make a bulleted list. I prefer using a dash since you do not need to use the *SHIFT* key:

- list item 1
- list item 2

[Back to Top](#back-to-top "Table of contents")

### Ordered lists

**Ordered lists**: use a number followed by  a period (1., 2., 3. etc.) to create an ordered list. :

1. Ordered item 1
1. Ordered item 2
1. Ordered item 3

```
1. Ordered item 1
1. Ordered item 2
1. Ordered item 3
```
**NOTE**: By using "1" for each list item, you can cut & paste to change the order of items and the numbering will change to match the new order. 

[Back to Top](#back-to-top "Table of contents")

### Nested lists

**Nested list**: Use the *SPACEBAR* key to align directly beneath the first character in the parent list item to create a nested list:

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

[Back to Top](#back-to-top "Table of contents")

### Task lists

You can create what looks like checkboxes and display completed tasks with a checkmark. It takes the form of an unordered list with the first characters being a set of square brackets which **_MUST_** have a space in them. For a completed task, add either a lower or uppercase "X":

- [ ] incomplete task
- [X] completed task
  - [ ] incomplete subtask
  - [x] complete subtask

```
- [ ] incomplete task
- [x] completed task
  - [ ] incomplete subtask
  - [x] completed subtask
```

[Back to Top](#back-to-top "Table of contents")

- - - 

## Code

This category deals with inline code and various typs of code blocks and none of them accept text effects:

- Inline code
- Code blocks
- Tab code blocks
- Code highlighting blocks
- Diff code blocks

### Inline code

Use a `single backtick` before and after text to display it as inline code:

    `single backtick`

### Code blocks

To add code that requires more than 1 line then use 3 backticks, hit *ENTER*, add your code block, hit *ENTER* again and add 3 more back ticks. 

    ```
    some code here
    ```

```
a {
  text-decoration: none;
}
```

[Back to Top](#back-to-top "Table of contents")

### Tab code blocks

It took me a hile how to show the 3 backticks for a code block. For that and other tricky markdown that will not dispay, hit the *TAB* button then enter your code

    This is a TAB code block, check with `backticks`

### Code highlighting blocks 

This is what you want to use. To highlight parts of your code add the language after the opening triple backticks. You'll have to do your own research but so far the following languages work: `md`, `html`, `css`, `js` or `javascript`, `php`, `xml`, `python`, `sql`, `apacheconf` (for Apache servers). I tried using `node` and `npm` for my node-npm repo but it had no effect.

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
[Back to Top](#back-to-top "Table of contents")

### Diff code blocks

This is really nice for highlighting text or code that was changed. Use `diff` after the opening triple backticks. Then use a minus sign (-) for what was changed, and a plus symbol (+) for the new version:

```diff
- this code or text is the old version
+ this is what it was changed to
```


    ```diff
    - this code or text is the old version
    + this is what it was changed to
    ```

[Back to Top](#back-to-top "Table of contents")

- - - 

## Hidden

This is an odd category with 3 effects, one of which you have probably only seen in discord:

- Comments
- Discord hidden text
- Hidden content

Only hidden text accepts text effects.

### Comments

This is a nice way to add a comment in the editor view of your markdown file. This would be good for teams members editing a documentation page for a new section. The best way is to use HTML syntax:

<!-- There is a comment here that you can't see -->

    <!-- There is a comment here that you can't see -->


### Discord hidden text

On Discord you may sometimes see a black rectangle that reveals text or code when you click on it. Use double pipes before and after the text/code that you want to conceal:

    ||Spoiler text|| in Discord

**NOTE**: This does not work on Slack or here on GitHub.

I'm adding on definitions because I saw it on a Markdown post but it doesn't work for me. Perhaps this only works in Discord as well. Let me know if you know how to use that:

    Definition: term : definition

[Back to Top](#back-to-top "Table of contents")

### Hidden content

This has the same effect as an accordian. I'm not sure why you would use this but here is how you would do it:

<details>
  <summary>Title 1</summary>
  <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
<details>
  <summary>Title 2</summary>
  <p>Content 2 Content 2 Content 2 Content 2 Content 2</p>
  <p>Content 2 Content 2 Content 2 Content 2 Content 2</p>
</details>

```
<details>
  <summary>Title 1</summary>
  <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
<details>
  <summary>Title 2</summary>
  <p>Content 2 Content 2 Content 2 Content 2 Content 2</p>
  <p>Content 2 Content 2 Content 2 Content 2 Content 2</p>
</details>
```

[Back to Top](#back-to-top "Table of contents")

- - - 

## Unique

The elements in this category are all unique and do not fit into any of the other categories:

- Headings
- Blockquotes
- Tables
- Horizontal rules
- Images
- Emojis
- HTML entities

All elements in this category accept text effects except for the obvious one: images, emojis and horizontal rules.

### Headings and paragraphs

There are 6 headings just like in HTML. Use a single hashtag for H1 and 6 hashtags for H6. The top title of this docuement is an H1 with a single hash, this section (Basic markdown) uses 2 hashtags, and this sub-section (Headings and paragraphs) uses 3 hashtags. 

**NOTE**: There is an automatic horizontal rule added when you use syntax for H1 and H2.

    # MARKDOWN CHEAT SHEET (Heading 1)
    ## Text effects (Heading 2)
    ### Headings and paragraphs (heading 3)
    ### Heading 4 (you most likely will not use H5 or H6) 

**Paragaphs**: Just use regular text but make sure to hit the *ENTER* key twice. Sometimes if you only hit ENTER once, the text will de displayed as the element directly above it.

[Back to Top](#back-to-top "Table of contents")

### Blockquotes

> Use a greater than sign (>) to quote a team member
> 
> Create a space like above using > with no text

    > use greater than sign (>) for a blockquote


### Tables

I only used this for the Pull Requests and Issues I opened on freeCodeCamp. That table is a list of common prefixes to include in your titles (See the Git commands link above). Here is a generic table. I will not explain all of this but pay attention to the syntax that is creating the column divisions and alignment:

| Left aligned | Center aligned | Right aligned |
| :----------- | :-----------: | -----------: |
| Content Left | Content Center | Content Right |
| Content Left | Content Center | Content Right |
| Content Left | Content Center | Content Right |
| Content Left | Content Center | Content Right |

```
| Left aligned | Center aligned | Right aligned |
| :----------- | :-----------: | -----------: |
| Content Left | Content Center | Content Right |
| Content Left | Content Center | Content Right |
| Content Left | Content Center | Content Right |
| Content Left | Content Center | Content Right |
```

[Back to Top](#back-to-top "Table of contents")

### Horizontal rules

Use 3 asterisks or dashes with or without a space to create a horizontal rule:

- - - 

    - - - 
    ---
    * * * 
    ***

**NOTE**: Make sure to hit _ENTER_ twice if you intend to use 3 asterisks witout spaces or it will set the text above it to an H3 tag.

[Back to Top](#back-to-top "Table of contents")

### Images

Images use the same syntax except for the addition of an exclamation mark immdiately before the opening square bracket. You can also use optional title text:

![picture alt text](https://via.placeholder.com/150 'Title is optional')

    ![picture alt](https://via.placeholder.com/150 'Title is optional')

[Back to Top](#back-to-top "Table of contents")

### Emojis

I'm not a huge fan of emojis, but here are some that I would consider using. The syntax is the emoji code inbetween colons:

    :Emoji_code:

`:+1:`,  `:smile:`, `:star:`, `:exclamation:`, `:question:`, `:thumbsdown:`, `:point_right:`, `:point_left:`, `:heart:`, `:sound:`, `:lock:`, `:email:`, `:guitar:`, `:one:`, `:two:` (and other #'s), `:arrow_left:`, `:arrow_right:`, `:arrow_up:`, `:x:`, `:link:`, `:copyright:`, and `:white_check_mark:`
- - - 
:+1:,  :smile:, :star:, :exclamation:, :question:, :thumbsdown:, :point_right:, :point_left:, :heart:, :sound:, :lock:, :email:, :guitar:, :one:, :two: (and other #'s), :arrow_left:, :arrow_right:, :arrow_up:, :x:, :link:, :copyright:, and :white_check_mark:

[Back to Top](#back-to-top "Table of contents")

### HTML entities

Just use the HTML entity to display the symbol. Here are the most used ones:

| Entity | Result| Title |
| ---- | ---- | ---- |
| `&copy;` | &copy; | Copyright |
| `&reg;` | &reg; | Registered TM |
| `&trade;` | &trade; | Trademark |
| `&cent;` | &cent; | Cent |
| `&pound;` | &pound; | Pound |
| `&euro;` | **&euro;** | Euro |
| `&not;` | &not; | Negation |
| `&macr;` | &macr; | Spacing Macron |
| `&laquo;` | &laquo; | Left quote? |
| `&raquo;` | &raquo; | Right quote? |
| `&deg;` | &deg; | Degree | 
| `&plusmn;` | &plusmn; | Plus minus | 
| `&sup2;` | 2&sup2; | Supercript 2 | 
| `&#8322;` | H&#8322;O | Subscript 2 | 
| `&#8323;` | NO&#8323;| Subscript 3 | 
| `&para;` | &para; | Paragraph | 
| `&frac14;` | &frac14; | Fractions | 
| `&frac38;` | &frac38; | Fractions | 
| `&times;` | &times; | Multiplication | 
| `&divide;` | &divide; | Division | 
| `&minus;` | &minus; | Subtraction | 
| `&empty;` | &empty; | Empty | 
| `&Phi;` | &Phi; | Phi | 
| `&pi;` | &pi; | Pi | 
| `&sum;` | &sum; | Sum | 
| `&radic;` | &radic; | Square root | 
| `&infin;` | &infin; | Infinity | 
| `&or;` | &or; | Down angle | 
| `&sim;` | &sim; | Proportional | 
| `&asymp;` | &asymp; | Approximately | 
| `≠` | ≠ | Not equal | 
| `&le;` | &le; | Less or equal to | 
| `&ge;` | &ge; | Greater or equal | 
| `&oplus;` | &oplus; | Circle plus | 
| `&ndash;` | &ndash; | En dash? | 
| `&mdash;` | &mdash; | Em dash? | 
| `&larr;` | &larr; | Left arrow | 
| `&rarr;` | &rarr; | Right arrow | 
| `&uarr;` | &uarr; | Up arrow | 
| `&darr;` | &darr; | Down arrow | 
| `&spades;` | &spades; | Spade | 
| `&clubs;` | &clubs; | Club | 
| `&hearts;` | &hearts; | Heart | 
| `&diams;` | &diams; | Diamond | 

NOTE: For subscripts 0 thru 9, change the last number, e.g.:

Zero&#8320; code = `&#8320;` so change 8320 to 8321 for subscript 1 (One&#8321;), change 8320 to 8322 for subscript 2 (Two&#8322;), etc.

[Back to Top](#back-to-top "Table of contents")

- - - 

## Notes

Nothing right now

[Back to Top](#back-to-top "Table of contents")

## Other markdown resources

1. [Daring Fireball](https://daringfireball.net/projects/markdown/basics "Detailed markdown syntax") - more markdown documentation
1. [Complete list of github markdown emojis](https://dev.to/nikolab/complete-list-of-github-markdown-emoji-markup-5aia) - Emojis
1. [GitHub emoji list](https://gist.github.com/rxaviers/7360908) - Emojis

[Back to Top](#back-to-top "Table of contents")
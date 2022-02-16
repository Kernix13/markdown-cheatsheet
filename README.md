# MARKDOWN CHEAT SHEET

Use this markdown cheat cheat as a guide for writing your markdown files. If you like it then clone or fork it, or at least click the **star** button. You can also check out the [Markdown Cheat Sheet article](https://kernixwebdesign.com/website/code/markdown-cheat-sheet-beginners/) I wrote, though it is not as inclusive as this guide.

I'm breaking up all the markdown syntax into 6 categories:

1. Styles
1. Links
1. Lists
1. Code 
1. Hidden
1. Miscellaneous

I'll explain what those mean in each section. But the point is that the first one (**Styles**) can be applied to all or some of the elements in each category with the exception of the Code category. That will make sense when you read each category descripion and notes.

**NOTE**: To view markdown in VS Code hit <kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+V or click the preview button at top right in line with the file name tabs.

<a id="back-to-top"></a>

## ~~A Literal~~ **Table** of *Contents*

| Category | Element | Accepts styles? | 
| -------: | :------ | :-------------: |
| **[Styles](#styles)**: | [Bold](#bold) | `N/A` |
|                        | [Italic](#italic) | `N/A` |
|                        | [Strike thru](#strike-thru) | `N/A` | 
| **[Links](#links)**:     | [External](#external) | **Yes** |
|                          | [Anchor](#anchor)   | **Yes** |
|                          | [Footnotes](#footnotes) | **Yes** |
| **[Lists](#lists)**:     | [Unordered](#unordered)  | **Yes** |
|                          | [Ordered](#ordered)   | **Yes** |
|                          | [Nested](#nested)    | **Yes** |
|                          | [Tasks](#tasks)     | No |
| **[Code](#code)**:        | [Inline](#inline) | No |
|                           | [Tab](#tab) | No |
|                           | [Generic](#generic) | No |
|                           | [Language block](#language-block) | No |
|                           | [Diff](#diff) | No |
| **[Hidden](#hidden)**: | [Comments](#comments) | No |
|                       | [Spoiler](#spoiler) | **Yes** |
|                        | [Details](#details) | No |
| **[Misc](#misc)**: | [Headings](#headings) | **Yes** |
|                | [Blockquotes](#blockquotes) | **Yes** |
|                | [Tables](#tables) | **Yes** |
|                | [Horizontal rules](#horizontal-rules) | **Yes*** |
|                | [Images](#images) | No |
|                | [Emojis](#emojis) | No |
|                | [HTML entities](#html-entities) | No |
| **[Notes](#notes)** | N/A | |
| **[Resources](#resources)** | N/A | |

- - - 

Since paragraphs are a thing of their own, let's cover that one first:

**Paragaphs**: Just use regular text but make sure to hit the <kbd>ENTER</kbd> key twice. Sometimes if you only hit <kbd>ENTER</kbd> once, the text will de displayed as the element directly above it.

## Styles

This category deals with the styling of individual words and can be used with every category except the Code category.

You can apply these effects to all or some of the words in:

- Headings
- Blockquotes
- Table cell values
- HTML entities (except strikethrough)
- Hidden (Spoiler only)

These do not work for the obvious ones (Horizontal Rules, Images, and Emojis), and for all elements in the Code category. 

[Back to Top](#back-to-top "Table of contents")

### Bold

**Bold**: use either 2 **asterisks** or 2 __underscores__ before and after the text for bold styling. The preferred syntax is to use asterisks for bold:

    **two asterisks**
    __two underscores__

###  Italic

**Italic**: use a *single asterisk* or _underscore_ before and after the text for italic styling. The preferred syntax is to use an underscore for italic:

    *single asterisk*
    _single underscore_

**_Bold and Italic_**: use either ***3 asterisks*** or **_2 asterisks and 1 underscore_** for bold and italic text. The preffered syntax is the latter:

    ***3 asterisks***
    **_2 asterisks and and 1 underscore_**

### Strike thru

**Strikethrough**: use two tildes (~~) before and after text that you want to display as ~~strikethrough~~:

    ~~double tildes~~

If you want, you can also do **~~bold strikethrough~~**, _~~_italic strikethrough_~~, and ***~~bold italic strikethrough~~***.

[Back to Top](#back-to-top "Table of contents")

- - - 

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

[Back to Top](#back-to-top "Table of contents")

### Anchor

**Same page anchor links**: This can be done in at least two different ways. For all the links in the table of contents I use the simpler method. But for the **Back to Top** link I use an actual `<a>` tag.

For the simple links, use the same syntax as for **Links** above with 2 exceptions for the URL part:

- precede the *URL* with a hashtag
- use the exact same text as where you are linking to but
  - all the text needs to be in lowercase, and
  - all words need to be connected with a dash (no spaces)  

Here is an example for the *Strike thru* section:

    [Strike thru](#strike-thru)

Here is the code for the anchor link using an HTML `<a>` tag:

    <a id="back-to-top"></a>

Here is the matching link for the above:

    [Back to Top](#back-to-top)

[Back to Top](#back-to-top "Table of contents")

### Footnotes

**Footnote links**: I assume footnotes would be useful in a very technical or long README file. Use square brackets where you want a footnote link to appear and use a caret symbol (^) followed by the number of the footnote. Then below that add the same syntax followed by a colon and the note itself. That will make the footnote text appear at the bottom of your file: 

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

You can use all text effects but with some exceptions: None of the effects work for Task lists, and you don't seem to be able to use VS Code shortcuts (<kbd>SHIFT+*</kbd>, etc) - you have to manually type *, _ or ~. 

### Unordered

**Unordered lists**: You can use either an asterisk or a dash followed by a space to make a bulleted list. I prefer using a dash since you do not need to use the <kbd>SHIFT</kbd> key:

- list item 1
- list item 2

[Back to Top](#back-to-top "Table of contents")

### Ordered

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

### Nested

**Nested list**: Use the <kbd>SPACEBAR</kbd> key to align directly beneath the first character in the parent list item to create a nested list:

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

### Tasks

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

This category deals with inline code and various typs of code blocks and none of them accept Styles:

- Inline code
- Code blocks
- <kbd>TAB</kbd> code blocks
- Code highlighting blocks
- Diff code blocks

### Inline

Use a `single backtick` before and after text to display it as inline code:

    `single backtick`

### Tab

It took me a while how to show the 3 backticks for a code block. For that and other tricky markdown that will not dispay, hit the <kbd>TAB</kbd> button twice then enter your code:

    This is a TAB code block, check with `backticks`

### Generic

To add code that requires more than 1 line then use 3 backticks, hit <kbd>ENTER</kbd>, add your code block, hit <kbd>ENTER</kbd> again and add 3 more back ticks. 

    ```
    some code here
    more here
    ```

```
a {
  text-decoration: none;
}
```

[Back to Top](#back-to-top "Table of contents")


### Language block

This is what you want to use. To highlight parts of your code add the language after the opening triple backticks. You'll have to do your own research but so far the following languages work: `md`, `html`, `css`, `js` or `javascript`, `php`, `xml`, `python`, `sql`, and `apacheconf` (for Apache servers). I tried using `node` and `npm` for my node-npm repo but it had no effect.

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

[Back to Top](#back-to-top "Table of contents")

- - - 

## Hidden

This is an odd category with 3 effects, one of which you have probably only seen in discord:

- Comments
- Spoiler text
- Details

Only Spoiler text accepts text effects.

### Comments

This is a nice way to add a comment in the editor view of your markdown file. This would be good for teams members editing a documentation page for a new section. The best way is to use HTML syntax:

<!-- There is a comment here that you can't see -->

    <!-- There is a comment here that you can't see -->


### Spoiler

On Discord you may sometimes see a black rectangle that reveals text or code when you click on it. Use double pipes before and after the word(s)/code that you want to conceal:

    ||Spoiler text|| in Discord

**NOTE**: This does not work on Slack or here on GitHub.

[Back to Top](#back-to-top "Table of contents")

### Details

This isn't a markdown thing but it is another example of using HTML tags in a Markdown file. It has the same effect as an accordian. I'm not sure why you would use this but here is how you would do it:

<details>
  <summary>Title 1</summary>
  <p>Some hidden content goes here</p>
  Here is some more without <p> tags
</details>
<details>
  <summary>Title 2</summary>
  <p>Same stuff here</p>
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

## Misc

The elements in this category are all unique and do not fit into any of the other category:

- Headings
- Blockquotes
- Tables
- Horizontal rules
- Images
- Emojis
- HTML entities

All elements in this category accept text effects except for the obvious one: images, emojis and horizontal rules.

### Headings

There are 6 headings just like in HTML. Use a single hashtag for H1 and 6 hashtags for H6. The top title of this docuement is an H1 with a single hash, this section (**Misc**) uses 2 hashtags, and this sub-section (**Headings**) uses 3 hashtags. 

**NOTE**: There is an automatic horizontal rule added when you use syntax for H1 and H2.

    # MARKDOWN CHEAT SHEET (Heading 1)
    ## Styles (Heading 2)
    ### Headings (heading 3)
    ### Heading 4 (you most likely will not use H5 or H6) 

Here is an example of using Bold, Italic, and Strikethrough in a heading:

    ## ~~A Literal~~ **Table** of *Contents*

[Back to Top](#back-to-top "Table of contents")

### Blockquotes

This is a nice effect but I don't know why you would use it on GitHub:

> Use a greater than sign (>) to quote a team member
> 
> Create a space like above using > with no text

    > use greater than sign (>) for a blockquote


### Tables

Here is a generic table but the Table of Contents above is another version. The pipes create the columns, the colons with dashes create the alignment:

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

**NOTE**: Make sure to hit <kbd>ENTER</kbd> twice if you intend to use 3 asterisks witout spaces or it will set the text above it to an H3 tag.

[Back to Top](#back-to-top "Table of contents")

### Images

Images use the same syntax as **Links** except for the addition of an exclamation mark immediately before the opening square bracket. You can also use the optional title text:

![picture alt text](https://via.placeholder.com/150 'Title is optional')

    ![picture alt](https://via.placeholder.com/150 'Title is optional')

[Back to Top](#back-to-top "Table of contents")

### Emojis

I'm not a huge fan of emojis, but here are some that I would consider using. The syntax is the emoji code in between colons:

    :Emoji_code:

`:+1:`,  `:smile:`, `:star:`, `:exclamation:`, `:question:`, `:thumbsdown:`, `:point_right:`, `:point_left:`, `:heart:`, `:sound:`, `:lock:`, `:email:`, `:guitar:`, `:one:`, `:two:` (and other #'s), `:arrow_left:`, `:arrow_right:`, `:arrow_up:`, `:x:`, `:link:`, `:copyright:`, and `:white_check_mark:`
- - - 
:+1:,  :smile:, :star:, :exclamation:, :question:, :thumbsdown:, :point_right:, :point_left:, :heart:, :sound:, :lock:, :email:, :guitar:, :one:, :two: (and other #'s), :arrow_left:, :arrow_right:, :arrow_up:, :x:, :link:, :copyright:, and :white_check_mark:

[Back to Top](#back-to-top "Table of contents")

### HTML entities

This actually is not a markdown thing but it's nice having a list for use in your README files. This would be helpful if you are a dev who loves and specializes in say science or math, etc. Here are the most used ones:

**Common**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&copy;` | &copy; | Copyright |
| `&reg;` | &reg; | Registered TM |
| `&trade;` | &trade; | Trademark |
| `&commat;` | &commat; | Self-explanatory | 
| `&larr;` | &larr; | Left arrow | 
| `&rarr;` | &rarr; | Right arrow | 
| `&uarr;` | &uarr; | Up arrow | 
| `&darr;` | &darr; | Down arrow | 
| `&or;` | &or; | Down angle | 


**Financial**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&cent;` | &cent; | Cent |
| `&pound;` | &pound; | Pound |
| `&euro;` | **&euro;** | Euro |

Math and science:
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
| `&sum;` | &sum; | Sum | 
| `&radic;` | &radic; | Square root | 
| `&infin;` | &infin; | Infinity | 
| `&sim;` | &sim; | Proportional | 
| `&asymp;` | &asymp; | Approximately | 
| `≠` | ≠ | Not equal | 
| `&le;` | &le; | Less or equal to | 
| `&ge;` | &ge; | Greater or equal | 
| `&ang;` | &ang; | Angle |
| `&angmsd;`| &angmsd; | Measured angle |

**NOTE**: For subscripts 0 thru 9, change the last number, e.g.:

Zero&#8320; code = `&#8320;` so change 8320 to 8321 for subscript 1 (One&#8321;), change 8320 to 8322 for subscript 2 (Two&#8322;), etc.

**Music**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&#9837;`| &#9837; | Music flat |
| `&#9838;`| &#9838; | Music natural |
| `&#9839;`| &#9839; | Music sharp |
| `&#119070;`| &#119070; | G-clef |
| `&#119092;`| &#119092; | Common time |
| `&#119093;`| &#119093; | Cut time |
| `&#248;`| &#248; | Half-diminished 7th |
| `&sung;`| &sung; | 8th note |

**Miscellaneous**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&not;` | &not; | Negation (?) |
| `&macr;` | &macr; | Spacing Macron (?) |
| `&spades;` | &spades; | Spade | 
| `&clubs;` | &clubs; | Club | 
| `&hearts;` | &hearts; | Heart | 
| `&diams;` | &diams; | Diamond |
| `&star;`| &star; | Star |
| `&starf;`| &starf; | Filled star |
| `&female;`| &female; | Female |
| `&male;`| &male; | Male |
| `&laquo;` | &laquo; | Left quote (?) |
| `&raquo;` | &raquo; | Right quote (?) |
| `&para;` | &para; | Paragraph | 
| `&ndash;` | &ndash; | En dash (?) | 
| `&mdash;` | &mdash; | Em dash (?) | 

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
| Up | ↑ |
| Down | ↓ |
| Left | ← |
| Right | → |

[Back to Top](#back-to-top "Table of contents")

- - - 

## Notes

The one thing I want to look into is using videos, animated GIFs, and more HTML tags in your profile and MD files. Oh, and also 2 and 3-column layouts. STOPPED

I used a GitHub generator for my Profile README. In there are `<p>`, `<a>`, and `<img>` tags. In the Details section above, there are `<details>`, `<summary>`, and `<p>` tags. I found this gist called <q>HTML Tags You Can Use on GitHub</q>. That document mentions that you can also use a number of different tags. Here they are with the ones I used above: 

Block tags
- `<p>`: Why? A-ha! In my profile generated text, the `<p>` tags have inline styles! That's why: `<p align="left">`
- `<div>`: Why?
- `<details>`, and `<summary>`: Why?
- `<dl>`, `<dt>`, and `<dd>`: Definition details tag (added below). Nice indentation.

Inline tags
- `<a>`: Why? Because of the atributes maybe? In my profile readme is `target="_blank"`
- `<img>`: Why? Because of the atributes maybe? Profile readme has `width="40" height="40"` 
- `<samp>`: <samp>Outputs text in monospace font like this line.</samp> 
- `<sub>`: Subscript<sub>1</sub>
- `<sup>`: Superscript<sup>2</sup>
- `<ins>`: Gives you an <ins>underlined</ins> effect.
- `<del>`: Similar to <del>strikethrough</del>.
- `<var>`: Used for variables and is similar to <var>italics</var>.
- `<q>`: I used this above in the title for the GitHub gist, but it adds <q>quotes around text</q>.
- `<kbd>`: Keyboard thing (in many of the above sections)

`<a>` tag attributes: hreflang, media, rel, target (**YES**), type
`<img>` tag attributes: height, width, sizes

**`dl`, `dt`, and `dd` example**:
<dl>
  <dt>Markdown</dt>
  <dd>The language used for your GitHub files</dd>
</dl>

```
<dl>
  <dt>Markdown</dt>
  <dd>The language used for your GitHub files</dd>
</dl>
```

Personally, I will look into using those tags in my README files and maybe try out *EVERY* HTML tag - when I have more time.

[Back to Top](#back-to-top "Table of contents")

## Resources

1. [Daring Fireball](https://daringfireball.net/projects/markdown/basics "Detailed markdown syntax") - more markdown documentation
1. [Complete list of github markdown emojis](https://dev.to/nikolab/complete-list-of-github-markdown-emoji-markup-5aia) - Emojis list
1. [GitHub emoji list](https://gist.github.com/rxaviers/7360908) - Emojis list
1. [Shields.io](https://shields.io/) - Shields for your projects

[Back to Top](#back-to-top "Table of contents")

<!-- 

**Esoteric**:
| Entity | Result| Title |
| ---- | ---- | ---- |
| `&oplus;` | &oplus; | Earth | 
| `&#9793;` | &#9793; | Earth | 
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
| `&#9794;`| &#9794; | Mars |
| `&#9795;`| &#9795; | Jupiter |
| `&#9796;`| &#9796; | Saturn |
| `&#9797;`| &#9797; | Uranus |
| `&#9798;`| &#9798; | Neptune |
| `&#9799;`| &#9799; | Pluto |

 -->
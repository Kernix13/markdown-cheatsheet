# MARKDOWN CHEAT SHEET

Use this markdown cheat cheat as a guide for writing your markdown files. If you like it then clone or fork it, or at least click the **star** button. You can also check out the [Markdown Cheat Sheet article](https:/kernixwebdesign.com) I wrote, though it is not as inclusive as this guide.

In the **basics markdown** section I have the simplest markdown syntax and the most basic styling to use in your markdown files and on sites like Discord and Slack. Thee are a number of forums and support ticket apps that allow markdown so keep that in mind.

In the **intermediate section** are styling examples to make your markdown look even more professional. Theat also applies to what I am calling **Advanced markdown**. It's not that there is advanced markdown, it's just the syntax in that section requires more than just a single character to display your markdown. 

You will not land a job because you are great with markdown, but it subconsciously makes a great first impression. Imagine a potential employer seeing your repo README files and the impression it makes if they are simple paragraphs or one that is rich with styling. In a pool of potential job canddates, you can either rise on that list or fall to the bottom.

**NOTE**: To view markdown in VS Code hit CTRL+SHIFT+V or click the preview button at top right in line with the file name tabs.

<a id="back-to-top"></a>

## Table of contents
1. [Basic markdowm](#basic-markdowm)
   1. [Headings and paragraphs](#headings-and-paragraphs)
   1. [Text decoration](#text-decoration)
   1. [Block quotes](#block-quotes)
   1. [Lists](#lists)
   1. [Inline code](#inline-code)
   1. [Horizontal rules](#horizontal-rules)
1. [Intermediate markdown](#intermediate-markdown)
   1. [Links](#links)
   1. [Images](#images)
   1. [Code blocks](#code-blocks)
   1. [Code blocks with highlighting](#code-blocks-with-highlighting)
   1. [Diff code blocks](#diff-code-blocks)
   1. [Comments](#comments)
1. [Advanced markdown](#advanced-markdown)
   1. [Task lists](#task-lists)
   1. [Tables](#tables)
   1. [Foldable text](#foldable-text)
   1. [Emojis](#emojis)
1. [Notes](#notes)
   1. [Hidden text on Discord](#hidden-text-on-discord)
   1. [Other resources](#other-resources)

## Basic markdowm

Here are the commands that use a simple characters to display markdown. Start with these and then move onto the other sections when you feel your README files are too simple.

### Headings and paragraphs

There are 6 headings just like in HTML. Use a single hashtag for H1 and 6 hashtags for H6. The top title of this docuement is an H1 with a single hash, this section (Basic markdown) uses 2 hashtags, and this sub-section (Headings and paragraphs) uses 3 hashtags. 

**NOTE**: There is an automatic horizontal rule added when you use syntax for H1 and H2.

    # MARKDOWN CHEAT SHEET (Heading 1)
    ## Basic markdowm (Heading 2)
    ### Headings and paragraphs (heading 3)
    ### Heading 4 (you most likely will not use H5 or H6) 

**Paragaphs**: Just use regular text but make sure to hit the *ENTER* key twice. Sometimes if you only hit ENTER once, the text will de displayed as the element directly above it.

    Try 2 tabs to create a code block type effect. This is a plain paragraph.

[Back to Top](#back-to-top "Table of contents")

### Text decoration

**Bold**: use either 2 **asterisks** or 2 __underscores__ before and after the text for bold styling. The preferred syntax is to use asterisks for bold:

    **two asterisks**
    __two underscores__


**Italic**: use a *single asterisk* or _underscore_ before and after the text for italic styling. The preferred syntax is to use an underscore for italic:

    *single asterisk*
    _single underscore_

**_Bold and Italic_**: use either 3 asterisks or 2 asterisks and 1 underscore for bold and italic text. The preffered syntax is the latter:

    ***3 asterisks***
    **_2 asterisks and and 1 underscore_**

**Strikethrough**: use two tildes (~~) before and after text that you want to display as ~~strikethrough~~:

    ~~double tildes~~

[Back to Top](#back-to-top "Table of contents")

### Block quotes

> Use a greater than sign (>) to quote a team member
> 
> Create a space like above using > with no text

    > use greater than sign (>) for a blockquote

### Lists

**Ordered lists**: You can use either an asterisk or a dash followed by a space to make a bulleted list. I prefer using a dash since you do not need to use the *SHIFT* key:

- list item one
- list item 2
  - child item 1

**Nested list**: Use the *SPACEBAR* key to align directly beneath the first character in the parent list item to create a nested list

    - List item one
    - List item two
      - Child item one

**Ordered lists**: use a number followed by  a period (1., 2., 3. etc.) to create an ordered list. For a nested ordered list, do the same as for nested unordered lists - align the number to be below the first character of the parent item:

1. Ordered item 1
1. Ordered item 2
   1. Child item 1

```
1. Ordered item 1
1. Ordered item 2
   1. Child item 1
```
**NOTE**: By using "1" for each list item, you can cut & paste to change the order of items and the numbering will change to match the new order.

[Back to Top](#back-to-top "Table of contents")

### Inline code

Use a `single backtick` before and after text to display it as inline code:

    `single backtick`

### Horizontal rules

Use 3 asterisks or dashes with or without a space to create a horizontal rule:

- - - 

    - - - 
    ---
    * * * 
    ***

**NOTE**: Make sure to hit _ENTER_ twice if you intend to use 3 asterisks witout spaces or it will set the text above it to an H3 tag.

[Back to Top](#back-to-top "Table of contents")

## Intermediate markdown

The following syntax requires a number of different characters to create the styling effects.

### Links

**External Links**: The syntax is to use square brackets around the link text and parentheses for the URL. You can also add an additional title for the link by adding a space after the URL and adding the link title in double quotes:

Here is a link to my [Beginner Git Commands](https://github.com/Kernix13/beginner-git-commands) repositiory. And here is the syntax:

    [Link text](URL "Optional link title")

**NOTE**: Only use a title if it adds information. Don't set the title text to be the same as the link text.


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

### Images

Images use the same syntax except for the addition of an exclamation mark immdiately before the opening square bracket. You can also use optional title text:

![picture alt text](https://via.placeholder.com/150 'Title is optional')

    ![picture alt](https://via.placeholder.com/150 'Title is optional')


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

### Code blocks with highlighting

This is what you want to use. To highlight parts of your code add the language after the opening triple backticks. You'll have to do your own research but so far the following languages work: `md`, `html`, `css`, `js` or `javascript`, `php`, `xml`, `python`, `sql`, `apacheconf` (for Apache servers). I tried using `node` and `npm` for my node-npm repo but it had no effect.

    ```css
    rules here
    ```

```css
a {
  text-decoration: none;
}
```

```md
## Heading 2
```

```html
<img href="http://somewhere.com" />
```

```js
console.log(${variable})
```

```php
<?php the_content(); ?>
```

[Back to Top](#back-to-top "Table of contents")

#### Diff code blocks

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

### Comments

This is a nice way to add a comment in the editor view of your markdown file. This would be good for teams members editing a documentation page for a new section. The best way is to use HTML syntax:

<!--There is a comment here that you can't see -->

    <!-- Now you can see it -->

## Advanced markdown

The following examples bring your markdown files up to the next level and will make your files stand out!

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

### Foldable text

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

### Emojis

I'm not a huge fan of emojis, but here are some that I would consider using:

:+1: and :smile: and :star: and :exclamation: and :question: and :thumbsdown: and :point_right: and :point_left: and :heart: and :sound: and :lock: and :email: and :guitar: and :one: and :two: etc :arrow_left: and :arrow_right: and :arrow_up: and :x: and :link: and :copyright: and :white_check_mark:

```
:+1: and :smile: and :star: and :exclamation: and :question: and :thumbsdown: and :point_right: and :point_left: and :heart: and :sound: and :lock: and :email: and :guitar: and :one: and :two: etc :arrow_left: and :arrow_right: and :arrow_up: and :x: and :link: and :copyright: and :white_check_mark:
```

[Back to Top](#back-to-top "Table of contents")

## Notes

There are other options for some of the styling mentioned above. I only included that which is easiest and that I prefer. Check the links below to more information on Markdown syntax. 

For discord, you have to enter the markdown syntax to have it display, however, on Slack there are editor buttons for everything in this guide.

### Hidden text on Discord

On Discord you may sometimes see a black rectangle that reveals text or code when you click on it. Use double pipes before and after the text/code that you want to conceal:

    ||Spoiler text|| in Discord


**NOTE**: This does not work on Slack or here on GitHub.

I'm adding on definitions because I saw it on a Markdown post but it doesn't work for me. Perhaps this only works in Discord as well. Let me know if you know how to use that:

    Definition: term : definition

[Back to Top](#back-to-top "Table of contents")

### Other resources

1. [Daring Fireball](https://daringfireball.net/projects/markdown/basics "Detailed markdown syntax")
1. [Complete list of github markdown emojis](https://dev.to/nikolab/complete-list-of-github-markdown-emoji-markup-5aia)
1. [GitHub emoji list](https://gist.github.com/rxaviers/7360908)

[Back to Top](#back-to-top "Table of contents")
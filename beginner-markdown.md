# Markdown Cheatsheet

You can preview markdown files in VS Code by using `CTRL + SHIFT + V`. The review is preet good - don't bother with extensions.

You can also preview markdown files in a web browser. I recommend the Chrome extension [Markdown Preview Plus](https://chromewebstore.google.com/detail/markdown-preview-plus/febilkbfcbhebfnokafefeacimjdckgl?pli=1) and I suggest choosing the theme called `ClearnessDarkLg`. You can then bookmark your "Best Of" notes for quick viewing.

## Paragraphs and text formatting

Paragraphs are just plain text but you need to hit <kbd>ENTER</kbd> twice to create a line break between paragraphs. If you only hit <kbd>ENTER</kbd> once, then the paragraphs will run into each other.

### Formatting

You can make most text

1. Bold
2. Italic
3. Bold-italic
4. Strikethrough

There are alternate ways for bold and italic, but below is the correct way to do it. If you have Prettier VS Code Extension, it will correct the alternate methods to what you see below below:

- Surround text with 2 asterisks for **bold text**.
- Surround text with 1 underscore for _italic text_.
- Use 2 asterisks and an inside underscore for or **_bold-italic text_**.
- Use 2 tildes for ~~strikethrough text~~.

```md
- Surround text with 2 asterisks for **bold text**.
- Surround text with 1 underscore for _italic text_.
- Use 2 asterisks and an inside underscore for **_bold-italic text_**.
- Use 2 tildes for ~~strikethrough text~~.
```

You may read that you can use 1 asterisk for italic or 3 asterisks for bold-italic, but Prettier will revert that syntax to what you see above.

**NOTE**: If you select a word or multiple words then hold SHIFT, you can wrap the words with `*`, `_`, `~`, or backticks. Otherwise, you have to add the characters to the beginning and end individually with **_NO_** spaces between the text and the symbols.

## Headings

- The heading above is an H2: `## Headings`
- Use a hash tag for each heading number level you want followed by a space
- Heading levels 1 and 2 have horizontal rules below them.
- FYI, H4 titles (`####`) are the same size as bold paragraph text.
- **NOTE**: As in HTML, H4 headings are sometimes used, H5 and H6 are rarely to never used.

```md
# H1 heading - 1 hashtag

## H2 heading - 2 hashtags

### H3 heading - 3 hashtags

#### H4 heading - 4 hashtags

##### H5 heading - 5 hashtags

###### H6 heading - 6 hashtags
```

## Lists

**NOTE**: To nest lists (ordered or unordered), make sure you line up the indented list symbol with the start of the text in the parent item above it.

### Ordered lists:

Use a number followed by a period then a space for each list item.

1. Item 1
2. Item 2
3. Item 3
   1. Child item 1 if you need a nested list

```md
1. Item 1
2. Item 2
3. Item 3
   1. Child item 1 if you need a nested list
```

### Unordered Lists:

Use a dash, a plus or a single asterisk (dashes are easier) followed by a space for each list item

- Item 1
- Item 2
- Item 3
  - Child Item 1 if you need a nested list

```md
- Item 1
- Item 2
- Item 3
  - Child Item 1 if you need a nested list
```

How to you add a paragraph, image, or code block inside a list? Add a line break and line up element or text with the beginning of the text in the list item.

- One
- Two

  ```js
  console.log('Note empty line above and below this code block');
  ```

- Three
  ```js
  console.log('Without an empty line');
  ```
- Four

  Paragraph here with empty line above and below

  > _Blockquote here with empty line above and below_

- Five

````md
- One
- Two

  ```js
  console.log('Note empty line above and below this code block (no effect)');
  ```

- Three
  ```py
  print('Without an empty line');
  ```
- Four

  Paragraph here with empty line above and below

  > _Blockquote here with empty line above and below_

- Five
````

## Links

The syntax for regular links is `[text](url)`, where the text in the square brackets is your link text, and you add the url in the parentheses. You can add an optional title for the link after the URL. Hover over the link below to see the title.

[Code:You](https://code-you.org/ 'Optional title here')

```md
[Code:You](https://code-you.org/ 'Optional title here')
```

**NOTE**: If you have a URL in your clipboard, highlight the text you want to be a link then just paste (<kbd>CTRL</kbd> + <kbd>V</kbd>) the link and VS Code will format the link for you.

But there are variations:

- Normal syntax (BEST): [Code:You](https://code-you.org/ 'Optional title here')
- Angle brackets: <https://code-you.org/>
- Just href: https://code-you.org/ (May not display as a link depending on the platform)

```md
- Normal syntax (BEST): [Code:You](https://code-you.org/ 'Optional title here')
- Angle brackets: <https://code-you.org/>
- Just href: https://code-you.org/ (May not display as a link depending on the platform)
```

Another excellent variation is replacing the parentheses `(href)` with another set of square brackets with a "token" inside `[1]`, where the token is usually a number. This is good where you have really long href values and you want to clean up your markdown. It would be best to place the href at the bottom of the markdown file similar to footnote links. That way you can keep track of them easier, but they can go anywhere:

- [Code:You][1]
- [CodeWars][2]

<!-- Put these at the bottom of you markdown file for easy reference -->
<!-- Although you could add them below your link if you are only using one time -->

[1]: https://code-you.org/
[2]: https://www.codewars.com/

```md
- [Code:You][1]
- [CodeWars][2]

<!-- Put these at the bottom of you markdown file for easy reference -->
<!-- Although you could add them below your link if you are only using one time -->

[1]: https://code-you.org/
[2]: https://www.codewars.com/
```

If you want a title then you need to use the standard syntax.

### Same page anchor links

You can also link to a heading section within a markdown file. To do this:

1. Add the exact heading text in the square brackets
2. Add a hash tag in the parentheses followed by the heading text all lowercase and connected with dashes

[Other markdown options](#other-markdown-options)

```md
[Other markdown options](#other-markdown-options)
```

## Code

1. Inline code: Use single backticks around a filename or piece of code like `README.md`, `background-color`, `<section>`, `getElementById()`, etc.

```
1. Inline code: Use single backticks around a filename or piece of code like `README.md`, `background-color`, `<section>`, `getElementById()`, etc.
```

2. Generic code block: To add code that requires more than 1 line use triple backticks, drop down 2 lines and add 3 more triple backicks. Add anything in between both sets of backticks.
3. TAB code block: an alternative to the above is to hit <kbd>TAB</kbd> and then add triple bakcticks. When you hit <kbd>ENTER</kbd> you should remain indented so you can hit <kbd>ENTER</kbd> again and add your ending set of triple backticks.

```
console.log("Hello");
```

````
```
console.log("Hello");
```
````

4. Language syntax code block: add the language after the first set of backticks to see syntax highlighting for the language. Check the GitHub repo [highlight.js](https://github.com/highlightjs/highlight.js/blob/main/SUPPORTED_LANGUAGES.md) for a list of languages and the text needed to indicate the language.

```js
document.getElementById('myId');
```

```html
<a href="https://code-you.org/"> Code:You</a>
```

````
```js
document.getElementById("myId")
```

```html
<a href="https://code-you.org/"> Code:You</a>
```
````

**NOTE**: To get backticks to appear in a code block, wrap the triple backtick code block in quadruple backticks or hit TAB twice:

      ```html
      <a href="https://code-you.org/"> Code:You</a>
      ```

## Images and other graphic elements

1. Images use the same syntax as Links except for the addition of an exclamation mark (`!`) immediately before the opening square bracket. You can also add an optional title after the src/url.

- If you want to control the width and height then you need to use an HTML `<img>` tag

```md
![Alt text here](url-to-image 'Optional title here')

<!-- Or use the footnote syntax -->

![alt text][1]
[1]: src

<!-- Image as a link but with a thumbnail - nest image syntax inside the alt text square brackets -->

[![alt text](src with smaller dimensions)](src)

<!-- OR use an img tag for cleaner syntax -->

[<img src="https://somedomain.com/images/image1.jpg" />](src)
```

.........................................................................

2. Emojis: it's easiest to just copy/paste the actual emoji. The syntax of `:emoji-name:` does not seem to work. This is not markdown syntax, it's just to show you that you can add emojis to markdown files.

Examples: 👍, 😄, 👌, ✅, ✔️, ⭐, 🌟, ❤️, ❗

    :+1:, :smile:, :ok_hand:, :white_check_mark:, :heavy_check_mark:,
    :star:, :star2:, :heart:, :exclamation:

.........................................................................

3. HTML entities: similar to emojis, these are not markdown syntax. You can copy/paste the actual entity or use the syntax which does work for these: prefixed with `&`, ending with `;` with the entity name in between. Here are some examples:

- Copyright: `&copy;` -> &copy;
- Check mark: `&check;` &check;
- Arrowhead: `&#10146;` ➢
- Square root: `&radic;` √
- Airplane: `&#9992;` ✈

## Miscellaneous

1. Horizontal rules: You can add horizontal rules using 3 asterisks or dashes:

---

---

````
```md
***
---
```
````

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

2. Blockquotes: use a greater than sign followed by a space for a blockquote. This one is not used as much but it's easy to do:

> One greater than sign for a blockquote (`>`),
>
> > 2 `>>` for an indented/nested blockquote.

```md
> One greater than sign for a blockquote (`>`),
>
> > 2 `>>` for an indented/nested blockquote.
```

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

3. Tables: You need to use pipe characters, colons, and dashes. The pipes are used to create the columns. The colon position defines the alignment and you need the dashes to complete that syntax. The colon and dashes also set the row above it to column headers which are rendered bold.

| Left aligned Content | Center aligned Content | Right aligned Content |
| :------------------- | :--------------------: | --------------------: |
| Left                 |        Centered        |                 Right |
| Row 2 col 1          |      Row 2 col 2       |           Row 2 col 3 |

```md
| Left aligned Content | Center aligned Content | Right aligned Content |
| :------------------- | :--------------------: | --------------------: |
| Left                 |        Centered        |                 Right |
| Row 2 col 1          |      Row 2 col 2       |           Row 2 col 3 |

<!-- Just copy the table above and edit it -->
```

If you have long lines of text then you should use an html table. That may make your file longer but it's easier to edit:

```html
<table>
  <thead>
    <!-- table header -->
    <tr>
      <th>Col 1</th>
      <th>Col 1</th>
      <th>Col 1</th>
    </tr>
  <thead>
  <tbody>
    <!-- Use a tr for each row -->
    <tr>
      <!-- the # of td elements needs to match the # of th elements above -->
      <td>row 1 col 1</td>
      <td>row 1 col 2</td>
      <td>row 1 col 3</td>
    </tr>
  </tbody>
</table>
```

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

4. Line breaks: use the HTML `<br>` element for line breaks. You will need these in tables for text to wrap or the columns will be too large to view in VS Code or will create horizontal scrolling on GitHub. They are also useful to create more vertical spacing. For tables with lots of text, it would be best to use the HTML `<table>` element, along with `<tbody>`, `<th>`, `<tr>`, and `<td>`.

. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .

5. Comments: You can add comments in your markdown using HTML syntax.

```md
<!-- Line break below, comment here -->
<br>
<br> <br>
```

## Other markdown options

If you want to dive deeper:

- Task lists
- Diff lists/code blocks
- Alerts
- Footnote links
- Underline using the HTML `<ins>` element
- HTML descriptions (`<dl>`, `<dt>`, `<dd>`)
- HTML details (`<details>`, `<summary>`)
- Other HTML elements: `<sub>`, `<sup>`, `<samp>`, `<kbd>`, `<mark>` elements
- Math expressions: may be useful for Data Analysis. See the GitHub blog post [Math support in Markdown](https://github.blog/news-insights/product-news/math-support-in-markdown/)
- Shields.io
- Devicons
- Mermaid Diagrams

If you use HTML tags, you can add `align="center"` or `align="right"` to center or right-align that element.

## Summary

In the beginning stick t o the basics:

1. Paragraphs with bold and/or italics
2. Headings: H1, H2, H3 only
3. Inline code and code blocks
4. Ordered and unordered lists
5. Links
6. Emojis

## Useful Links

1. [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/): beginners guide
2. [markdown-cheatsheet](https://github.com/Kernix13/markdown-cheatsheet): Basic markdown + advanced options for markdown files
3. [Markdown-Cheatsheet](https://github.com/lifeparticle/Markdown-Cheatsheet): Even more advanced options
4. Emoji lists:
   1. [GitHub emoji gist](https://gist.github.com/rxaviers/7360908)
   2. [emoji-cheat-sheet](https://github.com/ikatyang/emoji-cheat-sheet)
   3. [emoji-list](https://github.com/caiyongji/emoji-list)
5. [HTML Entities](https://www.toptal.com/designers/htmlarrows/symbols/)
6. [Devicons for GitHub](https://github.com/devicons/devicon/tree/master/icons)
7. [Sheilds.io](https://shields.io/) - badges for your projects

<!--
  For my CodeYou notes, I only use
  1. Paragraphs
  2. Bold and italic formatting
  3. H1, H2, and H3 headings
  4. Unordered and ordered lists
  5. Inline code
  6. Generic and language specific code blocks
  7. Links

  Other common ones I often use in my READMEs:
  - Markdown and HTML tables
  - Images
  - <br> tags for extra spacing
  - HTML entities and emojis
  - Comments
  - Same page anchor links

  Check these out:

  - awesome-markdown: https://github.com/mundimark/awesome-markdown?tab=readme-ov-file
  - markitdown: https://github.com/microsoft/markitdown
  - accessible markdown: https://github.blog/developer-skills/github/5-tips-for-making-your-github-profile-page-accessible/
 -->

<!--

New one: Horizontal images with gap -> hspace="5"

<p>
  <img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80" width="100" height="100" hspace="5" alt="alt text"/>
  <img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80" width="100" height="100" hspace="5" alt="alt text"/>
  <img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80" width="100" height="100" hspace="5" alt="alt text"/>
</p>

 -->

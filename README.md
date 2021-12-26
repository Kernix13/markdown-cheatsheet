To view markdown in VS Code hit CTRL+SHIFT+V or click the preview button at top right in line with the file name tabs.

Top Anchor<a name="top_anchor"></a>

`Top Anchor<a name="top_anchor"></a>`

# Heading 1

## Heading two

### Heading three

#### Heading four

##### Heading 5

###### Heading 6

```
# Heading 1
## Heading two
### Heading three, etc...
```

---

Apparent background color, just hit TAB twice:

    Like this

_Emphasized/Italic text_ or like _this_

**Bold text** or **like this**

~~Strikethrough text~~

**_Bold and italic_**

```
*Emphasized/Italic text* or like _this_
**Bold text** or __like this__
~~Strikethrough text~~
***Bold and italic***
```

[Text as an external link](https://www.google.com/)

```
[Text as an external link](https://www.google.com/)
```

Make sure anchor links are lowercase and with dashes and maybe underscores in between each word. If you are not using the anchor tag syntax as above, then your #anchor-text has to match the words exactly in the section you are linking to. For example, If you have a section called How to use anchor links, then use #how-to-use-anchor-links.

[Go To TOP](#top_anchor)

```
[Go To TOP](#top_anchor)
```

Tables look good - make sure to use | --- | --- | to make the column headers bold

Left, right and center aligned table:

| Left aligned content | Center aligned content | Right aligned content |
| :------------------- | :--------------------: | --------------------: |
| Content Left         |     Content Center     |         Content Right |
| Content Left         |     Content Center     |         Content Right |

Single tildes for an inline code block:

`code()`

Also this:

||Spoiler text|| in Discord

`Boxed text in Discord`

````
`code()`
``` Boxed text in Discord ```
````

Three tildes for a large code block and addd the language for code highlighting:

```json
{
  "name": "jim",
  "job": "front end developer"
}
```

```js
console.log(${variable})
```

```html
<img href="http://somewhere.com" />
```

```css
body {
  margin: 0 auto;
}
```

```php
<?php the_content(); ?>
```

For example, the above starts with (```json). It's diificult to shw this in a code block, but here is a version with an extra backtick to display it - just use 3 opening and closing backticks. Also, try html, css, js, php, py, etc.

````
` ```diff
- const nums = []
+ const nums = {}
` ```
````

Use 'diff' to show changes and greater than to quote a section of someone's reply:

```diff
- const nums = []
+ const nums = {}
```

For UL use \* or - or +. For nested lists, start nested item at least at the start of its parent. For OL repeat but use the number and a period

```
* Parent item with asterisk
  * Child with asterisk

- Parent item with dash
  - Child with dash

+ Parent item with plus
  + Child with plus

1. Parent ordered item
   1. Child ordered item
1. second item
1. 3rd item
```

For ordered lists, just keep using the #1 and the nmbers will increment. That way if you cut/paste an item to a different position, the numbering will remain correct.

Tasks - uncompleted and completed, can be nested also:

- [ ] incomplete
- [x] complete
  - [ ] incomplete subtask
  - [x] complete subtask

Use the greater than sign for blockquotes:

I agree with:

> idea 1

I don't agree with:

> idea 2

```
I agree with:
> idea 1

I don't agree with:
>  idea 2
> ## Heading 2 in a blockquote
```

> ## Heading 2 in a blockquote

---

---

---

Horizontal rule with --- or - - - or \* \* \* (see above):

How to remove the link aspect of an image to the file in the repo?

![picture alt](https://via.placeholder.com/150 'Title is optional')

Images on a row in tables (not responsive):

|                             First image                             |                            Second image                             |                             Third image                             |
| :-----------------------------------------------------------------: | :-----------------------------------------------------------------: | :-----------------------------------------------------------------: |
| ![picture alt](https://via.placeholder.com/150 'Title is optional') | ![picture alt](https://via.placeholder.com/150 'Title is optional') | ![picture alt](https://via.placeholder.com/150 'Title is optional') |

Foldable text is really cool:

<details>
  <summary>Title 1</summary>
  <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
<details>
  <summary>Title 2</summary>
  <p>Content 2 Content 2 Content 2 Content 2 Content 2</p>
  <p>Content 2 Content 2 Content 2 Content 2 Content 2</p>
</details>

Definition:
term
: definition

Footnote.[^1]
Some other important footnote.[^2]

[^1]: This is footnote number one.
[^2]: Here is the second footnote.

use this:

```
[^1]
```

Emojis worth using:

:+1: and :smile: and :star: and :exclamation: and :question: and :thumbsdown: and :point_right: and :point_left: and :heart: and :sound: and :lock: and :email: and :guitar: and :one: and :two: etc :arrow_left: and :arrow_right: and :arrow_up: and :x: and :link: and :copyright: and :white_check_mark:

```
:+1: and :smile: and :star: and :exclamation: and :question: and :thumbsdown: and :point_right: and :point_left: and :heart: and :sound: and :lock: and :email: and :guitar: and :one: and :two: etc :arrow_left: and :arrow_right: and :arrow_up: and :x: and :link: and :copyright: and :white_check_mark:
```

#### Most of these markdown formatting tips work in Discord and in Slack, though Slack has menu icons for most of them as well.

# HTML Tags that can be used in Markdown files

All HTML tags tested to see their effect in a markdown file. Checkout [MDN HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) for a logical breakdown on all HTML tags.



<div id="back-to-top"></div>

## Table of contents

1. [All tags](#all-tags)
1. [Block level tags](#block-level-tags)
   1. [Semanic tags](#semanic-tags)
   1. [Skipped block tags](#skipped-block-tags)
   1. [Unique HTML tags](#unique-html-tags)
   1. [HTML markdon versions](#html-markdon-versions)
   1. [Block tag examples](#block-tag-examples)
1. [Inline tags](#inline-tags)
   1. [Skipped inline tags](#skipped-inline-tags)
   1. [Inline that did not work](#inline-that-did-not-work)
   1. [Formatting text tags](#formatting-text-tags)
   1. [Inline that worked](#inline-that-worked)
   1. [Inline tag examples](#inline-tag-examples)
1. [Block tags that worked](#block-tags-that-worked)
1. [Inline tags that worked](#inline-tags-that-worked)

<br />

## All tags

From MDN:

Top level: Interesting section for the elements about the page - the root element is `<html>`. SKIP ALL OF THESE!

| Root      | Element   | Element   | Element | Element       |
| ---:      | :----:     | :----:    | :----:   | :----:         |
| `<head>`  |           |           |           |             | 
| Common:   | `<meta>`  | `<link>`  | `<title>` | `<script>`  |
| Uncommon: | `<base>`  | `<style>` |           |             |

<br />

Next is the `<body>` tag which contains all the elements that you tend to work with and that are being tested in this file. After that are the semantic **_Content Sectioning_** tags. It makes no sense to test the semantic tags, and all the non-semantic tags work except for address:

| Type          | Tag         | Tag       | Tag         | Tag         | 
| ---:          | :----:      | :----:    | :----:      | :----:      | 
| Semantic:     | `<article>` | `<aside>` | `<footer>`  | `<header>`  | 
|               | `<main>`    | `<menu>`  | `<nav>`     | `<section>` |
| Non-semantic: | `<address>` | `<h1>`    | `<h2>`      | `<h3>`      |
|               | `<h4>`      | `<h5>`    | `<h6>`      | `<hr>`      |

<br />

The next MDN section is called **_Text Content_**:

| Type     | Tag            | Tag       | Tag     | Tag     | Tag     | 
| ---:     | :----:         | :----:    | :----:  | :----:  | :----:  |
| Solo tags: | `<blockquote>` | `<div>` | `<p>`   | `<pre>` | `<dialog>` |
| Grouped tags: | `<dl>`         | `<dt>`    | `<dd>`  | -        | -        |
|          | `<details>` | `<summary>` | - | - | - |   
|          | `<figcaption>` | `<figure>` | -      | -       | -       |
|          | `<li>`         | `<ol>`    | `<ul>`  | -       | -       |     


<br />

The next section is huge: Inline text semantics

| Type          | Tag     | Tag      | Tag      | Tag     | Tag     | 
| ---:          | :----:  | :----:   | :----:   | :----:  | :----:  |
| Solo content: | `<a>`   | `<abbr>` | `<br>`   | `<bdi>` | `<bdo>` | 
|               | `<br>`  | `<cite>` | `<code>` | `<data>` | `<kbd>` | 
|               | `<samp>` | `<small>` | `<span>` | `<sub>` | `<sup>` |
|               | `<time>` | `<var>` | `<wbr>`  | -       | `       | 
| Solo format:  | `<b>`   | `<dfn>`  | `<em>`   | `<i>`   | `<kbd>` |
|               | `<q>`   | `<s>`    | `<strong>` | `<del>` | `<ins>` |       | 
| Connected:    | `<rp>`  | `<rt>`    | `<ruby>` | -      | -       |

<br />

Image and multimedia:

| Element | Element | Element |
| :---    | :----   | :----   |
| `<area>` | `<audio>` | `<img>` |
| `<map>` | `<track>` | `<video>` |

<br /> 

Miscellaneous -> Embedded content, canvas, SVG and MathML:

| Type      | Element | Element | Element |
| :---      | :----:   | :----:   | :----:   |
| Main tag: | `<embed>` | `<iframe>` | `<object>` | 
|           | `<picture>` | `<portal>` | `<svg>` |
|           | `<math>` | `<canvas`> | `<noscript>` |
| Support tags: | `<param>` | `<source>` | - |

<br />

The `<table>` tag: 

- MAIN: `<table>`, `<thead>`, `<tbody>`, `<tfoot> `
- OTHER: `<col>`, `<colgroup>`, `<td>`, `<th>`, `<tr>`

<br />

The `<form>` tag: 

- MAIN: `<form>` and `<fieldset>` with `<legend>`
- GROUPED: `<datalist>`, `<option>`, `<optgroup>`, and `<select>`
- OTHER: `<button>`, `<input>`, `<label>`, `<meter>`, `<output>`, `<progress>`, `<textarea>`

<br />

Wierd ones: `<slot>`, `<template>`

Depricated: `<acronym>`, `<applet>`, `<basefont>`, `<bgsound>`, `<big>`, `<blink>`, `<center>`, `<content>`, `<dir>`, `<font>`, `<frame>`, `<frameset>`, `<hgroup>`, `<image>`, `<keygen>`, `<marquee>`, `<menuitem>`, `<nobr>`, `<noembed>`, `<noframes>`, `<plaintext>`, `<rb>`, `<rtc>`, `<shadow>`, `<spacer>`, `<strike>`, `<tt>`, and `<xmp>`.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Block level tags

28 tags total

### Semanic tags

9 Semantic tags: SKIP

| HTML Tag       | Tested? | Displayed? | 
| ---------:     | :-----: | :--------: |
| `<article>`    | NO      | N/A       | 
| `<aside>`      | NO      | N/A       | 
| `<footer>`     | NO      | N/A       | 
| `<header>`     | NO      | N/A       | 
| `<hgroup>`     | Yes     | N/A       |
| `<main>`       | NO      | N/A       | 
| `<menu>`       | NO      | N/A       | 
| `<nav>`        | NO      | N/A       | 
| `<section>`    | NO      | N/A       | 

### Skipped block tags

7 tags skipped or did not display correctly. Forms, and therefore fieldsets, may need actions to work.

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<address>`    | Yes     | YES        | No         | no italics, needed br tags |
| `<dialog>`     | Yes     | NO         | -          | -        |
| `<fieldset>`   | Yes     | Yes        | Yes        | -              |
| `<legend>`     | Yes     | Yes        | Yes        | -              |
| `<figcaption>` | Yes     | NO         | NO         | -        |
| `<figure>`     | Yes     | NO         | NO         | -        |
| `<form>`       | No      | skip       | -          | -        |

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Unique HTML tags

8 TAGS WITH ALTERNATE FORMATIING THAT WORKED:

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------:       |
| `<blockquote>` | Yes     | YES        | Yes        | Inline CSS?    |
| `<hr>`         | Yes     | Yes        | Yes        | diff size?     |
| `<dd>`         | Yes     | Yes        | Yes        | Indent         |
| `<dl>`         | Yes     | Yes        | Yes        | Indent         |
| `<dt>`         | Yes     | Yes        | Yes        | Indent         |
| `<details>`    | Yes     | Yes        | Yes        | Hidden content |
| `<pre>`        | Yes     | Yes        | Yes        | NO NEED TO USE |
| `<table>`      | Yes     | Yes        | Yes        | Inline CSS?    |

NOTE: `dd`, `dt`, `dl` > 1st 'd' stands for description, 'l' for list, 't' for term, and 2nd 'd' for details, or description list, description term, description details.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### HTML markdon versions

11 TAGS THAT WORKED BUT ALREADY HAVE CORRESPONDING MARKDOWN TAGS:

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<div>`        | Yes     | Yes        | Yes        | Inline CSS? |
| `<p>`          | Yes     | Yes        | Yes        | Inline CSS? |
| `<h1>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<h2>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<h3>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<h4>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<h5>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<h6>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<ol>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<ul>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<li>`         | Yes     | Yes        | Yes        | Inline CSS? |
| **bold test**  | _italic_  | ~~strikethough~~ |    |              |

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Block tag examples

  <fieldset>
    Some text here inside a `fieldset` tag. **Bold**, _italic_, ~~strikethrough~~.
  </fieldset>

<br />

  <fieldset>
    <legend>Legend tag: **Bold**, _italic_, ~~strikethrough~~</legend>
    <code>fieldset</code> tag with a legend tag, inut tags don't display
  </fieldset>

Address tag check (Did not display as italic and needed `br` tags to display as block? Also, `tel` did not diaply as a link)
  <address>
      <a href="mailto:jim@rock.com">jim@rock.com</a><br>
      <a href="tel:+13115552368">(311) 555-2368</a><br>
      Mozilla Foundation<br>
      331 E Evelyn Ave<br>
      Mountain View, CA 94041<br>
      USA
  </address><br>

  <a href="mailto:jim@rock.com">jim@rock.com</a><br>
  <a href="tel:+13115552368">(311) 555-2368</a><br>
  Dark side of the moon<br>
  130 miles away<br>
  Above Earth<br>
  Space<br>

Blockquote tag check: no diff from gt key so will it accept inline css?
<blockquote cite="https://www.huxley.net/bnw/four.html">
    <p>Words can be like X-rays, if you use them properly—they’ll go through anything. You read and you’re pierced.</p>
</blockquote>

> Words can be like X-rays, if you use them properly—they’ll go through anything. You read and you’re pierced.


Figure, img, and figcaption tags check: displayed but as a paragraph
<figure>
    <img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg"
         alt="An eye" width="200px">
    <figcaption>An artistic eye but does it wrap when exceeds the length of the image? With figure element</figcaption>
    <img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg"
         alt="An eye" width="200px">
    <figcaption>An artistic eye but does it wrap when exceeds the length of the image? With figure element</figcaption>
</figure>

Headings and hgroup tag check: no effect for hgroup, inline for headings?
<hgroup>
  <h1>one</h1>
  <h2>two: no auto horiz rule? Yes, there is</h2>
  <h3>three</h3>
  <h4>four</h4>
  <h5>five</h5>
  <h6>six</h6>
</hgroup>

  <h1>HEADING 1 SIZE COMPARED TO PARAGRAPH SIZE</h1>
  <p>PARAGRAPH SIZE COMPARED TO HEADING 1 SIZE</p>
  <h2>HEADING 2 SIZE COMPARED TO PARAGRAPH SIZE</h2>
  <p>PARAGRAPH SIZE COMPARED TO HEADING 2 SIZE</p>
  <h3>HEADING 3 SIZE COMPARED TO PARAGRAPH SIZE</h3>
  <p>PARAGRAPH SIZE COMPARED TO HEADING 3 SIZE</p>
  <h4>MATCH -> HEADING 4 SIZE EQUALS PARAGRAPH SIZE (bold )</h4>
   <p>MATCH -> PARAGRAPH SIZE EQUALS HEADING 4 SIZE (plain)</p>
  <h5>HEADING 5 SIZE COMPARED TO PARAGRAPH SIZE</h5>
  <p>PARAGRAPH SIZE COMPARED TO HEADING 5 SIZE</p>
  <h6>HEADING 6 SIZE COMPARED TO PARAGRAPH SIZE</h6>
  <p>PARAGRAPH SIZE COMPARED TO HEADING 6 SIZE</p>

Takeaway: Consider `h5` or `#####` and `h6` or `######` for a smaller font size block element. 

ol, li, ul tags check: all worked, inline css?
<ul>
  <li>unordered</li>
</ul>
<ol>
  <li>ordered</li>
</ol>

Pre tag check: exactly the same as code blocks BUT WITHOUT CODE HIGHLIGHTING
<pre>
  function testFx() {
    console.log("Hello");
  }
</pre>

Table tag test: inline css? Bold, italic and strikethough do not work in table cells, but they do in markdown tables!!!
<table>
<thead>
<tr>
<th>Format</th>
<th>Syntax</th>
</tr>
</thead>
<tbody>
<tr>
<td>H1</td>
<td>#</td>
</tr>
<tr>
<td>H2</td>
<td>##</td>
</tr>
<tr>
<td>H3</td>
<td>###</td>
</tr>
<tr>
<td>Italics</td>
<td>*italics*</td>
</tr>
<tr>
<td>Bold</td>
<td>**Bold**</td>
</tr>
<tr>
<td>Strike thru</td>
<td>~~strikethrough~~</td>
</tr>
<tr>
<td>Horiz. Rule</td>
<td>&#8211; &#8211; &#8211;</td>
</tr>
<tr>
<td>Block quote</td>
<td>&gt; text here</td>
</tr>
</tbody>
</table>

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Inline tags

55 tags total

### Skipped inline tags

23 tags not even tested because they would not provide value, have no visual distinction, or have no application for a markdown file:

| HTML Tag       | Tested? | Displayed? | 
| ---------:     | :-----: | :--------: | 
| `<abbr>`       | NO      | N/A |
| `<acronym>`    | NO      | N/A |
| `<area>`       | NO      | N/A | 
| `<bdi>`        | No      | N/A |
| `<bdo>`        | No      | N/A |
| `<canvas>`     | No      | N/A |
| `<cite>`       | No      | N/A |
| `<data>`       | NO      | N/A |
| `<datalist>`   | NO      | N/A |
| `<input>`      | No      | N/A |
| `<label>`      | No      | N/A |
| `<map>`        | No      | N/A |   
| `<meter>`      | No      | N/A |
| `<noscript>`   | No      | N/A |
| `<object>`     | No      | N/A |
| `<output>`     | No      | N/A |
| `<portal>`     | No      | N/A |  
| `<progress>`   | No      | N/A |
| `<script>`     | No      | N/A |
| `<select>`     | No      | N/A |
| `<slot>`       | No      | N/A |
| `<template>`   | No      | N/A |
| `<textarea>`   | No      | N/A |
| `<tt>`         | No      | N/A |
| `<wbr>`        | No      | N/A | 

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Inline that did not work

13 tags tested but did not display:

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<audio>`      | YES     | NO         | No          | -         |
| `<big>`        | Yes     | No         | No          | -         |
| `<button>`     | Yes     | No         | No          | -         |
| `<dfn>`        | Yes     | NO         | No          | -         |
| `<embed>`      | Yes     | No         | No          | -         |
| `<iframe>`     | Yes     | No         | No          | -         |
| `<mark>`       | Yes     | NO         | ???         | ???       |
| `math`         | Yes     | Yes        | No          | - |         
| `<picture>`    | yES     | ???        | ???         | ???       |
| `<small>`      | Yes     | No         | No          | -         |
| `<svg>`        | Yes     | No         | No          | -         |
| `<time>`       | Yes     | No         | No          | -         |
| `<u>`          | Yes     | No         | No          | -         |
| `<video>`      | Yes     | No         | No          | -         |

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Formatting text tags

8 TAGS FOR FORMATTING THAT WORKED:

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use?   |
| ---------:     | :-----: | :--------: | :-------:  | :------:   |
| `<b>`          | Yes     | Yes        | -          | <b>Bold</b> |
| `<strong>`     | Yes     | Yes        | -          | <strong>Bold</strong> |
| `<s>`          | Yes     | Yes        | -          | <s>strikethru</s> |
| `<del>`        | Yes     | Yes        | -          | <del>strikethru</del> |
| `<em>`         | Yes     | Yes        | -          | <em>italic</em> |
| `<i>`          | Yes     | Yes        | -          | <i>italic</i> |
| `<var>`        | Yes     | Yes        | No         | <var>Italic</var>     |
| `<ins>`        | Yes     | Yes        | -          | <ins>Underline</ins>  |

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Inline that worked

11 TAGS TESTED THAT WORK:

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use?         |
| ---------:     | :-----: | :--------: | :-------:  | :------:         |
| `<a>`          | Yes     | Yes        | Yes        | no inline or target|
| `<br>`         | YES     | YES        | YES        | Line breaks      |
| `<code>`       | Yes     | Yes        | Yes        | NO NEED TO USE   |
| `<img>`        | Yes     | Yes        | Yes        | Inline CSS?      |
| `<kbd>`        | Yes     | Yes        | Yes        | Styling/Visual   |
| `<q>`          | Yes     | Yes        | Yes        | Not sure         |
| `<ruby>`       | Yes     | Yes        | -          | NOT APPLICABLE   |
| `<samp>`       | Yes     | Yes        | Yes        | Monospaced font! |
| `<span>`       | Yes     | N/A        | Yes        | Uses?            |
| `<sub>`        | Yes     | Yes        | Yes        | Subscript!       |
| `<sup>`        | Yes     | Yes        | Yes        | Superscript!     |

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Inline tag examples

Testing `a` tag: _blank, and inline styles DID NOT WORK

<a href="https://google.com" target="_blank" style="text-decoration: overline underline; font-family: cursive">GOOGLE</a>

Testing `audio` tag: visually appeared in VS Code preview but not on GitHub and does not function.

<audio controls src="https://raw.githubusercontent.com/himalayasingh/music-player-1/master/music/4.mp3">
    Your browser does not support the
    <code>audio</code> element.
</audio>

`b` and `strong` tags test: <br> ALL DISPLAYED
<b>Bold text</b> same as in **markdown** and how about <strong> the strong tag</strong>.

`code` tag test: SAME AS BACKTICKS 

This is a test of the <code>code tag</code> same as `backticks` I bet.

`del` & `s` tags test: BOTH WORKED

<del>Strikethrough text</del> same as in ~~markdown~~ and how about <s>the s tag</s>.

`dfn`, `em` and `i` tags test: EM and I WORKED, DFN DID NOT 

This is <em>em tag italics</em> same as in *markdown* and how about <i>the i tag</i> and <dfn>the dfn tag</dfn>. 

<p>A <dfn id="def-validator">validator</dfn> is a program that checks for syntax errors in code or documents.</p>

<button>Button tag does not work</button>

`embed` tag test: DID NOT DISPLAY

<embed type="video/mp4" src="https://player.vimeo.com/external/194837908.sd.mp4?s=c350076905b78c67f74d7ee39fdb4fef01d12420&profile_id=164" width="450" height="300">

`ins` and `u` tags test: u tag DID NOT WORK ins tag DID!

Will this <u>be displayed as underlined</u> and what about <ins>the ins tag</ins></u>?

`iframe` tag test: DID NOT DISPLAY and for some reason displays the code unlike the other elements that just did not display.

<iframe src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&layer=mapnik" id="inlineFrameExample" title="Inline Frame Example" width="300" height="200">
</iframe>

`mark` tag test: DID NOT DISPLAY

This is a <mark>mark tag</mark>, does it work?

`ruby` tag test: worked but not applicable to me

<ruby>
明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp>
</ruby>

`samp` tag test: WORKED

<p>This is regular text. <samp>SAMP monospaced text: Keyboard not found. Press F1 to continue</samp> and so is this.</p>

`small` and `big` tags test: DID NOT DISPLAY

<p>This is regular text. <small>The content is small</small>, but this isn't. This is <big>Big deprecated text</big></p>

`sub` and `sup` tags test: WORKED

H<sub>2</sub> and 2<sup>3</sup> and <sup>o</sup>7

`svg` tag test: DID NOT DISPLAY

<svg viewBox="0 0 300 100" xmlns="http://www.w3.org/2000/svg" stroke="red" fill="grey">
  <circle cx="50" cy="50" r="40" />
  <circle cx="150" cy="50" r="4" />

  <svg viewBox="0 0 10 10" x="200" width="100">
    <circle cx="5" cy="5" r="4" />
  </svg>
</svg>

`time` tag test: DID NOT WORK

<p>The Cure will be celebrating their 40th anniversary on <time datetime="2018-07-07">July 7</time> in London's Hyde Park.</p>

`var` tag test: ANOTHER VERSION OF ITALICS?

This is a <var>test of the var tag</var>, why would you use it?>

`video` tag test: DID NOT DISPLAY

<video controls width="250">
  <source
    src="https://player.vimeo.com/external/194837908.sd.mp4?s=c350076905b78c67f74d7ee39fdb4fef01d12420&profile_id=164"
    type="video/mp4">
  Sorry, your browser doesn't support embedded videos.
</video>

`q` and `kbd` tags: WORKED

The <q>q tag wraps text in quotes</q>, the kbd tag wraps keyboard stull in a styled format like with <kbd>CTRL</kbd> or <kbd>SHIFT</kbd>.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Block tags that worked

Duplicates markdown: `blockquote`, `h1` thru `h6`, `hr`, `ol` `ul` `li`, `pre`, `table`

Worked but unsure of use: `details` with `summary`, `dl` `dt` `dd` (indent), `div`

> Is align an attribute? How do I find similar attributes like that?

Attributes:
- `blockquote`: global
- `h1` thru `h4`: global, align (center, right)
- `h5` and `h6`: Same as above, very small font size!
- `ol`, `ul`: global
- `li`: global
- `pre`: global
- `table`: global
- `address`: global
- `details`, `summary`: global  
- `dl`, `dt`, `dd`: global
- `div`: global
- `p`: global, align (left, center, right)

Unless there is a way to display the tags differently, then I do not see the point of using `pre`, `table`, `lists`, or `blockquote`. Especially the table tag since there are a lot of tags you need to enter.

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

## Inline tags that worked

Duplicates markdown:
`a`, `b` and `strong` (BOLD), `code`, `del` and `s` (Strikethrough), `em` and `i` and `var` (Italics), `img` (width, align [left, center, right])

Worked:
`br` (line break), `ins` (underline), `sub` and `sup` (Obvious), `samp` (Monospaced font), `q` (quotes), `kbd` (format)

> Do they accept inline CSS?

Attributes:
- `a`: target did not work, no title attribute, no style attribute - DON'T USE!
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

Global attributes: id, class, draggable, **style**, **title**, tabindex, data-*, contenteditable, autofocus, 

The only tags worth using:
- `div` for dividers using - or _ or = or other characters (no use br tags)
- `p` for align center or right
- `headings` for anchor links with html entities or for center or right alignment
- `h5` and `h6` for smaller than paragraph size block elements
- `br` for line breaks of paragrpah text like the `address` tag
- `img` to set width and height and align of center or right
- `ins` for underline
- `kbd` for keyboard chars or other keys
- `samp` for monospaced font
- `sup` and `sub` for super and subscript
- maybe `dl` `dt` `dd` for the indent definition type of style
- maybe `span`

Skip the following unless I can find inline styles or attributes that work with the following: `blockquote`, `ol` `ul` `li`, `table`, `address`, or `a`. As for bold, italic, and strikehrough, just use the markdown versions.

## testing **double asterisks** and <b>the b tag</b> and the <strong>strong tag</strong>
<br><br>
<p align="center">Paragraph align="center", 2 br tags above</p>
<p align="right">Paragraph align="right"</p>
<div align="center">div align="center"</div>
<div align="right">div align="right"</div>

<h2 align="center"><ins>Centered h2</ins></h2>
<h2 align="right">Right h2</h2>

<div align="right">&#8673; <a href="#back-to-top" title="Table of Contents">Back to Top</a></div>

### Testing

abbr tag:

<p>You can use <abbr title="Cascading Style Sheets">CSS</abbr> to style your <abbr title="HyperText Markup Language">HTML</abbr>.</p>

Cite tag - italic link?

  <cite><a href="http://www.george-orwell.org/1984/0.html">Nineteen Eighty-Four</a></cite>
  <br />
  <p><cite>Nineteen Eighty-Four (without link)</cite></p>
  <br />
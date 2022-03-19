# HTML Tags that can be used in Markdown files

## Block level tags

28 tags total

8 Semantic tags: SKIP

| HTML Tag       | Tested? | Displayed? | 
| ---------:     | :-----: | :--------: |
| `<article>`    | NO      | N/A       | 
| `<aside>`      | NO      | N/A       | 
| `<footer>`     | NO      | N/A       | 
| `<header>`     | NO      | N/A       | 
| `<hgroup>`     | Yes     | N/A       |
| `<main>`       | NO      | N/A       | 
| `<nav>`        | NO      | N/A       | 
| `<section>`    | NO      | N/A       | 

<br />

6 tags skipped or did not display correctly. Forms, and therefore fieldsets, may need actions to work.

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<address>`    | Yes     | YES        | No         | no italics, needed br tags |
| `<dialog>`     | Yes     | NO         | -          | -        |
| `<figcaption>` | Yes     | NO         | NO         | -        |
| `<figure>`     | Yes     | NO         | NO         | -        |
| `<fieldset>`   | NO      | -          | -          | -        |
| `<form>`       | No      | skip       | -          | -        |

<br />

8 TAGS WITH ALTERNATE FORMATIING THAT WORKED:

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<blockquote>` | Yes     | YES        | Yes        | Inline CSS? |
| `<hr>`         | Yes     | Yes        | Yes        | diff size? |
| `<dd>`         | Yes     | Yes        | Yes        | Indent   |
| `<dl>`         | Yes     | Yes        | Yes        | Indent   |
| `<dt>`         | Yes     | Yes        | Yes        | Indent   |
| `<details>`    | Yes     | Yes        | Yes        | Hidden content |
| `<pre>`        | Yes     | Yes        | Yes        | NO NEED TO USE |
| `<table>`      | Yes     | Yes        | Yes        | Inline CSS? |

NOTE: dd, dt, dl > 1st 'd' stands for description, 'l' for list, 't' for term, and 2nd 'd' for details, or description list, description term, description details.

<br />

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

Address tag check (Did not display as italic but lines were directly below each other but was that the br tags and not the address tags? Also, `tel` did not diaply as a link)
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
  <h4>MATCH -> HEADING 4 SIZE EQUALS PARAGRAPH SIZE</h4>
   <p>MATCH -> PARAGRAPH SIZE EQUALS HEADING 4 SIZE</p>
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

## Inline tags

55 tags

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<a>`          | Yes     | Yes        | Yes        | no inline or target|
| `<abbr>`       | NO      | -          | -          |          |
| `<acronym>`    | NO      | -          | -          |          |
| `<audio>`      | YES     | NO         | -          |          |
| `<b>`          | Yes     | Yes        | -          | Bold?    |
| `<bdi>`        | No      | -          | -          |          |
| `<bdo>`        | No      | -          | -          |          |
| `<big>`        | Yes     | No          | -          |          |
| `<br>`         | YES     | YES        | YES        | Line breaks|
| `<button>`     | Yes     | No         | -          |          |
| `<canvas>`     | No      | -          | -          |          |
| `<cite>`       | No      | -          | -          |          |
| `<code>`       | Yes     | Yes        | Yes        | DON'T    |
| `<data>`       | NO      | -          | -          |          |
| `<datalist>`   | NO      | -          | -          |          |
| `<del>`        | Yes     | Yes        | No         | strikethru |
| `<dfn>`        | Yes     | NO         | -          |          |
| `<em>`         | Yes     | Yes        | -          | italics   |
| `<embed>`      | Yes     | No         | -          |          |
| `<i>`          | Yes     | Yes        | -          | italics |
| `<iframe>`     | Yes     | No         | -          |        |
| `<img>`        | Yes     | Yes        |            | Inline CSS? |
| `<input>`      | No      | -          | -          |          |
| `<ins>`        | Yes     | Yes        |            | Underline |
| `<kbd>`        | Yes     | Yes        |            | Styling/Visual |
| `<label>`      | No      | -          | -          |          |
| `<map>`        | No      | -          | -          |          |
| `<mark>`       | Yes     | NO         | -          |          |
| `<meter>`      | No      | -          | -          |          |
| `<noscript>`   | No      | -          | -          |          |
| `<object>`     | No      | -          | -          |          |
| `<output>`     | No      | -          | -          |          |
| `<picture>`    | ?       | ?          | ?          | ?        |
| `<progress>`   | No      | -          | -          |          |
| `<q>`          | Yes     | Yes        |            | Not sure |
| `<ruby>`       | Yes     | Yes        | -          | DON'T    |
| `<s>`          | Yes     | Yes        | -          | strikethru |
| `<samp>`       | Yes     | Yes        |            | Monospaced font |
| `<script>`     | No      | -          | -          |          |
| `<select>`     | No      | -          | -          |          |
| `<slot>`       | No      | -          | -          |          |
| `<small>`      | Yes     | No         | -          |          |
| `<span>`       | Yes     | -          | -          | Why?     |
| `<strong>`     | Yes     | Yes        | -          | Bold     |
| `<sub>`        | Yes     | Yes        |            | Subscript |
| `<sup>`        | Yes     | Yes        |            | Subscript |
| `<svg>`        | Yes     | No         | -          |          |
| `<template>`   | No      | -          | -          |          |
| `<textarea>`   | No      | -          | -          |          |
| `<time>`       | Yes     | No         | -          |          |
| `<u>`          | Yes     | No         | -          |          |
| `<tt>`         | No      | -          | -          |          |
| `<var>`        | Yes     | Yes        | No         | ITALICS? |
| `<video>`      | Yes     | No         | -          |          |
| `<wbr>`        | No      | -          | -          |          | 

Testing `a` tag: _blank, and inline styles DID NOT WORK

<a href="https://google.com" target="_blank" style="text-decoration: overline underline; font-family: cursive">GOOGLE</a>

Testing `audio` tag: DID NOT DISPLAY

`b` and `strong` tags test: <br> ALL DISPLAYED
<b>Bold text</b> same as in **markdown** and how about <strong> the strong tag</strong>.

`code` tag test: SAME AS BACKTICKS 

This is a test of the <code>code tag</code> same as `backticks` I bet.

`del` & `s` tags test: BOTH WORKED

<del>Strikethrough text</del> same as in ~~markdown~~ and how about <s>the s tag</s>.

`dfn`, `em` and `i` tags test: EM and I WORKED, DFN DID NOT 

This is <em>em tag italics</em> same as in *markdown* and how about <i>the i tag</i> and <dfn>the dfn tag</dfn>.

`embed` tag test: DID NOT DISPLAY

`ins` and `u` tags test: u tag DID NOT WORK ins tag DID!

Will this <u>be displayed as underlined</u> and what about <ins>the ins tag</ins></u>?

`iframe` tag test: DID NOT DISPLAY

`mark` tag test: DID NOT DISPLAY

This is a <mark>mark tag</mark>, does it work?

`ruby` tag test: worked but no need

<ruby>
明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp>
</ruby>

`samp` tag test: WORKED

<p>This is regular text. <samp>Keyboard not found. Press F1 to continue</samp> and so is this.</p>

`small` and `big` tags test: DID NOT DISPLAY

<p>This is regular text. <small>The content is small</small>, but this isn't. This is <big>Big deprecated text</big></p>

`sub` and `sup` tags test: WORKED

H<sub>2</sub> and 2<sup>3</sup> and <sup>o</sup>7

`svg` tag test: DID NOT DISPLAY

`time` tag test: DID NOT WORK

<p>The Cure will be celebrating their 40th anniversary on <time datetime="2018-07-07">July 7</time> in London's Hyde Park.</p>

`var` tag test: ANOTHER VERSION OF ITALICS?

This is a <var>test of the var tag</var>, why would you use it?>

`video` tag test: DID NOT DISPLAY

`q` and `kbd` tags: WORKED

The <q>q tag wraps text in quotes</q>, the kbd tag wraps keyboard stull in a styled format like with <kbd>CTRL</kbd> or <kbd>SHIFT</kbd>.

## Block tags that worked

Duplicates markdown: `blockquote`, `h1` thru `h6`, `hr`, `ol` `ul` `li`, `pre`, `table`

Worked but unsure of use: address`, `details` with `summary`, `dl` `dt` `dd` (indent), `div`

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

## Inline tags that worked

Duplicates markdown:
`a`, `b` and `strong` (BOLD), `code`, `del` and `s` (Strikethrough), `em` and `i` and `var` (Italics), `img` (width, align [left, center, right])

Worked but unsure of use:
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
- `headings` for anchor links with html entities
- `br` for line breaks of paragrpah text like the `address` tag
- `img` to set width and height and align of center or right
- `ins` for underline
- `kbd` for keyboard chars or other keys
- `samp` for monospaced font
- `sup` and `sub` for super and subscript
- maybe `dl` `dt` `dd` for the indent definition type of style

Unless I can find inline styles or attributes that work with all of the above and/or the following: `blockquote`, `ol` `ul` `li`, `table`, `address`, or `a`.

## testing **double asterisks** and <b>the b tag</b> and the <strong>strong tag</strong>
<br><br>
<p align="center">Paragraph align="center", 2 br tags above</p>
<p align="right">Paragraph align="right"</p>
<div align="center">div align="center"</div>
<div align="right">div align="right"</div>

<h2 align="center"><ins>Centered h2</ins></h2>
<h2 align="right">Right h2</h2>

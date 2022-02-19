# HTML Tags that can be used in Markdown files

## Block level tags

28 tags

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<address>`    | Yes     | YES        | yes & no   | p tags directly below each other      |
| `<article>`    | NO      | skip       | -          | -        |
| `<aside>`      | NO      | skip       | -          | -        |
| `<blockquote>` | Yes     | YES        | Yes        | Inline CSS? |
| `<details>`    | Yes     | Yes        | Yes        | Not sure |
| `<dialog>`     | Yes     | NO         | -          | -        |
| `<dd>`         | Yes     | Yes        | Yes        | Indent   |
| `<div>`        | Yes     | Yes        | ?          | Styling? |
| `<dl>`         | Yes     | Yes        | Yes        | Indent   |
| `<dt>`         | Yes     | Yes        | Yes        | Indent   |
| `<fieldset>`   | NO      | -          | -          | -        |
| `<figcaption>` | Yes     | NO         | NO         | -        |
| `<figure>`     | Yes     | NO         | NO         | -        |
| `<footer>`     | NO      | skip       | -          | -        |
| `<form>`       | No      | skip       | -          | -        |
| h1-h6          | Yes     | Yes        | Yes        | Inline CSS? |
| `<header>`     | Yes     | Yes        | -          | -        |
| `<hgroup>`     | Yes     | skip       | -          | -        |
| `<hr>`         | Yes     | Yes        |            | diff sizes? |
| `<li>`         | Yes     |Yes         | Yes        | Inline CSS? |
| `<main>`       | NO      | skip       | -          | -        |
| `<nav>`        | NO      | skip       | -          | -        |
| `<ol>`         | Yes     | Yes        | Yes        | Inline CSS? |
| `<p>`          | Yes     | Yes        | Yes        | Inline CSS? |
| `<pre>`        | Yes     | Yes        | Yes        | DON'T    |
| `<section>`    | NO      | skip       | -          | -        |
| `<table>`      | Yes     | Yes        | Yes        | Inline CSS? |
| `<ul>`         | Yes     | Yes        | Yes        | Inline CSS  |

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

ol, li, ul tags check: all worked, inline css?
<ul>
  <li>unordered</li>
</ul>
<ol>
  <li>ordered</li>
</ol>

Pre tag check: exactly the same as code blocks
<pre>
  function testFx() {
    console.log("Hello");
  }
</pre>

Table tag test: inline css?
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
| `<b>`          | Yes     | Yes        | -          |          |
| `<bdi>`        | No      | -          | -          |          |
| `<bdo>`        | No      | -          | -          |          |
| `<big>`        | No      | -          | -          |          |
| `<br>`         | YES     | YES        | YES        | Line breaks|
| `<button>`     | Yes     | No         | -          |          |
| `<canvas>`     | No      | -          | -          |          |
| `<cite>`       | No      | -          | -          |          |
| `<code>`       | Yes     | Yes        | Yes        | DON'T    |
| `<data>`       | NO      | -          | -          |          |
| `<datalist>`   | NO      | -          | -          |          |
| `<del>`        | Yes     | Yes        | No         |          |
| `<dfn>`        | Yes     | Yes        | -          |          |
| `<em>`         | Yes     | Yes        | -          |          |
| `<embed>`      | Yes     | No         | -          |          |
| `<i>`          | Yes     | Yes        | -          |          |
| `<iframe>`     | Yes     | No         | -          |          |
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
| `<svg>`        | Yes | - | - | |
| `<template>`   | No      | -          | -          |          |
| `<textarea>`   | No      | -          | -          |          |
| `<time>`       | Yes | - | - | |
| `<u>`          | Yes | - | - | |
| `<tt>`         | No      | -          | -          |          |
| `<var>`        | Yes | Yes | No | ITALICS? |
| `<video>`      | - | - | - | |
| `<wbr>`        | - | - | - | | 

Testing `a` tag: _blank, and inline styles DID NOT WORK

<a href="https://google.com" target="_blank" style="text-decoration: overline underline; font-family: cursive">GOOGLE</a>

Testing `audio` tag: DID NOT DISPLAY
<audio controls>
  <source src="https://raw.githubusercontent.com/himalayasingh/music-player-1/master/music/4.mp3" type="audio/mp3">
  <!-- <source src="horse.mp3" type="audio/mpeg"> -->
  Your browser does not support the audio tag.
  <embed type="audio/mp3"
       src="https://raw.githubusercontent.com/himalayasingh/music-player-1/master/music/4.mp3"
       width="300"
       height="200">
</audio>

`b` and `strong` tags test: <br> ALL DISPLAYED
<b>Bold text</b> same as in **markdown** and how about <strong> the strong tag</strong>.

`code` tag test: SAME AS BACKTICKS 

This is a test of the <code>code tag</code> same as `backticks` I bet.

`del` & `s` tags test: BOTH WORKED

<del>Strikethrough text</del> same as in ~~markdown~~ and how about <s>the s tag</s>.

`dfn`, `em` and `i` tags test: EM and I WORKED, DFN DID NOT 

This is <em>em tag italics</em> same as in *markdown* and how about <i>the i tag</i> and <dfn>the dfn tag</dfn>.

`embed` tag test: DID NOT DISPLAY

<embed type="video/mp4"
src="https://player.vimeo.com/external/194837908.sd.mp4?s=c350076905b78c67f74d7ee39fdb4fef01d12420&profile_id=164"
width="300"
height="200">
<embed type="video/mp4"
src="https://player.vimeo.com/external/194837908.sd.mp4"
width="300"
height="200">

`ins` and `u` tags test: u tag DID NOT WORK ins tag DID!

Will this <u>be displayed as underlined</u> and what about <ins>the ins tag</ins></u>?

`iframe` tag test: DID NOT DISPLAY

<iframe id="inlineFrameExample"
    title="Inline Frame Example"
    width="300"
    height="200"
    src="https://www.openstreetmap.org/export/embed.html?bbox=-0.004017949104309083%2C51.47612752641776%2C0.00030577182769775396%2C51.478569861898606&layer=mapnik">
</iframe>

`mark` tag test: DID NOT DISPLAY

This is a <mark>mark tag</mark>, does it work?

`ruby` tag test: worked but no need

<ruby>
明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp>
</ruby>

`samp` tag test: DID NOT DISPLAY

<p>This is regular text. <samp>Keyboard not found. Press F1 to continue</samp> and so is this.</p>

`small` tag test: WORKED

<p>This is regular text. <small>The content is small</small>, but this isn't.</p>

`sub` and `sup` tags test:

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

<source src="https://player.vimeo.com/external/194837908.sd.mp4?s=c350076905b78c67f74d7ee39fdb4fef01d12420&profile_id=164"
        type="video/mp4">

Sorry, your browser doesn't support embedded videos.
</video>


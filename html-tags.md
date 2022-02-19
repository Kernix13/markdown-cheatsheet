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
         alt="Elephant at sunset" width="200px">
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
| `<a>`          | Yes     | Yes        |            | Target, Inline CSS?|
| `<abbr>`       | NO      | -          | -          |          |
| `<acronym>`    | NO      | -          | -          |          |
| `<audio>`      | YES     | NO         | -          |          |
| `<b>`          | Yes     | - | - | |
| `<bdi>`        | No      | -          | -          |          |
| `<bdo>`        | No      | -          | -          |          |
| `<big>`        | No      | -          | -          |          |
| `<br>`         | YES     | YES        | YES        | Line breaks|
| `<button>`     | Yes     | No         | -          |          |
| `<canvas>`     | No      | -          | -          |          |
| `<cite>`       | No      | -          | -          |          |
| `<code>`       | Yes     | - | - | |
| `<data>`       | - | - | - | |
| `<datalist>`   | - | - | - | |
| `<del>`        | Yes | Yes | No | |
| `<dfn>`        | - | - | - | |
| `<em>`         | - | - | - | |
| `<embed>`      | - | - | - | |
| `<i>`          | - | - | - | |
| `<iframe>`     | - | - | - | |
| `<img>`        | Yes | Yes | Inline CSS | |
| `<input>`      | - | - | - | |
| `<ins>`        | Yes | Yes | Underline | |
| `<kbd>`        | Yes | Yes | Styling/Visual | |
| `<label>`      | - | - | - | |
| `<map>`        | - | - | - | |
| `<mark>`       | - | - | - | |
| `<meter>`      | - | - | - | |
| `<noscript>`   | - | - | - | |
| `<object>`     | - | - | - | |
| `<output>`     | - | - | - | |
| `<picture>`    | - | - | - | |
| `<progress>`   | - | - | - | |
| `<q>`          | Yes | Yes | Not sure | |
| `<ruby>`       | - | - | - | |
| `<s>`          | - | - | - | |
| `<samp>`       | Yes | Yes | Monospaced font | |
| `<script>`     | - | - | - | |
| `<select>`     | - | - | - | |
| `<slot>`       | - | - | - | |
| `<small>`      | Yes | No | - | |
| `<span>`       | - | - | - | |
| `<strong>`     | - | - | - | |
| `<sub>`        | Yes | Yes | Subscript | |
| `<sup>`        | Yes | Yes | Superscript | |
| `<svg>`        | - | - | - | |
| `<template>`   | - | - | - | |
| `<textarea>`   | - | - | - | |
| `<time>`       | - | - | - | |
| `<u>`          | - | - | - | |
| `<tt>`         | - | - | - | |
| `<var>`        | Yes | Yes | No | |
| `<video>`      | - | - | - | |
| `<wbr>`        | - | - | - | | 

Testing a tag:

<a href="https://google.com" target="_blank" style="text-decoration: overline underline; font-family: cursive">GOOGLE</a>

Testing audio tag: did not display
<audio controls>
  <source src="https://raw.githubusercontent.com/himalayasingh/music-player-1/master/music/4.mp3" type="audio/mp3">
  <!-- <source src="horse.mp3" type="audio/mpeg"> -->
  Your browser does not support the audio tag.
</audio>

b tag test: <br>
<b>Bold?</b>

code tag test:

This is a test of the <code>code tag</code> same as `backticks` I bet.



# HTML Tags that can be used in Markdown files

## Block level tags

28 tags

| HTML Tag       | Tested? | Displayed? | Correctly? | Why Use? |
| ---------:     | :-----: | :--------: | :-------:  | :------: |
| `<address>`    | Yes     | NO         | no italics | -        |
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
| `<pre>`        | Yes     | Yes        | Yes        | Inline CSS? |
| `<section>`    | NO      | skip       | -          | -        |
| `<table>`      | Yes     | Yes        | Yes        | Inline CSS? |
| `<ul>`         | Yes     | Yes        | Yes        | Inline CSS  |

Address tag check
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
Dark side of the moon
130 miles away
Above Earth
Space

Blockquote tag check:
<blockquote cite="https://www.huxley.net/bnw/four.html">
    <p>Words can be like X-rays, if you use them properly—they’ll go through anything. You read and you’re pierced.</p>
</blockquote>

> Words can be like X-rays, if you use them properly—they’ll go through anything. You read and you’re pierced.

dialog tag check
<dialog open>
  <!-- <p>Need br tags</p> -->
  Need br tags
</dialog><br><br><br>

Figure, img, and figcaption tags check
<figure>
    <img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg"
         alt="Elephant at sunset" width="200px">
    <figcaption>An artistic eye but does it wrap when exceeds the length of the image? With figure element</figcaption>
</figure>
<img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg" alt="Elephant at sunset" width="200px">
<figcaption>An artistic eye but does it wrap when exceeds the length of the image? Without figure element</figcaption>
<img src="https://kernixwebdesign.com/wp-content/uploads/2022/01/graphic-design-tips.jpg" alt="Elephant at sunset" width="200px">
<!-- <br> -->
An artistic eye but does it wrap when exceeds the length of the image? Without figure  and figcaptionelement


Headings and hgroup tag check
<hgroup>
  <h1>one</h1>
  <h2>two: no auto horiz rule???</h2>
  <h3>three</h3>
  <h4>four</h4>
  <h5>five</h5>
  <h6>six</h6>
</hgroup>

ol, li, ul tags check
<ul>
  <li>unordered</li>
</ul>
<ol>
  <li>ordered</li>
</ol>

Pre tag check
<pre>
  function testFx() {
    console.log("Hello");
  }
</pre>

## Inline tags

55 tags

| HTML Tag     | Tested? | Works? | Why Use? |
| ---------:   | :-----: | :----: | :-----:  | 
| `<a>`          | Yes | Yes | Inline CSS |
| `<abbr>`       | - | - | - |
| `<acronym>`    | - | - | - |
| `<audio>`      | - | - | - |
| `<b>`          | - | - | - |
| `<bdi>`        | - | - | - |
| `<bdo>`        | - | - | - |
| `<big>`        | - | - | - |
| `<br>`         | - | - | - |
| `<button>`     | Yes | No | - |
| `<canvas>`     | - | - | - |
| `<cite>`       | - | - | - |
| `<code>`       | - | - | - |
| `<data>`       | - | - | - |
| `<datalist>`   | - | - | - |
| `<del>`        | Yes | Yes | No |
| `<dfn>`        | - | - | - |
| `<em>`         | - | - | - |
| `<embed>`      | - | - | - |
| `<i>`          | - | - | - |
| `<iframe>`     | - | - | - |
| `<img>`        | Yes | Yes | Inline CSS |
| `<input>`      | - | - | - |
| `<ins>`        | Yes | Yes | Underline |
| `<kbd>`        | Yes | Yes | Styling/Visual |
| `<label>`      | - | - | - |
| `<map>`        | - | - | - |
| `<mark>`       | - | - | - |
| `<meter>`      | - | - | - |
| `<noscript>`   | - | - | - |
| `<object>`     | - | - | - |
| `<output>`     | - | - | - |
| `<picture>`    | - | - | - |
| `<progress>`   | - | - | - |
| `<q>`          | Yes | Yes | Not sure |
| `<ruby>`       | - | - | - |
| `<s>`          | - | - | - |
| `<samp>`       | Yes | Yes | Monospaced font |
| `<script>`     | - | - | - |
| `<select>`     | - | - | - |
| `<slot>`       | - | - | - |
| `<small>`      | Yes | No | - |
| `<span>`       | - | - | - |
| `<strong>`     | - | - | - |
| `<sub>`        | Yes | Yes | Subscript |
| `<sup>`        | Yes | Yes | Superscript |
| `<svg>`        | - | - | - |
| `<template>`   | - | - | - |
| `<textarea>`   | - | - | - |
| `<time>`       | - | - | - |
| `<u>`          | - | - | - |
| `<tt>`         | - | - | - |
| `<var>`        | Yes | Yes | No |
| `<video>`      | - | - | - |
| `<wbr>`        | - | - | - |
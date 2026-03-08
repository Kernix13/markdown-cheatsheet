# How does a README or GitHub repo show up in the SERPS?

I recently read an article about accessible GitHub profile READMEs which will help with your profiles being discovered. I sometimes see GitHub repos in the Search Engine Results Pages (SERPS) but never thought about how they appear in the SERPS. That got me wondering:

> "_How can I get my repos/READMEs to show up in Google searches?_"

One answer would be to make the README accessible. See [5 tips for making your GitHub profile page accessible](https://github.blog/developer-skills/github/5-tips-for-making-your-github-profile-page-accessible/) for examples on that. But you should also optimize your repo and README for SEO.

## SEO parameters + tools

> [!NOTE]
> The hard values are from the guidelines given to me while working for The HOTH (list items 1-4).

<div align="center">hello</div>

1. SEO Title: 50-60 characters ideally but up to 70 is okay, 50-55 for mobile
2. SEO/Meta Description: 120-158 characters, closer to 120 for mobile
3. Keyword Search Volume: should be >= 100
4. Keyword Density: should be 1-2% (# of times KW appears) / (total # of words)
5. Primary Keyword = "User Intent"
6. All keywords (primary + secondary) have to match the user intent
7. [Capitalize My Title](https://capitalizemytitle.com/): Use this site to properly capitalize your README h1 title
8. [wordcounter.net](https://wordcounter.net/): Use a site like this to get the character & word count for your h1 heading and your "_meta description_".

## Optimize content for the GitHub Explore section

1. Repository Name: High importance (primary keyword location)
2. About Section (Description): High importance
3. Topics/Tags: High importance
4. README Content: Medium importance for GitHub Explore, High for Google
5. Stars, Watchers, Forks: High importance for Explore, Low/Medium for Google

### Optimize Repository Name, Description, and Topics

- Include a primary keyword in the repository name
- Start the "About" description with your main keyword and keep it short and specific, explaining what the project does
- Add relevant topics/tags, use specific terms

### Create a High-Quality README

- Use clear headings (H1, H2, H3) to structure your content
- Incorporate relevant keywords naturally throughout the text, especially in headings and the first paragraph
- Add images or GIFs with keyword-rich alt text
- Provide clear instructions on how to install/use the project and include code examples and badges
- Add a clear call-to-action (CTA) encouraging users to star the project or contribute

### Leverage GitHub Pages

- If using GitHub Pages, make sure your site is mobile-friendly & fast-loading
- Add [Twitter cards](https://www.oncrawl.com/general-seo/a-complete-guide-to-twitter-cards/) and [Open Graph](https://ogp.me/) elements

### Build External Presence (Off-Page SEO)

- Share your repository on developer-focused platforms like Dev.to, Medium, and Reddit in relevant communities
- Link to your repository from your personal website, blog posts, or social media profiles
- Engage in communities by answering questions and providing support

### Use Google Search Console

- Add your GitHub GitHub Page(s) URL or Live Deploy URL to Google Search Console
- Use the "URL Inspection" tool to request indexing for new or updated pages

### How to check if your repo is indexed

- `site:github.com/yourusername/repo-name`
- If results appear, Google has indexed it

## ChatGPT reasons for repos ranking in the SERPs

### 1. The Repository Name (Huge Ranking Factor)

The repo name often becomes the page title, which Google heavily weights.

The actual `<title>` is:

- `username/repo_name: Sidebar About text`

### 2. README Content (The Main SEO Content)

The README.md file is essentially the page content Google indexes. Have a keyword rich titled followed by a "no-title" intro of 1-2 paragraphs. MAke your first paragraph short enough for a meta description with the keyword phrase.

Repos with long, well-written READMEs rank better because they contain:

- Clear descriptions
- Keywords
- Installation instructions
- Examples
- Use cases

**You generally should not put an image before the intro paragraph**.

High-Ranking GitHub README Structure:

```md
# Project Name – short descriptive subtitle

Badges (optional)

Intro paragraph (VERY important for SEO)

Screenshot / GIF demo

## Features

## Demo / Live Site

## Installation

## Usage

## API (if applicable)

## Project Structure

## Technologies Used

## Contributing

## License
```

### 3. Stars, Forks, and Watchers (Popularity Signals)

GitHub popularity acts like social proof signals. GitHub interprets these as authority signals, Google does not. High-star repos often dominate SERPs.

### 4. External Links (Huge SEO Signal)

Google sees it as authoritative if people link to the repo from:

- blogs
- documentation
- Stack Overflow or other dev sites
- tutorials

Many popular repos get thousands of backlinks.

### 5. meta description

- `Sidebar About text - username/reponame`

That is being replaced by Google by related text in the README so have a "no-title" intro below your `H1` descibing your project but make sure to place your keywords early in the text.

### 6. About text (Sidebar)

Include your core keywords and not much else in the About section.

### 7. Topics

Have sidebar topics related to your SEO keywords and be specific: Expressjs, React, CSS Grid, etc. + other related topics

## Image tips for better SEO

What high-quality repos usually do - They:

- Add screenshots to the repo
- Compress them
- Serve optimized images - Use WebP if possible
- UI screenshot -> 150–400 KB
- small feature image -> 80–200 KB

PNG to WebP conversion!!!

Task Lists - Replace with a normal list so that you do not get an error of "_Form elements do not have associated labels_"

Squoosh: conversion to WebP and optimization

- drag screenshot into Squoosh
- select WebP
- compression ~ 75–85
- download optimized image

## SEO Tips

1. Use a markdown to HTML conversion tool to convert your README to HTML
   - load the HTML version with Live Server
   - Run a Lighthouse report and look at the errors/warnings for SEO & Accessibility
   - Make all the changes you have control over
2. Download ans install Local WP
3. create a simple 1 page WordPress site with a block theme
4. copy/paste your HTML (inside the `<body>` tag) and add it to a Custom HTML block
5. Add an SEO plugin to the WordPress install (RankMath)
   - Add your SEO keyword phrase and make changes to the text/HTML based on what the plugin recommends
   - This will make sure your README text has the right % of Keywords and other related SEO & Accessibility factors
6. Install an accessibility plugin (Equalize Digital Accessibility Checker)
   - this may show accessibility issues that Lightthouse missed
7. You could opt to install the chrome extension [WAVE Web Accessibility Evaluation Tools](https://wave.webaim.org/extension/) and look at the issues and errors.

NOTE: Don't use task lists because Lighthouse flags them for not having labels

## SEO Checklist

1. Rewrite H1/Title
2. Add or rewrite intro paragraph
3. Add or rewrite About section
4. Ensure quality topics
5. Convert markdown to HTML
6. Run SEO & Accessibility analysis on the HTML version
7. Update markdown

<!--
## Checklist for this repo:

1. Rewrite H1/Title ✅
2. Add or rewrite intro paragraph ✅
3. Rewrite About section ✅
4. Ensure quality topics ✅
5. Convert markdown to HTML 📌
6. Run SEO & Accessibility analysis on the HTML version 📌
7. Update markdown 📌

Repos to-do:

- codeCompare
- what-chord-is-this
- beginner-git-commands
- personal-portfolio
- guitar-chord-names
- typescript-virtual-keyboard or WriterAssist
- tarp-configs
- github-actions-dotfiles?

-->

<!--

README SEO analyzer project idea: (NO LONGER INTERESTED IN THIS)
1. User enters main keyword phrase
2. User enters repo slug/name
3. User enters README text
4. User enters README H1 text
5. User enters README intro paragraph text
6. User enters sidebar about text

Do calculations and analysis for the SEO:
- Is keyword phrase in repo name?
- Is keyword phrase in H1 text?
- Is keyword phrase in intro pragraph text
- Is keyword phrase in About text text
- Get character count for H1 text
- Get character count for opening intro text
- Get word count for README
- Is README word count at least 300 words?
- Count occurrences in README for keyword phrase
- Calculate keyword density, KD: (Keyword occurrences) / (Word count)
  - Recommend KD is 0.5-2% or 0.5-1%
- Simulate what the search result might look like

Do an accessibility analysis:
1. Parse all README links
   - Do links have descriptive text?
2. Parse images
   - Do the images have alt text?
   - Is the alt text SEO rich?
   - Is the alt text too short (<5 words)?
3. Parse all headings
   - Are the headings sequential or out of order?
4. Parse list items
   - Do list items use proper markup (-, *, 1., etc) or are emojis being used?

RegEx:
- Extract All Headings: ^(#{1,6})\s(.+)
- capture the heading text: ^#\s(.+)
- Extract Images: !\[(.*?)\]\((.*?)\)
- Image alt text: !\[(.*?)\]\( and/or <img[^>]*alt=["'](.*?)["']
- Extract Links: \[(.*?)\]\((.*?)\)

Profile Readme tips:

# Jim Kernicky – Web Designer & Developer
The first few lines of your README act like the meta description for your profile. Include:

- Your roles/titles: web designer, WordPress developer, front-end developer, etc.
- Skills or technologies people might search for: WordPress, HTML/CSS, SEO-friendly websites, UI/UX, etc.
- Your value proposition: what you do for clients or projects.

Optional SEO Enhancements

- Include keywords naturally in sections like “About Me,” “Skills,” or “Projects.”
- Pin repositories that show your expertise in those skills. Google sometimes surfaces repos alongside your profile.
- Add a short tagline in your GitHub bio (the small text under your avatar) with keywords:

-->

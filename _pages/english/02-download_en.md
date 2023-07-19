---
title: Download
layout: splash_en
permalink: /en/download
header:
    overlay_image: /images/headers/home_header.webp
    overlay_filter: rgba(0, 0, 0, 0.6)
excerpt: "All available req42 templates for download - [various formats](#overview-of-different-formats) for different tools."
---

# File-based formats

These formats are generated from the [req42 GitHub repository](https://github.com/Hruschka/req42-framework/).

{% assign PREFIX = "https://github.com/Hruschka/req42-framework/raw/main/dist/req42-framework-" %}
{% assign formats = "asciidoc|docbook|docx|epub|markdown|markdownMP|markdownMPStrict|markdownStrict|gitHubMarkdown|gitHubMarkdownMP|html|latex|rst|textile" | split: "|"  %}
{% assign types = "plain|withhelp" | split: "|"  %}

| Format | Language | Without explanations | With explanations for each section |
|--------|----------|-------|-----------|
{% for format in formats %}| {{ format }} | EN | {% for type in types %} [.zip]({{PREFIX}}EN-{{type}}-{{format}}.zip)|{% endfor %}
|  | DE | {% for type in types %} [.zip]({{PREFIX}}DE-{{type}}-{{format}}.zip) |{% endfor %}
{% endfor %}

<br><br>

# Overview of different formats

- **asciidoc**: A powerful yet simple markup language commonly used for architecture documentation.

- **docbook**: An XML-based document format often used for technical documentation and books.

- **docx**: A Microsoft Word document format that can be used with LibreOffice or OpenOffice.

- **epub**: A widely adopted format for e-books based on open standards, readable on various e-book readers and platforms.

- **markdown**: A widely used and straightforward markup language, originally documented by its creator.

- **markdownMP**: The same format as "markdown" above, but each section is in its own file.

- **markdownMPStrict**: A restricted version of the "markdownMP" markup language, documented by its creator.

- **markdownStrict**: A restricted version of the general Markdown syntax, documented by its creator.

- **gitHubMarkdown**: A variant of Markdown used on [github.com](https://github.com/) and GitHub Enterprise.

- **gitHubMarkdownMP**: The same format as "gitHubMarkdown" above, but each section is in its own file.

- **html**: Used for display purposes only, not for editing.

- **latex**: A comprehensive document preparation system often used by individuals who value aesthetics and are willing to put in some effort.

- **rst**: ReStructuredText, a markup language commonly used by ReadTheDocs and in the Python world.

- **textile**: Another simple markup language, documented at [textile-lang.com](https://textile-lang.com/).

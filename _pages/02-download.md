---
title: Download
layout: splash
permalink: /download
header:
    overlay_image: /images/headers/framework_header.webp
    overlay_filter: rgba(0, 0, 0, 0.6)
excerpt: "Alle verfügbaren req42-Templates zum Download - verschiedene Formate für verschiedene Tools"
---

# Filebasierte Formate

Diese Formate werden auf der Grundlage ihrer AsciiDoc-Quellen aus dem [Github-Repository](https://github.com/Hruschka/req42-framework/) generiert.

{% assign PREFIX = "https://github.com/Hruschka/req42-framework/raw/main/dist/req42-framework-" %}
{% assign formats = "asciidoc|docbook|docx|epub|markdown|markdownMP|markdownMPStrict|markdownStrict|gitHubMarkdown|gitHubMarkdownMP|html|latex|rst|textile|textile2" | split: "|"  %}  
{% assign types = "plain|withhelp" | split: "|"  %}

| Format | Sprache | Ohne Erklärungen | Mit Erklärungen für jeden Abschnitt |
|--------|----------|-------|-----------| 
{% for format in formats %}| {{ format }} | EN | {% for type in types %} [.zip]({{PREFIX}}EN-{{type}}-{{format}}.zip)|{% endfor %}
|  | DE | {% for type in types %} [.zip]({{PREFIX}}DE-{{type}}-{{format}}.zip) |{% endfor %}
{% endfor %}


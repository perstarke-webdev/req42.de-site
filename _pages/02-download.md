---
title: Download
layout: splash
permalink: /download
header:
    overlay_image: /images/headers/home_header.webp
    overlay_filter: rgba(0, 0, 0, 0.6)
excerpt: "Alle verfügbaren req42-Templates zum Download - [verschiedene Formate](/download#übersicht-der-verschiedenen-formate) für verschiedene Tools"
---

# Filebasierte Formate

Diese Formate werden aus dem [req42-Github-Repository](https://github.com/Hruschka/req42-framework/) generiert.

{% assign PREFIX = "https://github.com/Hruschka/req42-framework/raw/main/dist/req42-framework-" %}
{% assign formats = "asciidoc|docbook|docx|epub|markdown|markdownMP|markdownMPStrict|markdownStrict|gitHubMarkdown|gitHubMarkdownMP|html|latex|rst|textile" | split: "|"  %}  
{% assign types = "plain|withhelp" | split: "|"  %}

| Format | Sprache | Ohne Erklärungen | Mit Erklärungen für jeden Abschnitt |
|--------|----------|-------|-----------| 
{% for format in formats %}| {{ format }} | EN | {% for type in types %} [.zip]({{PREFIX}}EN-{{type}}-{{format}}.zip)|{% endfor %}
|  | DE | {% for type in types %} [.zip]({{PREFIX}}DE-{{type}}-{{format}}.zip) |{% endfor %}
{% endfor %}

<br><br>

# Übersicht der verschiedenen Formate

- **asciidoc**: Eine leistungsstarke und dennoch einfache Auszeichnungssprache, die häufig für Architekturdokumentationen verwendet wird.

- **docbook**: Ein XML-basiertes Dokumentenformat, das oft für technische Dokumentationen und Bücher genutzt wird.

- **docx**: Ein Microsoft Word-Dokumentformat, das mit LibreOffice oder OpenOffice verwendet werden kann.

- **epub**: Ein weit verbreitetes Format für E-Books, das auf offenen Standards basiert und auf verschiedenen E-Book-Readern und -Plattformen gelesen werden kann.

- **markdown**: Eine weit verbreitete und einfache Auszeichnungssprache, ursprünglich vom Erfinder dokumentiert.

- **markdownMP**: Das gleiche Format wie "markdown" oben, aber jeder Abschnitt befindet sich in seiner eigenen Datei.

- **markdownMPStrict**: Eine eingeschränkte Version der "markdownMP"-Auszeichnungssprache, dokumentiert vom Erfinder.

- **markdownStrict**: Eine eingeschränkte Version der allgemeinen Markdown-Syntax, dokumentiert vom Erfinder.

- **gitHubMarkdown**: Eine Variante von Markdown, die auf GitHub.com und GitHub Enterprise verwendet wird.

- **gitHubMarkdownMP**: Das gleiche Format wie "gitHubMarkdown" oben, aber jeder Abschnitt befindet sich in seiner eigenen Datei.

- **html**: Wird nur zur Anzeige der Vorlage verwendet, nicht zur Bearbeitung.

- **latex**: Ein umfassendes Dokumentenvorbereitungssystem, das oft von Personen verwendet wird, die Wert auf Schönheit legen und bereit sind, einige Anstrengungen zu unternehmen.

- **rst**: ReStructuredText, eine Auszeichnungssprache, die häufig von ReadTheDocs und in der Python-Welt verwendet wird.

- **textile**: Eine weitere einfache Auszeichnungssprache, dokumentiert auf [textile-lang.com](https://textile-lang.com/).

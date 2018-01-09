# ✂️ Save time with some snippets!

Here are some useful snippets for writing posts for Alligator.io. Each snippet has a version for Atom, VS Code and Sublime Text. Sorry VI users 😆!

Thanks to [this snippet generator](https://github.com/pawelgrzybek/snippet-generator) for making it!

## Table of contents

* [Jekyll front matter](#jekyll-front-matter)
  * [Atom](#atom)
  * [VS Code](#vs-code)
  * [Sublime Text](#sublime-text)
* [Bullet points](#bullet-points)
  * [Atom](#atom-1)
  * [VS Code](#vs-code-1)
  * [Sublime Text](#sublime-text-1)
* [Code snippets](#code-snippets)
  * [Atom](#atom-2)
  * [VS Code](#vs-code-2)
  * [Sublime Text](#sublime-text-2)
* [Raw](#raw)
  * [Atom](#atom-3)
  * [VS Code](#vs-code-3)
  * [Sublime Text](#sublime-text-3)
* [Single-line Code Annotation](#single-line-code-annotation)
  * [Atom](#atom-4)
  * [VS Code](#vs-code-4)
  * [Sublime Text](#sublime-text-4)
* [Block Code Annotation](#block-code-annotation)
  * [Atom](#atom-5)
  * [VS Code](#vs-code-5)
  * [Sublime Text](#sublime-text-5)
* [Info Box](#info-box)
  * [Atom](#atom-6)
  * [VS Code](#vs-code-6)
  * [Sublime Text](#sublime-text-6)
* [Warning Box](#warning-box)
  * [Atom](#atom-7)
  * [VS Code](#vs-code-7)
  * [Sublime Text](#sublime-text-7)
* [Success Box](#success-box)
  * [Atom](#atom-8)
  * [VS Code](#vs-code-8)
  * [Sublime Text](#sublime-text-8)
* [File Description](#file-description)
  * [Atom](#atom-9)
  * [VS Code](#vs-code-9)
  * [Sublime Text](#sublime-text-9)
* [Post Image](#post-image)
  * [Atom](#atom-10)
  * [VS Code](#vs-code-10)
  * [Sublime Text](#sublime-text-10)
* [Lazy Post Image](#lazy-post-image)
  * [Atom](#atom-11)
  * [VS Code](#vs-code-11)
  * [Sublime Text](#sublime-text-11)
* [Collapsible](#collapsible)
  * [Atom](#atom-12)
  * [VS Code](#vs-code-12)
  * [Sublime Text](#sublime-text-12)
* [Parting Thoughts](#parting-thoughts)
  * [Atom](#atom-13)
  * [VS Code](#vs-code-13)
  * [Sublime Text](#sublime-text-13)

## Jekyll front matter

### Atom

```
'Jekyll front matter':
  'prefix': 'frontmatter'
  'body': """
    ---
    layout: page-fullwidth
    title:  "${1:Using JavaScript to Make Crispy Bacon}"
    categories:
        - ${2:JS}
    tags:
        - ${3:bacon}
    header: no
    breadcrumb: true
    meta_description: "${4:Description in the range of 80 to 155 characters.}"
    author: ${5:john_d}
    ---
  """
```

### VS Code

```
"Jekyll front matter": {
  "prefix": "frontmatter",
  "body": [
    "---",
    "layout: page-fullwidth",
    "title:  \"${1:Using JavaScript to Make Crispy Bacon}\"",
    "categories:",
    "    - ${2:JS}",
    "tags:",
    "    - ${3:bacon}",
    "header: no",
    "breadcrumb: true",
    "meta_description: \"${4:Description in the range of 80 to 155 characters.}\"",
    "author: ${5:john_d}",
    "---"
  ],
  "description": "Jekyll front matter"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
---
layout: page-fullwidth
title:  "${1:Using JavaScript to Make Crispy Bacon}"
categories:
    - ${2:JS}
tags:
    - ${3:bacon}
header: no
breadcrumb: true
meta_description: "${4:Description in the range of 80 to 155 characters.}"
author: ${5:john_d}
---
]]></content >
  <description>Jekyll front matter</description>
  <tabTrigger>frontmatter</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Bullet points

### Atom

```
'Bullet Point':
  'prefix': 'bullet'
  'body': """
    * *${1:Point 1}*: ${2:Text for point 1}
  """
```

### VS Code

```
"Bullet Point": {
  "prefix": "bullet",
  "body": [
    "* *${1:Point 1}*: ${2:Text for point 1}"
  ],
  "description": "Bullet Point"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
* *${1:Point 1}*: ${2:Text for point 1}
]]></content >
  <description>Bullet Point</description>
  <tabTrigger>bullet</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Code snippets

### Atom

```
'Code snippet':
  'prefix': 'snippet'
  'body': """
    <pre><code class="${1:language or 'nohighlight'}">${2:your code here}</code></pre>
  """
```

### VS Code

```
"Code snippet": {
  "prefix": "snippet",
  "body": [
    "<pre><code class=\"${1:language or 'nohighlight'}\">${2:your code here}</code></pre>"
  ],
  "description": "Code snippet"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<pre><code class="${1:language or 'nohighlight'}">${2:your code here}</code></pre>
]]></content >
  <description>Code snippet</description>
  <tabTrigger>snippet</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Raw

Liquid tags to escape mustache syntax:

### Atom

```
'Raw':
  'prefix': 'raw'
  'body': """
    {% raw %}${1:your mustache-escaped content here}{% endraw %}
  """
```

### VS Code

```
"Raw": {
  "prefix": "raw",
  "body": [
    "{% raw %}${1:your mustache-escaped content here}{% endraw %}"
  ],
  "description": "Raw"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
{% raw %}${1:your mustache-escaped content here}{% endraw %}
]]></content >
  <description>Raw</description>
  <tabTrigger>raw</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Single-line Code Annotation

### Atom

```
'annotation':
  'prefix': 'annotation'
  'body': """
    <span class="code-annotation">${1:your annotated code}</span>
  """
```

### VS Code

```
"annotation": {
  "prefix": "annotation",
  "body": [
    "<span class=\"code-annotation\">${1:your annotated code}</span>"
  ],
  "description": "annotation"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<span class="code-annotation">${1:your annotated code}</span>
]]></content >
  <description>annotation</description>
  <tabTrigger>annotation</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Block Code Annotation

### Atom

```
'Block annotation':
  'prefix': 'block-annotation'
  'body': """
    <span class="block-annotation">${1:your annotated block}</span>
  """
```

### VS Code

```
"Block annotation": {
  "prefix": "block-annotation",
  "body": [
    "<span class=\"block-annotation\">${1:your annotated block}</span>"
  ],
  "description": "Block annotation"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<span class="block-annotation">${1:your annotated block}</span>
]]></content >
  <description>Block annotation</description>
  <tabTrigger>block-annotation</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Info Box

### Atom

```
'Info box':
  'prefix': 'info-box'
  'body': """
    <p class="info-box">
      ${1:content here}
    </p>
  """
```

### VS Code

```
"Info box": {
  "prefix": "info-box",
  "body": [
    "<p class=\"info-box\">",
    "  ${1:content here}",
    "</p>"
  ],
  "description": "Info box"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<p class="info-box">
  ${1:content here}
</p>
]]></content >
  <description>Info box</description>
  <tabTrigger>info-box</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Warning Box

### Atom

```
'Warning box':
  'prefix': 'warning-box'
  'body': """
    <p class="info-box warning">
      ${1:content here}
    </p>
  """
```

### VS Code

```
"Warning box": {
  "prefix": "warning-box",
  "body": [
    "<p class=\"info-box warning\">",
    "  ${1:content here}",
    "</p>"
  ],
  "description": "Warning box"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<p class="info-box warning">
  ${1:content here}
</p>
]]></content >
  <description>Warning box</description>
  <tabTrigger>warning-box</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Success Box

### Atom

```
'Success box':
  'prefix': 'success-box'
  'body': """
    <p class="info-box success">
      ${1:content here}
    </p>
  """
```

### VS Code

```
"Success box": {
  "prefix": "success-box",
  "body": [
    "<p class=\"info-box success\">",
    "  ${1:content here}",
    "</p>"
  ],
  "description": "Success box"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<p class="info-box success">
  ${1:content here}
</p>
]]></content >
  <description>Success box</description>
  <tabTrigger>success-box</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## File Description

### Atom

```
'File description':
  'prefix': 'file-description'
  'body': """
    <p class="file-desc"><span>${1:file-name.js}</span></p>
  """
```

### VS Code

```
"File description": {
  "prefix": "file-description",
  "body": [
    "<p class=\"file-desc\"><span>${1:file-name.js}</span></p>"
  ],
  "description": "File description"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<p class="file-desc"><span>${1:file-name.js}</span></p>
]]></content >
  <description>File description</description>
  <tabTrigger>file-description</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Post Image

### Atom

```
'image':
  'prefix': 'post-image'
  'body': """
    <p class="text-center">
     <img src="${1:relative path}" width="${2:width}" height="${3:height}" class="slight-shadow" alt="${4:image description}">
    </p>
  """
```

### VS Code

```
"image": {
  "prefix": "post-image",
  "body": [
    "<p class=\"text-center\">",
    " <img src=\"${1:relative path}\" width=\"${2:width}\" height=\"${3:height}\" class=\"slight-shadow\" alt=\"${4:image description}\">",
    "</p>"
  ],
  "description": "image"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<p class="text-center">
 <img src="${1:relative path}" width="${2:width}" height="${3:height}" class="slight-shadow" alt="${4:image description}">
</p>
]]></content >
  <description>image</description>
  <tabTrigger>post-image</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Lazy Post Image

### Atom

```
'Lazy image':
  'prefix': 'post-image-lazy'
  'body': """
    <p class="text-center">
     <img data-original="${1:relative path}" width="${2:width}" height="${3:height}" class="slight-shadow" alt="${4:image description}">
    </p>
  """
```

### VS Code

```
"Lazy image": {
  "prefix": "post-image-lazy",
  "body": [
    "<p class=\"text-center\">",
    " <img data-original=\"${1:relative path}\" width=\"${2:width}\" height=\"${3:height}\" class=\"slight-shadow\" alt=\"${4:image description}\">",
    "</p>"
  ],
  "description": "Lazy image"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<p class="text-center">
 <img data-original="${1:relative path}" width="${2:width}" height="${3:height}" class="slight-shadow" alt="${4:image description}">
</p>
]]></content >
  <description>Lazy image</description>
  <tabTrigger>post-image-lazy</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Collapsible

### Atom

```
'Collapsible':
  'prefix': 'collapsible'
  'body': """
    <gator-collapse title="${1:title here}">
      <p>${2:content here}</p>
    </gator-collapse>
  """
```

### VS Code

```
"Collapsible": {
  "prefix": "collapsible",
  "body": [
    "<gator-collapse title=\"${1:title here}\">",
    "  <p>${2:content here}</p>",
    "</gator-collapse>"
  ],
  "description": "Collapsible"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<gator-collapse title="${1:title here}">
  <p>${2:content here}</p>
</gator-collapse>
]]></content >
  <description>Collapsible</description>
  <tabTrigger>collapsible</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

## Parting Thoughts

### Atom

```
'Parting thoughts':
  'prefix': 'parting-thoughts'
  'body': """
    <p class="t70 text-center">
      ${1:your text here}
    </p>
  """
```

### VS Code

```
"Parting thoughts": {
  "prefix": "parting-thoughts",
  "body": [
    "<p class=\"t70 text-center\">",
    "  ${1:your text here}",
    "</p>"
  ],
  "description": "Parting thoughts"
}
```

### Sublime Text

```
<snippet>
  <content><![CDATA[
<p class="t70 text-center">
  ${1:your text here}
</p>
]]></content >
  <description>Parting thoughts</description>
  <tabTrigger>parting-thoughts</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope >source.python</scope > -->
</snippet >
```

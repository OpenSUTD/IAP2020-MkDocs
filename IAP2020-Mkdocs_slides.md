---
marp: true
title: "IAP 2020: Introduction to Markdown and MkDocs"
theme: uncover
class: invert
paginate: false
---

# Introduction to

![invert width:700px](https://user-images.githubusercontent.com/48215474/71895190-3e3fdb00-3148-11ea-8c15-c2bfbf635f56.png)
<br>
Wei Min Cher

09 January 2020

![saturate:5.0 contrast: 100% height:100px drop-shadow:0,5px,10px,rgba(255,255,255)](https://3dcdsc.github.io/3DC-IAP-Conference-Working-Title/img/logowith3DC.png)

---

<!-- paginate: true -->
<!-- footer: IAP 2020: Introduction to Markdown and MkDocs -->

# Contents

- Markdown
- GitHub Flavored Markdown
- Typora
- Pandoc
- Mkdocs

---

![invert width:300px](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/800px-Markdown-mark.svg.png)

# Markdown

- Lightweight markup language
- Can be converted to many formats

---

![invert](https://avatars0.githubusercontent.com/u/8653968?s=200&v=4)

# GitHub Flavored Markdown

---

# Markdown Editor

- GitHub Gist
- Stackedit.io

---

# Headers

<br>

`# This is an h1 tag`
`## This is an h2 tag`
`###### This is an h6 tag`

---

# This is an h1 tag

## This is an h2 tag

###### This is an h6 tag

---

# Emphasis

<br>

`*This will be italic*` `_This will also be italic_`

`**This will be bold**` `__This will also be bold__`
<br>
`_You **can** combine them_`

---

_This will be italic_ _This will also be italic_
**This will be bold** **This will also be bold**
_You **can** combine them_

---

# Unordered Lists

```text
* Item 1
* Item 2
  * Item 2a
  * Item 2b
```

---

- Item 1
- Item 2
  - Item 2a
  - Item 2b

---

## Ordered Lists

```text
1. Item 1
2. Item 2
3. Item 3
  i. Item 3a
  ii. Item 3b
```

---

1. Item 1
2. Item 2
3. Item 3
   i. item 3a
   ii. item 3b

---

# Links

<br>

`http://github.com`
`[GitHub](http://github.com)`

---

http://github.com
[GitHub](http://github.com)

---

# Images

<br>

`![SUTD Logo](https://www.sutd.edu.sg/assets/sutd/img/logo-white.png)`

---

![invert width:500px](https://upload.wikimedia.org/wikipedia/en/thumb/f/f4/Singapore_University_of_Technology_and_Design_logo.svg/1280px-Singapore_University_of_Technology_and_Design_logo.svg.png)

---

# Tables

```text
First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```

---

![table height:300px](https://user-images.githubusercontent.com/48215474/71899032-c5924c00-3152-11ea-83fe-5d7de4c941b5.jpg)

---

# Activity 1 (10 mins)

- Make a to-do list with 3 categories
  1. To do
  2. In progress
  3. Done

---

```text
#### To do

1. Pray for good fortune

- Temple
- Bell curve god

##### In progress

1. Catching up on **_SLEEP_**

###### Done

1. School
```

---

#### To do

1. Pray for good fortune

- Temple
- Bell curve god

##### In progress

1. Catching up on **_SLEEP_**

###### Done

1. School

---

# Inline code

```text
I think you should use an `<addr>` element here instead.
```

---

I think you should use an `<addr>` element here instead.

---

# Syntax highlighting

````
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
````

````
```python
def foo():
    if not bar:
        return True
```
````

---

# Blockquotes

<br>

```text
As Kanye West said:

> We're living the future so the present is our past.
```

---

![width:1000px](https://user-images.githubusercontent.com/48215474/71900530-e7410280-3155-11ea-8c46-d714e78d79cf.jpg)

---

![saturate:5.0 contrast: 100% height:300px drop-shadow:0,5px,10px,rgba(255,255,255)](https://www.w3.org/html/logo/downloads/HTML5_Logo_512.png)

# Works with HTML.

---

![](https://avatars3.githubusercontent.com/u/12959900?s=200&v=4)

# Typora

http://typora.io/

---

# Inline Math

<br>

```text
The identity matrix is $\left[\begin{array}{cc}
1 & 0\\0 & 1\end{array}\right]$.

$$ e = mc^2$$

```

---

The identity matrix is $\left[\begin{array}{cc}1 & 0\\0 & 1\end{array}\right]$.

$$ e = mc^2$$

---

## Introduction to $LaTeX$

20 January 2020 (Monday)
TT16 (2.201)
7 - 10 pm
<br>
Sign up [here](https://docs.google.com/forms/d/e/1FAIpQLScYzcq2nsw-QWtsPPeN9J_t96SjpuSPPCvh4IDOBchfeol5UQ/viewform).

---

# Diagrams

---

# UML Sequence

#### `js-sequence`

<br>

````text
```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!

​```

````

---

![hay](http://support.typora.io/media/diagrams/Snip20160816_1.png)

---

# Flowchart

#### `flowchart.js`

````text
```flow
st=>start: Start
op=>operation: Your Operation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op
​```
````

---

![width:800px](http://support.typora.io/media/diagrams/Snip20160816_2.png)

---

![](https://avatars0.githubusercontent.com/u/57169982?s=200&v=4)

# Mermaid

#### `mermaid-js`

---

# Class Diagram

<br>

````text
```mermaid
classDiagram
      Animal <|-- Duck
      Animal <|-- Fish
      Animal <|-- Zebra
      Animal : +int age
      Animal : +String gender
      Animal: +isMammal()
      Animal: +mate()
````

---

```text
      class Duck{
          +String beakColor
          +swim()
          +quack()
      }
      class Fish{
          -int sizeInFeet
          -canEat()
      }
      class Zebra{
          +bool is_wild
          +run()
      }
```

---

## ![height:500px](http://support.typora.io/media/new-80/Screen%20Shot%202019-11-27%20at%2023.17.54.png)

---

# State Diagram

<br>

````text
```mermaid
stateDiagram
    [*] --> Still
    Still --> [*]

    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```
````

---

## ![height:700px](http://support.typora.io/media/new-80/Screen%20Shot%202019-11-27%20at%2023.18.55.png)

---

# Pie Chart

<br>

````text
```mermaid
pie
    title Pie Chart
    "Dogs" : 386
    "Cats" : 85
    "Rats" : 150
```
````

---

## ![height:500px](http://support.typora.io/media/new-80/Screen%20Shot%202019-11-27%20at%2023.19.11.png)

---

# Pandoc

Swiss-army knife to convert content

---

# Conversion between

- PDF
- Markup formats
- HTML formats
- Ebooks
- XML formats
- $TeX$ formats
- Word processor formats
- Interactive notebook formats
  $\cdots$

---

# Demo

Converting Markdown to PDF

---

# MkDocs

Project documentation with Markdown.

---

# Installing MkDocs

<br>

```python
pip install mkdocs
```

---

# Material theme for MkDocs

<br>

```python
pip install mkdocs-material
```

---

# Create a new site

- `cd` to the appropriate folder

```sh
mkdocs new my-project
cd my-project
```

---

# Editing `mkdocs.yml`

<br>

```yml
site_name: Test
nav:
  - Home: index.md
  - About: about.md
theme:
  name: "material"
```

---

# Serving the site

<br>

```sh
mkdocs serve site
```

- Site up at [localhost:8000](http://localhost:8000/)

---

# Activity 2 (15 min)

- Play around with the Material themed site
- Refer to [Getting Started](https://squidfunk.github.io/mkdocs-material/getting-started/) for more customization

---

# Building the site

<br>

```sh
mkdocs build site
```

- By default, files at `/site`

---

![invert](https://www.nicepng.com/png/full/178-1787529_deploy-to-github-pages-github-pages-logo-png.png)

Free web hosting for GitHub users

---

# Personal Sites

- at _username_.github.io
- Repository should be '_username_.github.io'
- Source: `master` branch
  - Contents of `\site` to be placed here

---

# Project Sites

- at _username_.github.io/_project_
- Repository can have any name
- Source: `master` branch `/docs` folder
  - Contents of `\site` to be placed inside `/docs`

---

# Activity 3 (5 mins)

Host the website on GitHub.

---

# Powered by

![saturate:2.0 contrast: 100% height:100px drop-shadow:0,5px,10px,rgba(255,255,255)](https://raw.githubusercontent.com/marp-team/marp/master/marp.png)
Markdown Presentation Ecosystem

---

This entire slide deck was done entirely in Markdown.

---

# Source Code

<br>

![invert height:300px](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn.afterdawn.fi%2Fv3%2Fnews%2Foriginal%2Fgithub-logo.png&f=1&nofb=1)

[OpenSUTD](https://github.com/OpenSUTD) / [IAP2020-MkDocs](https://github.com/OpenSUTD/IAP2020-MkDocs)

---

# [OpenSUTD](https://github.com/opensutd)

<br>

![invert height:200px](https://avatars2.githubusercontent.com/u/43567235?v=4)

An open organisation owned
by the SUTD community.

---

### Signing off,

![height:250px](https://avatars2.githubusercontent.com/u/48215474?s=460&v=4)
[@flamanta](https://github.com/flamanta)

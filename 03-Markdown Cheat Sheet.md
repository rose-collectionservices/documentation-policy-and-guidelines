# Markdown Cheatsheet

Collection Services documentation is encoded using Markdown. The following explains how to encode the features most commonly found in Collection Services' manuals and documents. For information on additional features not covered by this cheat sheet, additional Markdown resources are listed [here](#Additional-markdown-resources).

* [1.0 Headings](#10-headings)
* [2.0 Emphasis](#20-emphasis)
  * [2.1 Bold text](#21-bold-text)
  * [2.2 Italicized text](#22-italicized-text)
* [3.0 Lists](#30-lists)
  * [3.1 Unordered lists](#31-unordered-lists)
  * [3.2 Ordered lists](#32-ordered-lists)
* [4.0 Links](#40-links)
  * [4.1 External links](#41-external-links)
  * [4.2 Links to other GitHub documents](#42-links-to-other-github-documents)
  * [4.3 Links to headings within the same GitHub document](#43-links-to-headings-within-the-same-github-document)
* [5.0 Images](#50-images)
* [6.0 Footnotes](#60-footnotes)
* [7.0 Tables](#70-tables)
* [8.0 Code and syntax](#80-code-and-syntax)

---

## 1.0 Headings

Use 1-6 hash marks (#) at the beginning of a heading. The number of hash marks used corresponds to the equivalent HTML header. A space is required between the final hash mark and the heading.

For example, the headings used in this post are encoded like this:

```
# Markdown cheat sheet
## 1.0 Headings
### 2.1 Unordered lists
```

---

## 2.0 Emphasis

### 2.1 Bold text

Use double asterisks (`**`).

For example, `**bold text**` displays as **bold text**.

### 2.2 Italicized text

Use a single asterisk (`*`) **or** a single underscore (`_`).

For example, both `*italicized text*` and `_italicized text_` displays as _italicized text_.

---

## 3.0 Lists

### 3.1 Unordered lists

Use an asterisk (`*`) followed by a space to create a bulleted list. Use the tab key to indent the asterisk to create a sub-list. A blank line is required both before and after the list.

For example:

``` 
    * Item one
    * Item two
        * Sub-item one
```

The above example will display like this:

* Item one
* Item two
   * Sub-item one

### 3.2 Ordered lists

```
1. Item one
2. Item two
   1. Sub-item one
3. Item three
```

The above example will display like this:

1. Item one
2. Item two
   1. Sub-item one
3. Item three

*Note:* The numbers used in creating an ordered list don't actually matter. For example, the following:

```
1. Item one
1. Item two
1. Item three
```

will still display like this:

1. Item one
1. Item two
1. Item three

---

## 4.0 Links

### 4.1 External links

To create a link to an external site, use the following syntax: `[hyperlinked text](<www.websiteAddress.com> "www.websiteAddress")`

For example, the following was used to create this link to [Emory University](<www.emory.edu> "www.emory.edu"):

```
The following was used to create this link to 
[Emory University](<www.emory.edu> "www.emory.edu").
```

The text contained within speech marks will appear if a user hovers over the linked text.

### 4.2 Links to other GitHub documents

To create a link to another GitHub document, use the following syntax: `[hyperlinked text](path/to/GitHub/document)`

For example, when linking to a page within the same repository, like [01-Overview of Archival Processing](https://github.com/rose-collectionservices/collection-services-manual/tree/master/01-OVERVIEW%20OF%20ARCHIVAL%20PROCESSING#overview-of-archival-processing), the following syntax should be used:

```
when linking to a page within the same repository, like
[01-Overview of Archival Processing](/01-OVERVIEW%20OF%20ARCHIVAL%20PROCESSING),
the following syntax should be used
```

*Note:* When a file name contains spaces, use `%20` in place of the space (as in the above example).

### 4.3 Links to headings within the same GitHub document

To create a link to a heading within the current GitHub document, us the following syntax: `[hyperlinked text](#heading)`.

For example, this link to [section 1.0](#10-headings) of this document is encoded like this:

```
[section 1.0](#10-headings)
```

*Note:* In the second set of parentheses, remove any punctuation, replace spaces with a dash (`-`), and use all lower caps.

---

## 5.0 Images

To add an image to a document:

1. Move a copy of the image files into the relevant image folder in GitHub.
2. At the position in the document where you would like the image to display, use the following syntax:

```
![Description of image](path/to/image/file "Description of image")
```

For example:

```
![Figure 1: Example accession record](/06-LOCAL%20PRACTICE/Images/accessionRecord.jpg "Figure 1: 
Example accession record")
```

*Note:* When a file name contains spaces, use `%20` in place of the space (as in the above example).

---

## 6.0 Footnotes

1. Add an in-text reference to a footnote using the following syntax:

```
<a href="#anchor1"><sup>1</sup></a>
```

2. Add footnote text using the following syntax at the end of your document:

```
<a id="anchor1">[1]</a> Here is my footnote.
```

For example:

```
I create a reference to a footnote like this <a href="#anchor1"><sup>1</sup></a>.
```

```
<a id="anchor1">[1]</a>And I create the footnote itself like this.
```

The example listed above will display like this:

I create a reference to a footnote like this <a href="#anchor1"><sup>1</sup></a>.

---

## 7.0 Tables

You can 'draw' tables in Markdown using a series of dashes (`-`) and pipes (`|`). However, this can be time-consuming. I recommend populating a spreadsheet with your data and uploading it as a CSV file [here](https://www.tablesgenerator.com/markdown_tables# "https://www.tablesgenerator.com/markdown_tables#"). This will generate the Markdown table code, which you can simply copy and paste into your document.

---

## 8.0 Code and syntax

Use a single back tick (`) to highlight code or syntax in a sentence.

For example: 
```
`Inline code` has `back ticks` around it
```

displays as: `inline code` has `back ticks` around it.

Use triple back ticks (```) to create a code block.

For example:

```

```This is a code block.```

```

displays as

```
This is a code block.
```

------

## Additional Markdown resources

* [Adam Pritchard's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet")
* [Daring Fireball: Markdown](https://daringfireball.net/projects/markdown/ "https://daringfireball.net/projects/markdown/")
* [Markdown Syntax](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf "https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf")
* [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables# "https://www.tablesgenerator.com/markdown_tables#")

------

*Footnotes:*

<a id="anchor1">[1]</a>And I create the footnote itself like this.

# Using Markdown in Documentation

>Markdown is a text-to-HTML conversion tool for web writers.

>Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML).

For example, this entire page was created using Markdown!

Below is a quick reference of all the Markdown syntax that is supported by Stoplight.

## Headers

```no-highlight
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Emphasis

```no-highlight
Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~
```
Emphasis, aka italics, with *asterisks* or _underscores_.

Strong emphasis, aka bold, with **asterisks** or __underscores__.

Combined emphasis with **asterisks and _underscores_**.

Strikethrough uses two tildes. ~~Scratch this.~~

## Lists

>In this example, leading and trailing spaces are shown with with dots: ⋅⋅⋅

```no-highlight
1. First ordered list item
2. Another item
   ..- Unordered sub-list
3. Actual numbers don't matter, just that it's a number
   ..1. Ordered sub-list
4. And another item

...You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).
```
## Links

Different ways to create links.

```no-highlight
1. To link Inline-style
[I'm an inline-style link](https://www.google.com)

2. To link Reference-style
[I'm a reference-style link][https://www.google.com "Google's Homepage"]

3. To link to API explorer from documentation pages
[API page](../api?type=post&path=/v1/apis)

4. To link/reference to another document/markdown
[Charge](?path=docs/Transactions/Charges.md)

5. To create anchor link within the page. You can place anchor by declaring <a name = "portal"></a>. Now you can reference this link anywhere within the page by declaring link such as [Dev Portal](#portal)

```
1. To link Inline-style
[I'm an inline-style link](https://www.google.com)

2. To link Reference-style
[I'm a reference-style link][https://www.google.com "Google's Homepage"]

3. To link to API explorer from documentation pages
[API page](../api?type=post&path=/v1/apis)

4. To link/reference to another document/markdown
[Charge](?path=docs/Transactions/Charges.md)

5. To create anchor link within the page. You can place anchor by declaring <a name = "portal"></a>. Now you can reference this link anywhere within the page by declaring link such as [Dev Portal](#portal)

## Images

Here's our logo ( hover to see the title text ):

![Fiserv Logo](../../assets/images/Fiserv_Logo.jpg "Fiserv Logo")


## Code and Syntax Highlighting

Inline `code` has `back-ticks around` it.

> Here is the example for javascript code.


```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
>Use language tags to change the syntax highlighting.

```json
{
  "JSON": "Syntax Highlighting"
}
```


## Tables

Tables aren't part of the core Markdown spec, but they are part of GFM and *Markdown Here* supports them. They are an easy way of adding tables to your email -- a task that would otherwise require copy-pasting from another application.

```no-highlight
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |


The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
```

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

## Blockquotes

> This is a blockquote.

```no-highlight
> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can *put* **Markdown** into a blockquote. 
```

## Horizontal Rule

```
Three or more...

---

Hyphens

***

Asterisks

___

Underscores
```
## Table with Nested Object

Table with nested objects, containing descriptions, HTML tags are also allowed.

| Name | Description | Example | 
|------|-------------|:----:|
| Headers | Large text refer to Header section for more detail | <h1> Hello </h1>
| Emphasis | italics, bold, or strikethrough | *italics*, **bold**, ~~strikethrough~~, **bold and _italics_**
| Lists | Refer to Lists section for more details | 1. List item 1 <br> 2. List item 2
| Links | Hyperlinks, refer to above Link section for more details | To link to API explorer from documentation pages API page [API page](../api?type=post&path=/v1/apis)
| Images | Visual representation | ![Fiserv Logo](../../assets/images/Fiserv_Logo.jpg "Fiserv Logo")
| Code | code blocks, syntax highlighting | <pre> String main(void) <br> { <b>this is a pre block </b> } </pre>  `rendering code snippets` 
| Tables | contains rows and columns | <table><tr><td>Table</td><td>Mini Description</td></tr><tr><td>Type</td><td>String</td></tr></table>
---

![API Explorer Expand All for Nested Objects](../../assets/images/API_Explorer_Expand_All.gif)

## Error Messages

Light mode error message color: #DD3435 <p style="color: #DD3435;">This text is light mode error message color.</p>
Dark mode error message color: #FF453A <p style="color: #FF453A;">This text is light mode error message color.</p>

## Footer Color

Light mode color: #e0e0e0 <hr style="border-color: #e0e0e0;">
Dark mode color: #333333 <hr style="border-color: #333333;">
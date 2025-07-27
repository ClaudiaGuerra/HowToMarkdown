# Markdown: The ultimate guide
This is a document to use as reference for my personal notes. For some time, I've been trying to find a simple way to keep my personal, learning and work notes. I've tried several tools (Notion, OneNote, Obsidian, Overleaf for LaTex, etc.) but they didn't seem to work for me. In consequence, I decided to use Markdown in the comfort of my offline VSCode. Most of this guide has been made using the [Markdown Guide](https://www.markdownguide.org/) using my own examples. Here, a guide for myself:

## Headings
To insert headings, you can use:

| Markdown               | Output                       |
|---                     |---                           |
| # Headings level 1     | <h1>Heading 1</h1>           |
| ## Heading level 2     | <h2>Heading level 2</h2>     |
| ### Heading level 3    | <h3>Heading level 3</h3>     |
| #### Heading level 4   | <h4>Heading level 4</h4>     |
| ##### Heading level 5  | <h5>Heading level 5</h5>     |
| ###### Heading level 6 | <h6>Heading level 6</h6>     |

æ

## Paragraphs
If you want to create a paragraph, it is not necessary to insert a \<br> you can just press "Enter". Like this, simple as that. I am not planning to write a few paragraphs just to show this (it would be nice, tough, but I still have a few other things to do). Soooo, have a look at the usual Lorem Ipsum:

Esse ea sunt pariatur consequat occaecat qui proident. Irure ut dolore excepteur fugiat aliqua amet duis pariatur Lorem. Cupidatat Lorem dolor consectetur officia fugiat enim non mollit fugiat mollit.

Labore est fugiat ut sunt. Voluptate ullamco voluptate ad aliquip ex id nostrud cupidatat sunt consequat eu mollit sint eiusmod. Eiusmod nostrud qui quis commodo cillum consectetur aliquip do excepteur.

Consectetur consequat mollit aliquip consectetur. Aliqua exercitation ipsum officia Lorem. Velit ea ad proident ex anim nisi elit ipsum ad est. Non magna sit aliqua exercitation magna mollit elit nulla id consequat aliquip. Cillum quis ipsum cupidatat ad laborum ad eu qui.

Enter, Enter, Enter. That's the key.
 
## Text colour
Black text might be a bit boring sometimes, don't you think? Well, I've got good news for you! If you want to change it, you can use:
``` html
<span style="color:blue">The text should be written like this</span>.
```
***Output***:
<span style="color:blue">The text should be written like this</span>.

## Blockquotes
> Adding a block qoute is simple. Just start the prase with a ">" and that's it!

## Emphasis
For **bold**, use:
``` markdown
**Text**
```

For *italic*, use:
``` markdown
*Text*
```

## Tables
I am not going to lie: I prefer LaTeX for tables, however, Markdown still has a reasonably good tables format. A bit limited, but good enough. I have not found a way to merge a row, hopefully I will at some point of my existence.

This table ...
|   Lorem  | Ipsum      |
| -------- | -------    |
| Proident | amet       |
| elit     | ea         |
| aliquip  | incididunt |

... looks like this in markdown:
```markdown
| Lorem    | Ipsum      |
| -------- | -------    |
| Proident | amet       |
| elit     | ea         |
| aliquip  | incididunt |
```
## Lists
Writing lists are quite simple. When you use markdown, it will always create a list with ordered numbers, even if the numbers you are using are not in a sequence (1,2,3,4 or 1,5,3,6 or 1,1,1,1) will always show the same (1,2,3,4)
### Ordered Lists
***Markdown***
```markdown
1. Item 1
2. Item 2
```
or, you can use unordered numbers. It's the same thing:
```markdown
1. Item 1
5. Item 2
```

***HTML***
```markdown
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

***Output***
1. Item 1
2. Item 2

### Unordered Lists
To create an unordered list, add dashes (-), asterisks (*), or plus signs (+) in front of line items. 

***Markdown***
```markdown
- Item 1
- Item 2
```
***HTML***
```markdown
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```

***Output***
- Item 1
- Item 2

#### Symbols
You can use dashes (-), asterisks (*), or plus signs (+), no restriction!

***Dash***
```markdown
- Item 1
- Item 2
```
***Asterisk***
```markdown
* Item 1
* Item 2
```
***Plus sign***
```markdown
+ Item 1
+ Item 2
```
***Output:***
>+ Item 1
>+ Item 2

### Indent items
Indent items? Sure, no problem! Indent one or more items to create a nested list.

***Markdown***
```markdown
- Item
    - Subitem
    - Subitem
```

***HTML***
```markdown
<ul>Item
  <li>Subitem<li>
  <li>Subitem<li>
</ul>
```
***Output***
<ul>
    <li>Item</li>
        <ul>
            <li>Subitem</li>
            <li>Subitem</li>
        </ul>
</ul>


## Links
I didn't write this section, I copied from [Markdown Guide](https://www.markdownguide.org/) and modified a few things. 

To create a link, enclose the link text in brackets and then follow it immediately with the URL in parentheses.

```markdown
My favorite search engine is [Duck Duck Go](https://duckduckgo.com).
```

The rendered output looks like this:
My favorite search engine is [Duck Duck Go](https://duckduckgo.com).


### URLs and Email Addresses
To quickly turn a URL or email address into a link, enclose it in angle brackets.
```markdown
<https://www.markdownguide.org>
<fake@example.com>
```
The output looks like this:
https://www.markdownguide.org
fake@example.com

### Formatting Links
To emphasize links, add asterisks before and after the brackets and parentheses. To denote links as code, add backticks in the brackets.
```markdown
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).
```

The rendered output looks like this:

>I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).

## Images
To insert an image use 
```markdown
![Kirkstall Abbey](Kirkstall-Abbey.jpg)
```
![Kirkstall Abbey](assets/images/Kirkstall-Abbey.jpg "Kirkstall Abbey")
*Kirkstall Abbey, Leeds, UK.*

### Captions
Markdown does not support captions natively so you can use HTML or simple text after the image:

```markdown
![Kirkstall Abbey](Kirkstall-Abbey.jpg)
*Kirkstall Abbey, Leeds, UK.*
```

```HTML
<figure>
    <img src="assets/images/Kirkstall-Abbey.jpg"
         alt="Kirkstall Abbey, Leeds, UK">
    <figcaption>Kirkstall Abbey, Leeds, UK.</figcaption>
</figure>
```
You can also add images from the internet by pasting the link in parentheses. 

## Code
A code block can be executed from here. If you pass the cursor on top of the code block, you will see a green "play" button. Clicking on it will execute the code, and will show the result below.


For example:
```javascript {cmd="node"}
const date = Date.now()
console.log(date.toString())
```

The syntax to write a code block is:

````markdown
```javascript {cmd="node"}
const date = Date.now()
console.log(date.toString())
```
````
Remember to use the {cmd="node"} next to JavaScript, to allow it to be executed.

**Note**: If you have multiple blocks of code, you can use the button "ALL" to execute all of them at once.
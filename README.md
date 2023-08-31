# Learning _MARKDOWN_ syntax

Creating a paragraph does not require an especific symbol or preparation, you just have to start writing. For example: This is a paragraph.
As long as it does not have an "enter space" indicating a full stop or **line break**, it will continue for as long as you want.

But, at the moment you press "enter", it will create another paragraph, like this.

## Aplying _italic_ and **bold**

To apply _italic_, you just have to add an underscore (\_) before and after a phrase or word, but you can also use an asterisk (\*) to do the trick. Here's an example:

`_italic_`

`*italic*`

In the same order of ideas, to apply **bold** to a phrase or a word, you will have to add two asterisks (\*\*).

`**bold**`

To use **_both at the same time_**, you will have to add, first the two asterisks (\*\*) and then an underscore (\_) before and after each phrase or word. Another way to do it is using three asterisks (\*\*\*), you will achieve the **_same results_**. This is how:

`**_bold and  italic_**`

`***bold and italic***`

Keep in mind, though, that once you start using one of the different ways, you should keep consistency using the same through the whole document in order to avoid issues.

## Headings

Headings will need the symbol # before them in order to work and the number will increase acording to the type of heading we need to use.

`# Heading 1`

It is important to leave a blank space between the hashtag (#) symbol and the heading.

## heading 2

This would be the syntax:

`## heading 2`

### heading 3

This would be the syntax:

`### heading 3`

#### heading 4

This would be the syntax:

`#### heading 4`

##### heading 5

This would be the syntax:

`##### heading 5`

###### heading 6

This would be the syntax:

`###### heading 6`

## Links

For links you will need two types of symbols:
`[]()`

[Google](https://www.google.com)

`[Google](https://www.google.com)`

It is the same for internal links:

[Learning _MARKDOWN_](#learning-markdown-syntax)

`[Learning _MARKDOWN_](#learning-markdown-syntax)`

However, this only works with headings because they serve as anchors of the document.

### Images

Images use the same format as links: `[]()`, but we will need to ad an exclamation symbol before, like this `![Here goes the 'alt' HTML text](Here goes the link or the location of the image)`

![Here goes the alt HTML text](https://jonmircha.com/img/blog/this-is-javascript.jpg)

`![Here goes the 'alt' HTML text](https://jonmircha.com/img/blog/this-is-javascript.jpg)`

## Separating lines

There are two main ways to create separating lines, with three hyphen (\-) or with three asterisks (\*).

---

`---`

---

`***`

This is the equivalent to the `<hr/>` etiquete in HTML.

## Lists

We can use numbers `1., 2., 3., etc` for ordered lists or asterisks/hyphen `-` for unordered lists, in both cases there has to be a blank space between the elements.

### Ordered list

1. Item 1
2. Item 2
   1. Sub Item 1
   2. Sub Item 2
      1. Sub-sub Item 1
3. Item 3

Like this:

```markdown
1. Item 1
2. Item 2
3. Sub Item 1
4. Sub Item 2
5. Sub-sub Item 1
6. Item 3
```

---

### Unordered list

- Item
- Item
  - Sub Item
  - Sub Item
    - Sub-sub Item
- Item

Like this:

```markdown
- Item
- Item
  - Sub Item
  - Sub Item
    - Sub-sub Item
- Item
```

## Blockquotes

We use the `>` symbol to create a blockquote.

> To be or not to be, that is the question.
> _Shakespeare_.

```markdown
> To be or not to be, that is the question.
> _Shakespeare_.
```

> As the emperor talks of ruling the universe, it still is not better than a good drink.
>
> > _Unknown._

```markdown
> As the emperor talks of ruling the universe, it still is not better than a good drink.`
>
> > _Unknown._
```

## Tables

We use the symbol pipe | as the column lines of the table and in the second row, we have to add three hyphens between those pipes.

| Table header | Table header | Table header |
| ------------ | ------------ | ------------ |
| Data 1       | Data 2       | Data 3       |
| Data 4       | Data 5       | Data 6       |
| Data 7       | Data 8       | Data 9       |
| Data 10      | Data 11      | Data 12      |

Here's how:

```markdown
| Table header | Table header | Table header |

| --- | --- | --- |

| Data 1 | Data 2 | Data 3 |

| Data 4 | Data 5 | Data 6 |
```

## Codes

### Inline code

If we need to highlight an especific word because it is related to a programming language, we just need to use (\` \`), like this: \`word\`.

For example, the word `let`, which is used in different languages.

```
`let`
```

### Block code

It is possible to create code blocks in two different ways, the fenced code method and the indented method.

The fenced method implies adding three (```) at the beggining and ending of the block of code. The indented method is more simple, you just have to indent the block of code that you want to create.

The main difference between both of them is that the fenced method allows you to add **syntax highlighting**, which basically makes the code looks nicer depending on which language are you using in your code.

Here you can see more info:

[Fenced Code Blocks](https://www.markdownguide.org/extended-syntax/#fenced-code-blocks).

And here, you will find the different languages that are supported by this feature:

[Markdown Supported Languages](https://github.com/jincheng9/markdown_supported_languages).

Keep in mind that this also depends on the markdown editor you use. The editor need to detect the language and do the syntax highlight.

### Fenced Method - JS

```js
function sumar(a, b) {
  return a + b;
}
```

````
```js
function sumar(a, b) {
  return a + b;
}
```
````

---

### Indented Method - json

    {
      "firstName": "John",
      "lastName": "Smith",
      "age": 25
    }

```
    {
      "firstName": "John",
      "lastName": "Smith",
      "age": 25
    }
```

Here's another example with html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title></title>
  </head>
  <body></body>
</html>
```

However, inside of markdown we can use _HTML_ code directly:

<form>
  <label for="Q">Search:</label>
  <input type="search" name="Q" id="Q"/>
</form>

```
<form>
  <label for="Q">Buscar:</label>
  <input type="search" name="Q" id="Q"/>
</form>
```

## Comments

To make a comment in _MARKDOWN_ is the same as in _HTML_:

```html
<!-- This is a comment -->
```

## References:

- [JonMirCha](https://www.youtube.com/watch?v=FlsoBiteuPM&list=PLvq-jIkSeTUZ7FtDshwPGlZoLSWyR5ryt&index=5&ab_channel=jonmircha)
- [Markdown Guide](https://www.markdownguide.org/)

---
title: "Solidity, Handle with Care"
date: 2021-04-03T23:29:21+05:30
draft: false
github_link: "https://github.com/gurusabarish/hugo-profile"
author: "4111self"
tags:
  - Solidity
  - Blockchain
image: https://miro.medium.com/max/880/1*KhxTw-tTuNN8hhmbF3uzVw.png
description: ""
toc:
---

## Solidity Shortcomings
As a programmer with some experience in Solidity, the programming language used to write smart contracts on the Ethereum blockchain, I've come to realize that while it's a powerful tool, it also has some significant flaws that can lead to unintended consequences.

Let's dive deep into the intricacies of Solidity and examine these flaws, as well as their implications on smart contracts and the Ethereum network.

One of the biggest issues with Solidity is its lack of inheritance capabilities. Inheritance is a fundamental feature in Object-Oriented Programming (OOP) and allows developers to build complex systems by creating a hierarchy of classes that inherit properties and behaviors from a parent class. Without inheritance, developers are forced to reinvent the wheel for every new smart contract they write, making the code more complex and prone to errors.

Another flaw in Solidity is its handling of exceptions. Unlike most programming languages, Solidity doesn't have a try-catch mechanism to handle exceptions. Instead, it uses a require() function, which throws an exception and reverts all changes made to the state if the condition inside the require statement is not met. While this might seem straightforward, it's a double-edged sword that can lead to unintended consequences. For example, if a smart contract calls another contract and that contract throws an exception, the calling contract will also be terminated, leading to a cascade of failures and potential loss of funds.

Finally, Solidity is susceptible to vulnerabilities such as the well-known Reentrancy Attack. This attack allows an attacker to repeatedly call a smart contract's functions and extract funds before the contract has a chance to update its internal state. This vulnerability is a direct consequence of the lack of proper concurrency handling in Solidity and can lead to massive losses if not mitigated properly.

In conclusion, while Solidity is a powerful tool for developing smart contracts on the Ethereum blockchain, its limitations and flaws can lead to unintended consequences. Developers must be aware of these flaws and take proper precautions when writing and deploying smart contracts to minimize the risk of loss of funds and other security incidents. It's important that the Ethereum community continues to work towards improving Solidity and making it a safer and more robust programming language for smart contracts.

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use _Markdown syntax_ within a blockquote.

### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.</p>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

| Name  | Age |
| ----- | --- |
| Bob   | 27  |
| Alice | 23  |

### Inline Markdown within tables

| Inline&nbsp;&nbsp;&nbsp; | Markdown&nbsp;&nbsp;&nbsp; | In&nbsp;&nbsp;&nbsp;                | Table  |
| ------------------------ | -------------------------- | ----------------------------------- | ------ |
| _italics_                | **bold**                   | ~~strikethrough~~&nbsp;&nbsp;&nbsp; | `code` |

## Code Blocks

### Code block with backticks

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Example HTML5 Document</title>
  </head>
  <body>
    <p>Test</p>
  </body>
</html>
```

### Code block indented with four spaces

    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

### Code block with Hugo's internal highlight shortcode

{{< highlight html >}}

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## List Types

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- List item
- Another item
- And another item

### Nested list

- Item
  1. First Sub-item
  2. Second Sub-item

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1

## H2

### H3

#### H4

##### H5

###### H6

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

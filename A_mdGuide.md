# :dizzy:Markdown demo (atom)

* Markdown Language本質上係一種html變種，所以html tags都照樣可以用:
  * e.g. <font color="pink"> Hello, text in pink </font>

---
## Atom Guide
* `ctrl` + `shift` + `p` 可以call terminal出黎
* Project Folder請唔好有中文or符號, Markdown Preview會睇唔到圖片
* 若然你只係想睇內容，最好用`.html`files會比較好睇 :)
* Btw, markdown主要都係作為文字記錄平台, 如果要畫圖/非文字媒體最好用其他software(e.g. powerpoint) 畫完再貼上黎會比較方便
* atom入面打`i` + `tab` = *italic*(自動出個斜線符號包住)，同理`b`+`tab` = **bold**
* `File` $\rightarrow$ `Stylesheet` 可以自己加css(改字體etc.)

**必裝Packages**
- Markdown preview enhanced
- Markdwon table editor
- Markdown image assistant
---

[toc]

## General
```
# Header1
## Header2
### Header3
max = Header6
```

*Italic1*   _Italic2_
**Bold1**   __Bold2__
~~StrikThrough~~
==Highlight==

### Lists
- unordered list
  * sublist
1. ordered list
  1. ordered list

- [ ] Task list
    - [x] To-do list



### Table
`Tab`: Next cell
`Enter`: Next line
`Esc`: Leave table edit mode
| Column1    |   Column2    |     Column3 |
|:---------- |:------------:| -----------:|
| Left align | Center align | Right align |
| L          |      C       |           R |

| Merge    | cell      |
| -------- | --------- |
| >        | col_merge |
| Enable   | row_merge |
| Extended | ^         |
| table    | Function  |



***

### Link
[GitHub](http://github.com)

### Image
![thumb-1920-752685](assets/thumb-1920-752685.png)

---
### Text Formatting
`Superscript:` 1^st^
`Subscript:` CO~2~
`Footnotes:` Article [^1]
[^1]:Wikipedia

`Abbreviation:`
*[md]: markdown
*[cool]: and beautiful
md is cool

`emoji:` :smiley: :fa-flag:
Cheatsheet:
`@import` "assets\emoji_list.md"

---


### Blockquote
> Evil knows of the good,
>> But good does not know of the evil

### Code Block
```ruby {.line-numbers}
main()
{
  int i=0;
  while (1)
    break;
  end;
}
```


## Maths
[CheatSheet](https://katex.org/docs/supported.html)

### Basics
$ x^5+y^{10} = {dy \over dx}2x$
$ \sqrt[4]{x}  \not= \int \iint  $

```Math
 \tag{equation 1}
 f(x,y)=sin(2\pi\theta)

```

$$
\tag{2.10}
 \sum_{n=1}^{100} e^n
$$

$
\tilde{a}, \vec{F}, \bar{y}, \big(,\Big(, \bigg( ABCD \bigg)
$

### Matrix
```Math
\begin{matrix}
  a&b\\
  c&d
\end{matrix}
```
```Math
\begin{bmatrix}
  a&b\\
  c&d
\end{bmatrix}
```
```Math
\begin{vmatrix}
  a&b\\
  c&d
\end{vmatrix}
```

### Alignments

```Math
x = \begin{cases}
   a &\text{if } b \\
   c &\text{if } d
\end{cases}
```
```Math

\begin{alignedat}{2}
   10&x+ &3&y = 2 \\
   3&x+&13&y = 4
\end{alignedat}

```

### Greek Letters
$ \Delta \delta \phi \Phi$

### Logics, Set Theory
| $\therefore$ | $\because$    |
| ------------ | ------------- |
| $\sub$       | $\empty$      |
| $\in$        | $\varnothing$ |

### Marcos
``` Math
 \def\func{x^y}
 \func + \func \over \func
```


## Diagrams

### flow charts
```flow
st=>start: hello
e=>end: byebye
op=>operation: add a into b
cond=>condition: are you sure?

st->op->cond
cond(yes)->e
cond(no)->op
```

## Import

### Configure Image
@import "image.png" {width="400px" height="300px" title="Hello" align="Right"}


### Supported file types
Common:
`.jpeg(.jpg)`, `.gif`, `.png`
`.csv`: converted to markdown table.
`.html`: embeded directly
`.pdf`: you need to download **pdf2svg** first


## Presentation
[Guide](https://shd101wyy.github.io/markdown-preview-enhanced/#/presentation)

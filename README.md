
# Readme file styling

## Heading
```
example: # The largest heading
         ## The second largest heading
         ###### The smallest heading
```
> output:
# The largest heading
## The second largest heading
###### The smallest heading

## Bold text
```
syntax: ** ** or __ __
command: ctrl + b
example: **Bold text**
```
> output: **this is bold text**

## Italic text
```
syntax: * * or _ _
command: ctrl + i
example: *Bold text*
```
> output: *this is bold text*

## Strikethrough Text
```
syntax: ~~ ~~
example: ~~Bold text~~
```
> output: ~~this is bold text~~

## Bold and nested italic
```
syntax: ** ** and _ _
example: **This text is _extremely_ important**
```
> output: **This text is _extremely_ important**
 
## All bold and italic
```
syntax: *** ***
example: ***All this text is important***
```
> output: ***All this text is important***

## Quoting code
```
syntax: ` `
command: ctrl + e
example: ``` 
         line one
         line two
         line three
         ```
```
> output: 
```
line one
line two
line three
```

## Link
```
syntax: [](url)
command: ctrl + k
example: [GitHub Pages](https://pages.github.com/)
```
> output: [GitHub Pages](https://pages.github.com/)

## Relative links
You can define relative links and image paths in your rendered files to help readers navigate to other files in your repository.

A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:
```
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```
GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. You can use all relative link operands, such as `./` and `../`.

Relative links are easier for users who clone your repository. Absolute links may not work in clones of your repository - we recommend using relative links to refer to other files within your repository.

## Images
You can display an image by adding `!` and wrapping the alt text in`[ ]`. Then wrap the link for the image in parentheses `()`.
```
![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)
```
> output: 

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

GitHub supports embedding images into your issues, pull requests, discussions, comments and .md files. You can display an image from your repository, add a link to an online image, or upload an image. For more information, see "[Uploading assets]()."

Here are some examples for using relative links to display an image.

| Context | Relative Link |
| --- | --- |
| In a `.md` file on the same branch | `/assets/images/electrocat.png` |
| In a `.md` file on another branch | `/../main/assets/images/electrocat.png` |
| In issues, pull requests and comments of the repository | `../blob/main/assets/images/electrocat.png` |
| In a `.md` file in another repository | `/../../../../github/docs/blob/main/assets/images/electrocat.png` |
| In issues, pull requests and comments of another repository | `../../../github/docs/blob/main/assets/images/electrocat.png?raw=true` |

## Horizontal line
```
syntax: ---
```
> output: 
---

## Lists
You can make an unordered list by preceding one or more lines of text with `-` or `*`.
```
- George Washington
- John Adams
- Thomas Jefferson
```
> output: 
- George Washington
- John Adams
- Thomas Jefferson

```
1. James Madison
2. James Monroe
3. John Quincy Adams
```
> output:
1. James Madison
2. James Monroe
3. John Quincy Adams

### Nested Lists

You can create a nested list by indenting one or more list items below another item.

To create a nested list using the web editor on GitHub or a text editor that uses a monospaced font, like Atom, you can align your list visually. Type space characters in front of your nested list item, until the list marker character (`-` or `*`) lies directly below the first character of the text in the item above it.

```
1. First list item
   - First nested list item
     - Second nested list item
```
> output: 
1. First list item
   - First nested list item
     - Second nested list item

To create a nested list in the comment editor on GitHub, which doesn't use a monospaced font, you can look at the list item immediately above the nested list and count the number of characters that appear before the content of the item. Then type that number of space characters in front of the nested list item.

In this example, you could add a nested list item under the list item `100. First list item` by indenting the nested list item a minimum of five spaces, since there are five characters (`100.` ) before `First list item`.

```
100. First list item
     - First nested list item
```
> output:
100. First list item
     - First nested list item

You can create multiple levels of nested lists using the same method. For example, because the first nested list item has seven spaces (`␣␣␣␣␣-␣`) before the nested list content `First nested list item`, you would need to indent the second nested list item by seven spaces.

```
100. First list item
     - First nested list item
       - Second nested list item
```

> output: 
100. First list item
     - First nested list item
       - Second nested list item

## Task lists
To create a task list, preface list items with a regular space character followed by `[ ]`. To mark a task as complete, use `[x]`.

```
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:
```

> output: 
- [x] #739
- [ ] https://github.com/octo-org/octo-repo/issues/740
- [ ] Add delight to the experience when all tasks are complete :tada:

If a task list item description begins with a parenthesis, you'll need to escape it with `\`:

`- [ ] \(Optional) Open a followup issue`




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



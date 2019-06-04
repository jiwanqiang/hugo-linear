---
title: "Hugo Linear Theme Preview"
date: 2019-06-02T16:59:50+08:00
tags: ["hugo", "theme", "linear", "preview"]
draft: true
---

I created one theme for [hugo](https://gohugo.io/) static site generator that named [linear](https://github.com/jiwq/hugo-linear). In this theme beta version, it owns some basic features. In this article, I will introduce it for you. 

If you like this theme, welcome use it and also thank you help to growing up. Such as star the project or report the issue or new feature or submit the pull request, even donate a cup of coffee for me.

## 1. Basic
### 1.1 Headings
```markdown
# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6
```

### 1.2 Emphasis
To **bold text**, add two asterisks(`**`) or underscores(`__`) before and after a word or phrase.<sup>[[1]](#ref00)</sup>

To *italicize text*, add one asterisk(`*`) or underscore(`_`) before and after a word or phrase.<sup>[[2]](#ref01)</sup> 

To emphasize text with ***bold and italics*** at the same time, add three asterisks(`***`) or underscores(`___`) before and after a word or phrase.<sup>[[3]](#ref02)</sup>

To ~~deleted text~~, add two tildes(`~~`) before and after a word or phrase.

### 1.3 Blockquotes
> 恰同学少年，风华正茂；书生意气，挥斥方遒。
>
> <cite>-- 毛泽东 ·《沁园春·长沙》</cite>
>
>> 沁园春，词牌名，又名“东仙”“寿星明”“洞庭春色”等。

### 1.4 Ordered List
1. First Item
  2. Indented item
  2. Indented item
2. Second Item
  1. Indented item
  1. Indented item

### 1.5 Unordered Lists
* First Item
  * Indented item
  * Indented item
* Second Item
  - Indented item
  - Indented item
* Third Item
  + Indented item
  + Indented item

### 1.6 Task List
- [ ] Hugo Linear Project 
  - [ ] Add chart shortcode for data statistics
  - [ ] Supports TOC in article page
  - [ ] Add some new templates such as about/project etc.
  - [x] Add [LaTex](https://mathjax.org) basic function
  - [x] Add [syntax highlighting](https://highlightjs.org/usage/) for code
  - [x] Add [task lists](https://github.com/blog/1375-task-lists-in-gfm-issues-pulls-comments)
  - [x] Initial the project
  - [x] Design the basis tone
  - [x] Design the theme wireframe

## 2. Advance
### 2.1 Table
| Align to Left  | Align to Center | Align to Right |
| :------------- | :-------------: | -------------: |
|  Content Cell  |  Content Cell   |  Content Cell  |
|  Content Cell  |  Content Cell   |  Content Cell  | 

### 2.2 Syntax Highlighting
As we all know `Hello, world!` is the first program for us in the programming road. In linear theme we used `highlight.js` implements the syntax highlighting.<sup>[[4]](#ref03)</sup>

**C (1972)**
```c
int main() {
  print("Hello, world!");
}
```
**Bash Shell (1978)**
```bash
echo "Hello, world!"
```
**Objective-C (1980)**
```objc
int main() {
  NSLog(@"Hello, world!");
}
```
**Python (1989)**
```python
print("Hello, world!")
```
**Java (1995)**
```Java
package hello;
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("Hello, world!");
  }
} 
```
**JavaScript (1995)**
```javascript
<script>
  console.log("Hello, world!")
</script>
```
**Go (2009)**
```
package main
import "fmt"
func main() {
  fmt.Println("Hello, world!")
}
```
**Kotlin (2011)**
```
package hello
fun main() {
  println("Hello, world")
}
```
**Swift (2014)**
```
print("Hello, world!")
```

### 2.3 Mathematics
[MathJax](https://mathjax.org) allows you to include mathematics in your web pages, either using `LaTeX`, `MathML`, or `AsciiMath` notation, and the mathematics will be processed using JavaScript to produce `HTML`, `SVG`, or `MathML` equations for viewing in any modern browser.<sup>[[5]](#ref04)</sup>

<div>
$$
(\nabla_X Y)^k = X^i (\nabla_i Y)^k = X^i \left( \frac{\partial Y^k}{\partial x^i} + \Gamma_{im}^k Y^m \right)
$$
</div>

## 3. Shortcodes
Shortcodes are simple snippets inside your content files calling built-in or custom templates.<sup>[[6]](#ref05)</sup>

### 3.1 Build-in Figure
{{< figure src="/assets/hugo-linear-preview/deer.jpg" title="🦌Deer 🦌" class="center">}}

### 3.2 Build-in Gist
Bloggers often want to include GitHub gists when writing posts. Let’s suppose we want to use the gist at the following url:
```
https://gist.github.com/jiwq/6d6f145d3ba8ca8ffba0
```

We can embed the gist in our content via username and gist ID pulled from the URL:
{{< gist jiwq 6d6f145d3ba8ca8ffba0 >}}
### 3.3 Build-in Instagram
{{< instagram Bq_fHjuFTuz >}}

### 3.4 Build-in Tweet
{{< tweet 877500564405444608 >}}

### 3.5 Build-in Vimeo
{{< vimeo 146022717 >}}

### 3.6 Build-in Youtube
{{< youtube w7Ft2ymGmfc >}}

## Reference
* <p id='ref00'>[Markdown Basic Syntax Documentation](https://daringfireball.net/projects/markdown/syntax)</p>
* <p id='ref01'>[GitHub Flavored Markdown Spec](https://github.github.com/gfm/)</p>
* <p id='ref02'>[Markdown Guide](https://www.markdownguide.org/)</p>
* <p id='ref03'>[highlight.js](https://highlightjs.org)</p>
* <p id="ref04">[MathJax](https://www.mathjax.org/)</p>
* <p id='ref05'>[Hugo Documents](https://gohugo.io/documentation/)</p>

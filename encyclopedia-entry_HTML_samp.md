#HTML [&lt;samp>](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/samp) element

*&lt;samp> is an HTML element.*

The &lt;samp> element is an element intended to represent **_output_** from a computer program, and therefore carries that semantic interpretation when used within an HTML document. Use of the element will usually result in the text placed between its opening (`<samp>`), and closing (`</samp>`) tags to be displayed in the browser's default monospace font.

## Syntax

The &lt;samp> element uses opening and closing tags since it modifies content/text and so must have the closing tag to delineate what is to be modified. That is, it is not a "singleton"/"self-closing", tag as those tags *do not* modify other content, unlike the &lt;samp> tag.

```
<samp>Place computer output to be rendered using the "<samp>" element here.</samp>
```

## Attributes

This element only includes the [global attributes](https://developer.mozilla.org/en-US/docs/HTML/Global_attributes).

## Browser Compatibility

&lt;samp> is supported in effectively all browsers (since IE6+, Firefox 2+, Chrome 1+ etc).

## Example 1

This code example shows the basic use of the `<samp>` element and how its content gets rendered.

```
<p>Upon an unsuccessful file search, you may see a response: <samp>File not found.</samp></p>
```
And this is the rendered code:

<p>Upon an unsuccessful file search, you may see a response: <samp>File not found.</samp></p>

## Example 2 - Rendering Multi-line code with corresponding output

Here I'll make a point about the semantic difference between the <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/code" target="_blank"><strong><code>&lt;code></code></strong></a> and `<samp>` tags, both of which will render text placed between their opening and closing tags in the browser's default monospace font. So while they render their content similarly, they carry different semantic interpretations and should be used accordingly. The `<code>` element is meant, semantically, to represent a section of computer code. I will also use the <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/pre" target="_blank"><strong><code>&lt;pre></code></strong></a> (**preserve formatting**) tag to format the text as typed with regard to whitespace - spacing and line breaks. It also renders its content in the browser's default monospace font and is useful for representing multi-line blocks of code that need particular as-typed formatting.

To represent programming code input, you would use the `<code>` tag like so:

```
<pre><code>
var myArray = [6, 5, 4, 3, 1, 2];
myArray.sort();
console.log(myArray);
</code></pre>
```
And this would be the rendering:  
<pre><code>
var myArray = [6, 5, 4, 3, 1, 2];
myArray.sort();
console.log(myArray);
</code></pre>

Now, to render the output of such code, you should use the `<samp>` element like so:

`<samp>[ 1, 2, 3, 4, 5, 6 ]</samp>`

And this would be the rendering:

<samp>[ 1, 2, 3, 4, 5, 6 ]</samp>

So, while the default rendering, which could be changed with CSS, is similar, the semantic meaning within the document is appropriately different.

## Notes

As noted and to further clarify and point out, the HTML `<pre>` element will also render its text content with the browser's default monospace font, but **_it is not intended, by itself, to semantically represent computer input or output._** However, **`pre`** stands for **preserve formatting** and as such it honors whitespace, such as spaces, carriage returns, and tabs, within the content. That is the content will be rendered just as it is typed, as illustrated in Example 2 above. That is the purpose of the `<pre>` element.

Just for completeness, when discussing and rendering computer-related code, input, keyboarding, and output, we have an additional HTML element available - the <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/kbd" target="_blank"><strong><code>&lt;kbd></code></strong></a> element. This element identifies user keyboard input and produces an inline element whose content is displayed in the browser's default monospace font.

Here is an example of its use:

```
<p>To copy the text, first select it, then press <kbd>Ctrl</kbd> + <kbd>C</kbd></p>
```

And this is the rendered code:

<p>To copy the text, first select it, then press <kbd>Ctrl</kbd> + <kbd>C</kbd></p>

So with the combination of the `<pre>`, `<code>`, `<samp>`, and `<kbd>` HTML elements, we can discuss, render, and semantically represent, computer-related code, input, keyboarding, and output information within an HTML document in a consistent and appropriate manner.

## Browser Support as of this writing

This element is supported in effectively all browsers (since IE6+, Firefox 2+, Chrome 1+ etc).

**References:**

1. [&lt;samp> - developer.mozilla.org][ref1]  
2. [&lt;pre> - developer.mozilla.org][ref2]  
3. [&lt;code> - developer.mozilla.org][ref3]  
4. [&lt;kbd> - developer.mozilla.org][ref4]  
5. [pre, code, kbd, samp, and var - ficksworkshop.com][ref5]  
6. [&lt;code> vs &lt;pre> vs &lt;samp> for inline and block code snippets][ref6]  
7. [What are the differences between kbd, samp and code in HTML][ref7]  
8. [Can I use samp - caniuse.com][ref8]  

[ref1]:https://developer.mozilla.org/en-US/docs/Web/HTML/Element/samp
[ref2]:https://developer.mozilla.org/en-US/docs/Web/HTML/Element/pre
[ref3]:https://developer.mozilla.org/en-US/docs/Web/HTML/Element/code
[ref4]:https://developer.mozilla.org/en-US/docs/Web/HTML/Element/kbd
[ref5]:http://www.ficksworkshop.com/blog/14-coding/93-pre-code-kbd-samp-var
[ref6]:http://stackoverflow.com/questions/4611591/code-vs-pre-vs-samp-for-inline-and-block-code-snippets
[ref7]:http://stackoverflow.com/questions/32284477/what-are-the-differences-between-kbd-samp-and-code-in-html
[ref8]:http://caniuse.com/#search=samp


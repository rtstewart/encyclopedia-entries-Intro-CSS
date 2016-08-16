# CSS [caption-side](https://developer.mozilla.org/en-US/docs/Web/CSS/caption-side)

*caption-side is a CSS property.*

The `caption-side` CSS property positions the content of a table's `<caption>` element to the specified side. The HTML `<caption>` Element/(HTML Table Caption Element) represents the title of a table. `<caption>` is the first descendant of a `<table>`, however it may placed elsewhere, relative to the table, with CSS.

## Syntax

Introduction to the syntax/usage. A example of CSS syntax is below:

```
caption-side: top|bottom|initial|inherit|unset;
```

### Values

Only __\**standard*__ values are presented here. The values are relative to the CSS [`writing-mode`](https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode) property.

<table>
    <caption>Valid CSS property <code>caption-side:</code> values, types, and their effects</caption>
    <tr>
        <th>Value</th>
        <th>Value Type</th>
        <th>Effect</th>
    </tr>
    <tr>
        <td><code>top</code></td>
        <td>directional</td>
        <td>Postitions the caption above the table. This is the default.</td>
    </tr>
    <tr>
        <td><code>bottom</code></td>
        <td>directional</td>
        <td>Postitions the caption below the table.</td>
    </tr>
    <tr>
        <td><code>inherit</code></td>
        <td>Global</td>
        <td>This indicates that the <code>caption-side</code> value defined on the parent's element must be used.</td>
    </tr>
    <tr>
        <td><code>initial</code></td>
        <td>Global</td>
        <td>Sets this property to the default (top) value.</td>
    </tr>
    <tr>
        <td><code>unset</code></td>
        <td>Global</td>
        <td>Resets the property to its inherited value if inherited from its parent. If the property is not inherited, it resets the property to the default value. This is the general effect of the global/CSS-wide <em>keyword</em> <code>unset</code>.</td>
    </tr>
</table>

## Example 1

The table above uses the `<caption>` element, with no specification for `caption-side`, since within Markdown, we cannot use CSS. So the default value of `top` is being used for the `<caption>` content *"Valid CSS property caption-side: values, types, and their effects"*.

Here is the code:

```
<table>
    <caption>Valid CSS property <code>caption-side:</code> values, types, and their effects</caption>
    <tr>
        <th>Value</th>
        <th>Value Type</th>
        <th>Effect</th>
    </tr>
    <tr>
        <td><code>top</code></td>
        <td>directional</td>
        <td>Postitions the caption above the table. This is the default.</td>
    </tr>
    <tr>
        <td><code>bottom</code></td>
        <td>directional</td>
        <td>Postitions the caption below the table.</td>
    </tr>
    <tr>
        <td><code>inherit</code></td>
        <td>Global</td>
        <td>This indicates that the <code>caption-side</code> value defined on the parent's element must be used.</td>
    </tr>
    <tr>
        <td><code>initial</code></td>
        <td>Global</td>
        <td>Sets this property to the default (top) value.</td>
    </tr>
    <tr>
        <td><code>unset</code></td>
        <td>Global</td>
        <td>Resets the property to its inherited value if inherited from its parent. If the property is not inherited, it resets the property to the default value. This is the general effect of the global/CSS-wide <em>keyword</em> <code>unset</code>.</td>
    </tr>
</table>
```

[Here is a separate HTML document with `caption-side: top` set for the same table code.](https://rtstewart.github.io/encyclopedia-entries-Intro-CSS/caption-side_top.html)  Notice the `<caption>` content is still on top - the default location/value - but is centered with respect to the table when used in an HTML document.

## Example 2

[This is an HTML document with `caption-side: bottom`.](https://rtstewart.github.io/encyclopedia-entries-Intro-CSS/caption-side_bottom.html) The `<caption>` content is now below the table and centered with respect to the table.

## Notes

__\*__ There are four other __*non-standard*__ values that were proposed for CSS 2, but removed from the final CSS 2.1 specification: `left`; `right`; `top-outside`; and `bottom-outside` [[1]][ref1].

## Browser Support as of this writing

<table>
    <tr>
        <th colspan="6">Desktop</th>
    </tr>
    <tr>
        <th>Feature</th>
        <th>Chrome</th>
        <th>Firefox</th>
        <th>Internet Explorer</th>
        <th>Opera</th>
        <th>Safari</th>
    </tr>
    <tr>
        <td>Basic support (for top and bottom)</td>
        <td>1.0</td>
        <td>1.0</td>
        <td>8.0</td>
        <td>4.0</td>
        <td>1.0</td>
    </tr>
    <tr>
        <td>top and bottom are relative to the <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode" target="_blank"><code>writing-mode</code></a> value</td>
        <td>Not Supported</td>
        <td>42</td>
        <td>Not Supported</td>
        <td>Not Supported</td>
        <td>Not Supported</td>
    </tr>
</table>

<table>
    <tr>
        <th colspan="6">Mobile</th>
    </tr>
    <tr>
        <th>Feature</th>
        <th>Chrome</th>
        <th>Firefox</th>
        <th>Internet Explorer</th>
        <th>Opera</th>
        <th>Safari</th>
    </tr>
    <tr>
        <td>Basic support (for top and bottom)</td>
        <td>?</td>
        <td>?</td>
        <td>?</td>
        <td>?</td>
        <td>?</td>
    </tr>
    <tr>
        <td>top and bottom are relative to the <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/writing-mode" target="_blank"><code>writing-mode</code></a> value</td>
        <td>Not Supported</td>
        <td>42.0</td>
        <td>Not Supported</td>
        <td>Not Supported</td>
        <td>Not Supported</td>
    </tr>
</table>

**References:**

1. [caption-side - developer.mozilla.org][ref1]  
2. [CSS caption-side Property - www.w3schools.com][ref2]  
3. [unset - developer.mozilla.org][ref3]  

[ref1]:https://developer.mozilla.org/en-US/docs/Web/CSS/caption-side
[ref2]:http://www.w3schools.com/cssref/pr_tab_caption-side.asp
[ref3]:https://developer.mozilla.org/en-US/docs/Web/CSS/unset




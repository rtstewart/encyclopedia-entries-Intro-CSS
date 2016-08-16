# CSS [vertical-align](https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align)

*`vertical-align` is a CSS property.*

The `vertical-align` CSS property defines the vertical alignment of an inline element or table-cell. That is, it controls how elements set next to each other on a line are lined up.

Provide an overview of what the reference entry is, how it's used, it's significance, or how it's commonly used.

## Syntax

In typical CSS format, the syntax of `vertical-align` is to follow the colon after `vertical-align:` with either: a **keyword** value, a **length** value, a **percentage** value, or a **Global** value.

The following gives a syntax example using the **keyword** `text-top`:

`vertical-align: text-top;`

So, generally, the syntax is:

* `vertical-align: [keyword value];`  
* `vertical-align: [length value];`  
* `vertical-align: [percentage value];`  
* `vertical-align: [Global value];`  

### Values

The **Global** values that `vertical-align` can take are:

`vertical-align: inherit;`  
`vertical-align: initial;`  
`vertical-align: unset;`  

For inline elements, (e.g., `<span>, <img>, display: inline-block;`) `vertical-align` can take the following values, *__most__ of which vertically align the element relative to its parent element*. For elements that do not have a baseline, the bottom margin edge is used instead.
<table>
    <caption><strong><code>vertical-align</code> values for inline elements</strong></caption>
    <tr>
        <th width="20%">Value<br>(for inline elements)</th>
        <th>Type</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><code>baseline</code></td>
        <td>keyword</td>
        <td>This is the default value. Aligns the baseline of the element with the baseline of its parent.</td>
    </tr>
    <tr>
        <td><code>sub</code></td>
        <td>keyword</td>
        <td>Aligns the baseline of the element with the subscript-baseline of its parent. Where a &lt;sub> element would be positioned.</td>
    </tr>
    <tr>
        <td><code>super</code></td>
        <td>keyword</td>
        <td>Aligns the baseline of the element with the superscript-baseline of its parent. Where a &lt;sup> element would be positioned.</td>
    </tr>
    <tr>
        <td><code>text-top</code></td>
        <td>keyword</td>
        <td>Aligns the top of the element with the top of the parent element's font.</td>
    </tr>
    <tr>
        <td><code>text-bottom</code></td>
        <td>keyword</td>
        <td>Aligns the bottom of the element with the bottom of the parent element's font.</td>
    </tr>
    <tr>
        <td><code>middle</code></td>
        <td>keyword</td>
        <td>Aligns the middle of the element with the baseline plus half the x-height of the parent.</td>
    </tr>
    <tr>
        <td><code>px, em, rem, etc.</code></td>
        <td>length</td>
        <td>Aligns the baseline of the element at the given length above the baseline of its parent.<br><em>Negative values are allowed.</em></td>
    </tr>
    <tr>
        <td><code>%</code></td>
        <td>percentage</td>
        <td>Aligns the baseline of the element at the given percent <em>of the line-height property of the element itself</em> above the baseline of its parent.<br><em>Negative values are allowed.</em></td>
    </tr>
    <tr>
        <td><code>top</code></td>
        <td>keyword</td>
        <td>Align the top of the element and its descendants with the top of the entire line.<br><strong>Vertically aligns the element relative to the entire line rather than relative to its parent.<br>
        That is, the top of the element is aligned with the top of the tallest element on the line</strong></td>
    </tr>
    <tr>
        <td><code>bottom</code></td>
        <td>keyword</td>
        <td>Align the bottom of the element and its descendants with the bottom of the entire line.<br><strong>Vertically aligns the element relative to the entire line rather than relative to its parent.<br>
        That is, the bottom of the element is aligned with the bottom of the lowest element on the line</strong></td>
    </tr>
</table>

`vertical-align` can take the following values for table cells, or for `display: table-cell` elements:

<table>
    <caption><strong><code>vertical-align</code> values for table cells and <code>display: table-cell;</code> elements</strong></caption>
    <tr>
        <th width="25%">Value<br>(for table cells, or display: table-cell;)</th>
        <th>Type</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><code>baseline, sub, super, text-top, text-bottom</code></td>
        <td>keyword</td>
        <td>Align the baseline of the cell with the baseline of all other cells in the row that are baseline-aligned.
        </td>
    </tr>
    <tr>
        <td><code>top</code></td>
        <td>keyword</td>
        <td>Align the top padding edge of the cell with the top of the row.
        </td>
    </tr>
    <tr>
        <td><code>middle</code></td>
        <td>keyword</td>
        <td>Center the padding box of the cell within the row.
        </td>
    </tr>
    <tr>
        <td><code>bottom</code></td>
        <td>keyword</td>
        <td>Align the bottom padding edge of the cell with the bottom of the row.
        </td>
    </tr>
    <tr>
        <td><code>px, em, rem, etc.</code></td>
        <td>length</td>
        <td>Align the baseline of the cell with the baseline of all other cells in the row that are baseline-aligned.
        <br><em>Negative values are allowed.</em></td>
    </tr>
    <tr>
        <td><code>%</code></td>
        <td>percentage</td>
        <td>Align the baseline of the cell with the baseline of all other cells in the row that are baseline-aligned.
        <br><em>Negative values are allowed.</em></td>
    </tr>
</table>

## Examples for Inline elements (`<span>`, `<img>`, `display: inline-block;`, etc.)

View [this page](vertical-align_inline-elements_examples.html) for examples of each vertical-align setting for inline elements per the table above.

## Examples for table cell (`<td>`) or `display: table-cell;` elements.

View [this page](vertical-align_table-cells_commonly-used-values_examples.html) for examples of commonly-used vertical-align settings for table cell (`<td>`) or `display: table-cell;` elements.

## Complex

The [_**last two examples here**_](vertical-align_inline-elements_examples.html) illustrate `vertical-align: top;`, and `vertical-align: bottom;` for inline elements, the effects of which are a little harder to visualize without example. Refer to the table above for the description of the effects of these two property/value pairs and observe how the `vertical-align: top;`, or `vertical-align: bottom;` aligned element lines up with either the top of the tallest element, or bottom of the lowest element, respectively, on the line and **not** relative to the parent element.

## Notes

[Reference 7]() is an excellent reference for exhaustive detail on often-confounding situations for using `vertical-align` with inline elements.

## Browser Support as of this writing

This CSS property is supported in effectively all browsers (since IE6+, Firefox 2+, Chrome 1+ etc).

**References:**

1. [vertical-align - developer.mozilla.org][ref1]  
2. [vertical-align - css-tricks.com][ref2]  
3. [CSS vertical-align Property - www.w3schools.com][ref3]  
4. [CSS Baseline: The Good, The Bad And The Ugly][ref4]  
5. [Centering in the Unknown - css-tricks.com][ref5]  
6. [Understanding vertical-align, or "How (Not) To Vertically Center Content"][ref6]  
7. [Vertical-Align: All You Need To Know][ref7]  
8. [vertical-align (CSS property)][ref8]  

[ref1]:https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align
[ref2]:https://css-tricks.com/almanac/properties/v/vertical-align/
[ref3]:http://www.w3schools.com/cssref/pr_pos_vertical-align.asp
[ref4]:https://www.smashingmagazine.com/2012/12/css-baseline-the-good-the-bad-and-the-ugly/
[ref5]:https://css-tricks.com/centering-in-the-unknown/
[ref6]:http://phrogz.net/css/vertical-align/
[ref7]:http://christopheraue.net/2014/03/05/vertical-align/
[ref8]:https://www.sitepoint.com/web-foundations/vertical-align-css-property/



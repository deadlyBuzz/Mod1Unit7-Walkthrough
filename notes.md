# Notes
These are notes for the program designed to appear with each commit of the program.

1. 2026-06-14  22:49 Added the width to show results.
> Will cause the final box width to be 340px (300 + 2*20 padding)

2. 2026-06-14  22:52 Using Emvedded "Box Sizing"
> Paddin and Border are included in the 300px.

3. 2026-06-14  23:11 Added some font properties.

4. Adding some Child specificitiy
The notes state how the following:
```css
    div p {
        color: darkslategrey;
    }
```
- can access all **&lt;P&gt;** children.
- That it is a Descendant Selector
- It targets **&lt;P&gt;** tags indide any **&lt;DIV&gt;**, at any depth.

This makes sense, however it also has the example: 

```css
div > p {
    font-weight: bold;
}
```
and the comment:
>Direct **&lt;P&gt;** children

This is not clear and obvious, so lets see what it does?.

2026-06-14  23:19 So Far - Both the same.
2026-06-14  23:21 *THIS* one on the other hand, has correctly only applied the BOLD text to the paragraphs indside the DIV, the others inside the article, are not applied.
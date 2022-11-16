# CSS
**CSS** stands for cascading style sheets, and is the language used to add styling to a document, like your HTML page.

## CSS Syntax
CSS is a rule-based language that allows you to select elements and apply your chosen styling to them. Some elements inherit default styling from the browser (h1 headers sizing and font-weight), but CSS allows you to override and customize the styles on your page to make it your own.

## CSS Structure
```
.pink {
    color: pink;
    background-color: black;
}
```
**Selector**: *.pink* in the above example is the selector, and it chooses elements with the class "pink" to apply the chosen rules.
**Property**: *color* and *background-color* are both properties that will have values applied to them for the selected elements.
**Value**: *pink* and *black* are the values for the chosen properties.
**Declaration**: a declaration is composed of a property & value, and the rule applied to a specific selector may have multiple declarations.

## Applying Styles
CSS styling can be applied in multiple ways:
**External**: An external style sheet that is referenced through a < link > element.
**Internal**: Style sheet is contained on the same page within a < style > element.
**Inline**: Styles applied directly to an element using the style attribute.

### Cascading Applcation
Since it's possible to apply styles from multiple sources, the cascading nature of CSS determines which style will be applied when there are conflicting or redundant properties. The last style read will be what gets applied, so knowing the CSS hierarchy is important in ensuring the wanted styles are used.

***Hierarchy***
1. Inline Styles
2. Internal & External style sheets (dependent on order in document)
3. Browswer defaults

# CSS
Cascading Style Sheets

- Type Selector
- ID Selector
- Class Selector

### How to add style to an element?
You can add style to an element by specifying it in the style element and setting a property for it like this:

Type Selector =>
    element {
    property: value;
    }

    selector1, selector2 {
        property: value;
    }

### <div>
The div element is used mainly for design layout purposes unlike the other content elements you have used so far. Add a div element inside the body element and then move all the other elements inside the new div.
The div tag should an id that is to be used for styling in id selector pattern  
<div id="example-id"> </div>

## ID Selector
You can use the id selector to target a specific div element. An id selector is defined by a name with a hash symbol directly in front of it, like this:

ID Selector =>
    #example-id {
    width: 250px;
    }

## Class selector
A class selector is defined by a name with a dot directly in front of it, like this:

.class-name {
  styles
}

To apply the class's styling to the div element, remove the id attribute and add a class attribute to the div element's opening tag. 

## Block level elements
Block-level elements take up the entire width of their parent element.

## Inline elements



## Style nested elements
The p elements are nested in an article element with the class attribute of item.
You can style all the p elements nested anywhere in elements with a class named item like this:

.item p { }
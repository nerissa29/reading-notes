# Readings: HTML Lists, Control Flow with JS, and the CSS Box Model

## Learn HTML: Ordered and unordered list

## When should you use an unordered list in your HTML document?

*Unordered list* creates bulleted lists. It creates a list of items in no order. An unordered list can be used in a group of items in which the order is not required. It can be used in creating grocery lists or to-do lists. 

A good example would be the following, adapted from MDN web docs[^2]:

``` 
<ul>
    <li>Milk</li>
    <li>Cheese
        <ul>
            <li>Blue cheese</li>
            <li>Feta</li>
        </ul>
    </li>
</ul>

```

- Milk
- Cheese
  - Blue cheese
  - Feta
  


## How do you change the bullet style of unordered list items?

The bullet style can be changed through CSS styling. The CSS property *list-style-type* allows the list items to have a different bullet style other than disc. The *list-style-type* property varies from the following: [^3]:

- list-style-type: space-counter;
- list-style-type: disc;
- list-style-type: circle;
- list-style-type: "\1F44D"; // thumbs up sign

The bullet style of an unordered list can also be changed by creating nested lists of items. A good example would be:

***Nesting lists of items***

```
<ul>
    <li>Eggs</li>
    <li>Yogurt</li>
    <li>Bread
        <ul>
            <li>Spanish bread</li>
            <li>Loaf Bread</li>
        </ul>
    </li>
</ul>
```


## When should you use an ordered list vs an unordered list in your HTML document?

*Ordered list* is useful when describing steps, making it easier for the user to follow through. It creates a list in a specific, numerical or alphabetical order. The ordered list is good for creating a recipe, footnotes, or steps in building something. 

A good example would be the following, adapted from MDN web docs[^1]:

``` 

<ol>
  <li>Mix flour, baking powder, sugar, and salt.</li>
  <li>In another bowl, mix eggs, milk, and oil.</li>
  <li>Stir both mixtures together.</li>
  <li>Fill muffin tray 3/4 full.</li>
  <li>Bake for 20 minutes.</li>
</ol>

```

1. Mix flour, baking powder, sugar, and salt.
2. In another bowl, mix eggs, milk, and oil.
3. Stir both mixtures together.
4. Fill muffin tray 3/4 full.
5. Bake for 20 minutes.


*Unordered list* is useful when the list of items is not necessarily needed in numerical or alphabetical order. It can be used to emphasize important key points or information, making it easier for the user to read. It is best used when the order is not required or doesn't matter.

``` 

<ul>
  <li>Things to bring:
    <ul>
      <li>Towels</li>
      <li>Change of clothes</li>
      <li>Snacks</li>
      <li>Drinks</li>
    </ul>
  </li>
</ul>

```


## Describe two ways you can change the numbers on list items provided by an ordered list?

- Nesting list of items - the example below is adapted from MDN web docs[^1]

```
<ol>
  <li>first item</li>
  <li>second item  <!-- closing </li> tag not here! -->
    <ol>
      <li>second item first subitem</li>
      <li>second item second subitem</li>
      <li>second item third subitem</li>
    </ol>
  </li>            <!-- Here's the closing </li> tag -->
  <li>third item</li>
</ol>
```

- Another way to change the numbers on list would be by using the ***type attribute*** and is written like[^1]:

```

<ol type="A">
  <li>Introduction</li>
  <li>Contents</li>
  <li>Conclusion</li>
</ol>

```

Results would be:
A. Introduction
B. Contents
C. Conclusion

Other ***type attributes*** include:
- i - lowercase Roman numerals
- I - uppercase Roman numerals
- 1 - numbers
- a - lowercase letters
- A - uppercase letters
    




## References:

[^1]: [The Ordered List element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
[^2]: [The Unordered List element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)
[^3]: [MDN: list-style-type](https://developer.mozilla.org/en-US/docs/Web/CSS/list-style-type)
 

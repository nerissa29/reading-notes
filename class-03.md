# Readings: HTML Lists, Control Flow with JS, and the CSS Box MOdel

## Learn HTML: Ordered and unordered list

## When should you use an unordered list in your HTML document?

Ordered list is useful when describing steps, making it easier for the user to follow through. It ceates a list in a specific, with numerical or alphabetical order. Ordered list is good to use when creating a recipe, footnotes, or steps in building something. 

A good example would be the folloowing, adapted from MDN web docs[^1]:

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

Unordered list on the other hand, creates a bulleted lists. It creates list of items in no order. Unordered list can be used in group of items in which the order is not required. It can be used in creating grocery lists, or to-do list. 

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

-Milk
-Cheese
--Blue cheese
--Feta


## References:

[^1]: [<ol>: The Ordered List element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
[^2]: [<ul>: The Unordered List element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)


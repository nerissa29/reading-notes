## Reading Notes 8

### Learn CSS - Flexbox

#### Flexbox is designed for one-dimensional content. Explain what this means.

Flexbox is design for laying out groups of items in one dimension; it can control the alignment and spacing (distributing space) between items that are within the container. It provides flexible boundaries between its content[^1].

One of the layoout that can be used using the flex-direction is[^1]:
- row: the items lay out as a row.
- row-reverse: the items lay out as a row from the end of the flex container.
- column: the items lay out as a column.
- column-reverse : the items lay out as a column from the end of the flex container.

#### Explain the difference between the main axis and cross axis.

The *main axis* is set by *flex-direction* property. If it's a row, *mainaxis* "is along the row", and it it's a column, *main axis* "is along the column"[^1]. The *cross axis* on the other hand, runs in the opposite direction of the *main axis*; if *flex-deirection* for example is row, then the *cross axis* "runs along the column", it is main axis that follows the flex-direction[^1].

#### How can using certain properties of flexbox negatively impact accessibility?

Using *row-reverse* and *column-reverse* can have negative impacts, especially to screen readers. It changes the visula order, and not the logical order; the keyboard navigation "follows the DOM not the visual display"[^1].


### CSS Layout - Flexbox

#### What are some advantages of using flexbox over float?

- the positioning of child elements are eaiser
- using flexbox, the inside margin (its content) does not collapse with the flex container's margin
- laying out and grouping items together, makes it easier to make changes to the element's order

#### How does this topic connect with your long term goals?

Flexbox helps build and design web pages much easier. It makes it easy for the developer to align and group contents. In laying out the contents/items within the same container, the flexbox helps a lot when it comes to controlling the dimensions since it’s one-dimensional. It’s also easy to control the spacing between the items/contents. 



[^1]: [Flexbox](https://web.dev/learn/css/flexbox/)

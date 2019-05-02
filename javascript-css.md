## Adding a class

To add a class use the `add` method.

This method can be found within the `classList` property that exists for every element.

```javaScript
    Element.classList.add('className')
```

Here's how you would add the `red` class to a paragraph of text:

```html
<p>This is a paragraph of text</p>
```

```javascript
const p = document.querySelector("p");
p.classList.add("red");
```

---

# DOM Traverse

Let's say you want to go to your neighbors house.

What's the fastest and most efficient way to get there?

1. Move from your house to neighbor's house.

1. Lookup their address on Google maps, then walk according to the directions Google gives you.

If you move directly from your house to their house, you're doing the equivalent of traversing the DOM -- selecting one element from a neighboring element.

If you lookup their address on Google, you're doing the equivalent of
`document.query.Selector` to find elements.

Can you guess which method is more efficient?

```html
<div class="neighborhood">
  <div class="your-house">😎</div>
  <div class="neighbor-house">🎉</div>
</div>
```

You probably know the answer--its always easier to move from an element to another (compared do doing a full search). That's the way we traverse the DOM.

You can traverse in three directions:

1. Downwards
1. Sideways
1. Upwards

# Traversing downwards

There are two ways to traverse downwards:

1. `querySelector` or `querySelectorAll`
1. `children`

## querySelector or querySelectorAll

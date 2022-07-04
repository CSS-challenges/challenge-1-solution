# CSS challenge #1 📱 The mobile basic layout

When learning CSS, the most difficult thing is not usually which CSS selectors and properties to apply, but to know **which elements do we apply them to**. 

One of the most beneficial things is to learn which HTML containers to create and how to group the elements in order to make the styling as easier as possible. 

> ⚠️ Note: there are **many** ways to style layouts. This is NOT the only correct way, in fact, there are really advanced techniques for pretty much anything. This will focus on using simple CSS features that you have already seen.

Today we will recreate a really basic mobile layout. We will NOT be doing it responsive (yet):

![](docs/final.png)

Observe 👀:
- The navbar is sticked to the end of the page (even when the user is scrolling down)
- The whole page has the SAME padding and space to the border. It feels homogenic.

---

## What's in the code?

- Basically, a bunch of HTML elements and cards that are not grouped yet. You will fix that later.
- Some basic CSS styling. We have introduced *CSS variables*, a really interesting technique that you will learn today.

In CSS, we can create variables just like in JavaScript. Why? Because writing stuff like "#17c3b2" all the time is really hard to remember, but I do know that I want to apply the "main blue" of my color palette to that specific element.

### How do we create variables?

```css

/* In the root of the page, you create them, as many as you want */
:root {
  --primary-blue: #17c3b2;
  --primary-orange: #fe6d73;
}

/* And then you can use them in anyplace where you would use a color */
h1 {
  color: var(--primary-blue);
}

/* That's it! */

```

⚠️ You **don't** have to create any more variables in this project, but you will use the ones given to you.

---

## Iteration 1: The navbar

Navbars are usually composed of lists, because it makes them very accessible to people browsing through a screen reader (blind, etc.). But that doesn't mean we WANT the list styles, so let's get rid of them:

Add the following:








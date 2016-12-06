# The story-item component

This component renders the view and style found in view.html and style.css inside itself,
using the `nx.middlewares.render` middleware. Styles are scoped to the component by default.
It also uses a custom middleware, that registers the `story-id` and `story` attributes on the element.
Whenever these attributes are found or change value, the element
fetches (if its the id attribute) and displays the matching story.

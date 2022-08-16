# shopping-cart-react

<h2><a href="https://yanshtein.github.io/shopping-cart-react/" rel="nofollow">Live Demo</a></h2>

This project deployed using Heroku, uses a simple responsive React shopping cart app, which consists of a few products and a DB.

<b>Project functionality:</b>
- Search input function enables to lookup items by names, categories, and etc.
Search filters data items in the DB, and returns the filtered items based on the user input.
- Each product, added to cart, added to the number of items currently in cart.
A single method named addToCart is responsible for checking if an item already exist in cart by checking item id and that item index.
If item exist -> the quantity property is increased by one.
Else if item is new -> add the item to the cart state.
- Clicking on the cart icon, opens a modal box containing the items added.
- Each item quantity can be changed in the cart.
The + add button uses addtoCart same method.
The - remove button used removeFromCard method and uses same principle, only if one item left, next time the button will be pressed, the item will be removed completly from the cart. 
- The cart can be emptied by clicking the empty button.
When clicked the cart state will be initialized to 0.
- The checkout button calculates total items prices and shows the final price.
The total var is responsible to map over the cart current state and perform calculation and reduce over the items quantity and price.

![Screenshot](youShop.png)


For my own practice I chose to write the app as simple as I can. 
Currently I am rewriting this same app,
to have more functionality, consist of multiple components rather than one large component.
I also plan to add constructors and prototypes to use items category inheritance in the items filter.

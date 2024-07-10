                      INTERACTIVE SHOPPING LIST
 This is a piece of code tailor made to store shopping list items. It enables a user to access any l
 item he/she wants, add or remove an item from the list according to their desires.
 The program also marks the items that have been purchased and the user can clear the list of the items purchased.  
                      Shoppinglist.html
   This file contains the external link to the picture on the home page.
   The title of the html page,the add item,mark purchases and clear list buttons area also contained herein albeit without the functionality needed for them to seamlessly operate yet.
                      Style.css
    This file contains the necessary css code to add to the visual styles necessary to make the program more appealing to the eye.Parts that make up the CSS page include:
       1.Body
       This part includes the global properties and values that can be applied to the other parts of the css through inheritancr.Also includes properties such as border and border radius which we can use to specify the style, width and color of the outer margins encapsulating the shopping list.
       2.Input elements
       This part serves the purpose of styling the content input in the input field.
       Properties include:
         Input[type="text"]
         Width
         Padding
       3.Button Styles
         Targets the "button" elements in html. All the buttons on the page will be affected by the css styles under this heading. Css styles here include padding and margin-right which adds a margin of 10px to the right side of each button.
       4.Navigation menu styles
         Defines styles for a navigation menu.
         Parts of the navigation menu include:
            ul:
            Includes the list-style-type for removing the default bullet points from the list and padding.
            li:
            includes the display and justify content properties.
            li-purchased:
            This part is used to style items on the'already purchased list' with properties such as text decoration for putting line-through text and background color.

                      Events.js
       The events.js file contains the DOM events for adding items,marking them as purchased and
       clearing the list of the items purchased.
       Parts of the events.js file include:
         1 DOMContentLoaded Event Listener:
           Ensures the JavaScript runs after the HTML document is fully loaded.
           
         2.DOM Element Selection:
         Selects the input field, buttons, and list container from the DOM.

         3.ShoppingList Array:
         Stores the list of shopping items, each as an object with name and purchased properties.

         4.renderList Function:
         Clears the existing list (innerHTML = '').
         Iterates over shoppingList and creates a new <li> element for each item.
         Sets the text content of the <li> to the item name.
         Adds a purchased class to <li> if the item is marked as purchased.
         Adds an event listener to each <li> to toggle the purchased state when clicked.
         Appends each <li> to the list container.

         5.addItem Function:
         Gets the value from the input field, trims any whitespace, and adds it to the shoppingList array as an object with purchased set to false.
         Clears the input field and re-renders the list.
         togglePurchased Function:
         Toggles the purchased state of the item at the given index in the shoppingList array.
         Re-renders the list.

         6.clearList Function:
         Clears the shoppingList array and re-renders the list.

         7.markAllAsPurchased Function:
         Sets the purchased property of all items in the shoppingList array to true.
         Re-renders the list.

         8.Event Listeners:
         Attaches addItem to the click event of the "Add Item" button.
         Attaches clearList to the click event of the "Clear List" button.
         Attaches markAllAsPurchased to the click event of the "Mark All as Purchased" button.

        Result
        The provided code, when combined with the appropriate HTML structure, will create a fully functional shopping list application. Users can add new items, mark them as purchased by clicking on them, mark all items as purchased with a single button click, and clear the list entirely.












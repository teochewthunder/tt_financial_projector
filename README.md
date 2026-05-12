# VueJS Financial Projector (TBA)
This simple application accepts financial input for an entire year and projects accumulated savings.

## JavaScript
- Data
  - `currentIndex`: An integer. Defaults to 0. Meant as a pointer to the current element in `items`.
  - `errors`: An object 
    - `name`: A string. Default empty. Used to store an error message.
    - `amount`: A string. Default empty. Used to store an error message.
  - `items`: An array of objects.
    - `name`: A string. Default empty.
    - `month`: An integer: Defaults to 0. Max 12. Supposed to represent a month of the year, with 0 representing "All".
    - `amount`: An integer: Defaults to 0.
  - `monthItems`: An array. Empty by default
  - `monthItemsTemplate`: An array of 13 objects with the same structure. The first object is a template, and the rest corresponds to each month of the year.
    - `monthName`: A string. Default empty.
    - `itemsIn`: An array of objects, subset of `items`.
    - `itemsInTotal`: A number. Total of `amount` in `itemsIn`.
    - `itemsOut`: An array of objects, subset of `items`.
    - `itemsOutTotal`:  A number. Total of `amount` in `itemsOut`.
    - `cumulative`: A calculated number.
  - months
- Computed
  - sortedItems
- Methods
  - `addUpdateItem()`
  - `removeItem()`
  - `setCurrentIndex()`
  - `sortItemOrder()`

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
  - monthItems
  - monthItemsTemplate
  - months
- Computed
  - sortedItems
- Methods
  - `addUpdateItem()`
  - `removeItem()`
  - `setCurrentIndex()`
  - `sortItemOrder()`

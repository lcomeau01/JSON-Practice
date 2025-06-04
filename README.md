# 🛍️ JSON Product Viewer

**JSON Product Viewer** is a web-based project designed to practice **creating, parsing, and dynamically displaying JSON data** using **JavaScript** and **jQuery**. 
The site reads from a custom `products.json` file and renders a responsive product catalog, with filtering capabilities based on categories.


## Features

- Reads a local JSON file containing product information
- Dynamically generates and displays product cards
- Category dropdown filter that updates view in real-time
- Styled with CSS Grid and interactive hover effects
- Responsive, clean layout

## How It Works

1. On load, the app fetches `products.json` using **jQuery's `.get()`** method.
2. Each product entry is converted into a styled product card.
3. The dropdown is automatically populated with unique category names found in the JSON.
4. When a category is selected, only matching products are displayed.

## File Overview

### `index.html`
- Main webpage file that handles:
  - Loading the product data
  - Populating the dropdown filter
  - Rendering products to the page
- Includes:
  - Embedded CSS for layout and styling
  - Inline JavaScript for parsing and rendering JSON data
  - jQuery for DOM interaction and AJAX requests

### `products.json`
- Custom-written JSON file containing an array of product objects (to practice the correct syntax of JSON) 
- Each product includes:
  - `Name`
  - `Description`
  - `Price`
  - `Categories` (array)

#### Example product entry:
```json
{
  "Name": "Oversized Queen Graphic Tee",
  "Description": "Oversized T-shirt with Queen Logo",
  "Price": "$34.95",
  "Categories": ["Womens Clothes", "Graphic Tees", "Band Tees"]
}

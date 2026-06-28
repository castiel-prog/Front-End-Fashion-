# Atlas Atelier - Fashion Outfit Builder

A modern web application for browsing, previewing, and purchasing curated outfit collections. Users can explore pre-built outfits, see how different clothing pieces combine together, and add items to their cart.

## Features

✨ **Modern UI**
- Dark luxury aesthetic with gradient accents
- Responsive design for desktop and mobile
- Smooth animations and transitions
 **Outfit Browsing**
- 9 curated outfit collections across 6 categories
- Filter by style: All, Casual, Formal, Street Style, Business, Athletic
- High-quality product images

 **Interactive Preview**
- Click "Preview" to open a detailed outfit view
- Visual dots on each clothing item with connecting lines to details
- See item name, category, and individual prices
- Click dots or items to highlight them
- Dynamic preview sizing based on image aspect ratio

**Shopping Cart**
- Real-time cart counter in header
- Add complete outfits to cart
- Cart persists during session

## File Structure
FrontEndFashion/
├── homepage.html # Landing page with hero section
├── build.html # Main outfit builder/browsing page
├── build.css # Styling for build page
├── style.css # Global styles
└── README.md # This file

## How to Use

### View Outfits
1. Open `build.html` in your browser
2. Browse the 9 featured outfit collections
3. Use filter tabs to narrow by style category

### Preview an Outfit
1. Click the **"Preview"** button on any outfit card
2. View the full outfit image with interactive dots
3. Click any dot or item in the sidebar to highlight it
4. See connecting lines showing which piece is which
5. Close with the X button or click outside the modal

### Add to Cart
1. Click **"Add to Cart"** on an outfit
2. Watch the cart counter in the header increase
3. The number shows total items in cart

### Navigate
- Click the **Atlas Atelier** logo to return to homepage
- Use navigation links: Build, Brands, Lookbook, About
- Cart icon shows current item count

## Customization Guide

### Adjust Dot Positions
Edit the `pos` values in `build.html` within each outfit's `pieces` array:

```javascript
{ name: 'Oversized Tee', category: 'Top', price: '$45', pos: { x: 40, y: 35 } }
Change Outfit Details


Modify any outfit object:
{
  id: 1,
  category: 'casual',
  title: 'Outfit Name',
  description: 'Outfit description...',
  price: '$XXX',
  image: 'image-url',
  items: 3,
  pieces: [
    { name: 'Item 1', category: 'Type', price: '$XX', pos: { x: XX, y: XX } },
    // ... more pieces
  ]
}
Add New Outfit
Add a new object to the outfits array in build.html:

{
  id: 10,
  category: 'casual',
  title: 'Your Outfit Name',
  description: 'Your description',
  price: '$XXX',
  image: 'your-image-url',
  items: 3,
  pieces: [
    { name: 'Piece 1', category: 'Top', price: '$50', pos: { x: 50, y: 35 } },
    { name: 'Piece 2', category: 'Bottom', price: '$70', pos: { x: 50, y: 60 } },
    { name: 'Piece 3', category: 'Footwear', price: '$80', pos: { x: 50, y: 85 } }
  ]
}
Design Features
Color Scheme: Dark background (#06080b) with warm accent colors (bronze/orange #d67b3a)
Typography: Inter font family for modern, clean look
Animations: Smooth hover effects, dot highlighting, modal transitions
Responsive: Mobile-friendly with breakpoints at 1024px and 640px
Browser Compatibility
Chrome/Edge (latest)
Firefox (latest)
Safari (latest)
Mobile browsers
Future Enhancements
 User authentication and saved favorites
 Individual item pages with detailed specs
 Size and color variants
 Real checkout system with payment integration
 User reviews and ratings
 Styling tips and outfit recommendations
 Social sharing features
 Brand pages and collections
Getting Started
Clone or download the repository
Open homepage.html in a web browser
Click "Build" to explore outfit collections
Customize outfits and images as needed



License
This project is open source and available for personal and commercial use.

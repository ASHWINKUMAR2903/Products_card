# Product_card
## Date: 09.07.25
## Objective:

To replicate a product card layout similar to those found on real-time e-commerce platform like FlipKart using the CSS Box Model (margin, border, padding, and content).

## Tasks:

#### 1. Structure the HTML Layout:
Create a container ```<div>``` for the product card.

Add an ```<img>``` for the product image.

Include ```<h2>``` for product name, ```<p>``` for description, and a ```<span>``` or ```<div>``` for price.

Add a “Buy Now” or “Add to Cart” button.

#### 2. Apply Box Model Styling in CSS:
Use padding inside each section (image, text, button) to ensure readability.

Use margin around the card to space it from the page edges or other cards.

Add a border to outline the card.

Control width and height for consistent sizing.

#### 3. Visual Styling:
Add a background color to the card container.

Use box-shadow to simulate depth (card lifting effect).

Add border-radius for rounded corners.

#### 4. Center the Card:
Use display: flex and justify-content: center and align-items: center on the parent container.

#### 5. Bonus Enhancements:
Use a hover effect on the button (e.g., background color change).

Make the card responsive with percentage-based widths or media queries.
## HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flipkart Clone-Product Card</title>
    <link href="style.css" rel="stylesheet">
</head>
<body>
    <div class="page-container">
    <div class="product-card">
      <img src="img1.webp" alt="Smartphone">
      <h2>Smartphone XYZ</h2>
      <p>6.5" Display, 128GB Storage, 48MP Camera</p>
      <div class="price">₹14,999</div>
      <button>Add to Cart</button>
    </div>

    <div class="product-card">
      <img src="img2.jpg" alt="Headphones">
      <h2>Wireless Headphones</h2>
      <p>Bluetooth 5.0, 40H Battery, Noise Cancellation</p>
      <div class="price">₹2,499</div>
      <button>Add to Cart</button>
    </div>

    <div class="product-card">
      <img src="img3.jpg" alt="Laptop">
      <h2>Laptop ABC 14"</h2>
      <p>Intel i5, 8GB RAM, 512GB SSD, Windows 11</p>
      <div class="price">₹49,999</div>
      <button>Add to Cart</button>
    </div>
  </div>
</body>
</html>
```
## CSS Code:
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f1f3f6;
  padding: 40px 20px;
}

.page-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 150px;
}

.product-card {
  width: 280px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 12px;
  padding: 16px;
  box-shadow: 0 40px 20px rgba(0,0,0,0.08);
  text-align: center;
}

.product-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 6px 16px rgba(0,0,0,0.15);
}

.product-card img {
  width: 100%;
  height: auto;
  border-radius: 10px;
  margin-bottom: 12px;
}

.product-card h2 {
  font-size: 18px;
  margin-bottom: 8px;
  color: #333;
}

.product-card p {
  font-size: 14px;
  color: #555;
  margin-bottom: 10px;
}

.product-card .price {
  font-size: 20px;
  font-weight: bold;
  color: #007b5e;
  margin-bottom: 14px;
}

.product-card button {
  padding: 10px 16px;
  font-size: 14px;
  background-color: #ff9f00;
  border: none;
  color: white;
  border-radius: 6px;
  cursor: pointer;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

.product-card button:hover {
  background-color: #fb641b;
  transform: scale(1.05);
}

@media (max-width: 900px) {
  .page-container {
    justify-content: center;
  }
}
```
## Output:
![image](https://github.com/user-attachments/assets/9f7a0ecf-c162-4330-b882-9ff0829f31ee)

## Result:
A product card layout similar to those found on real-time e-commerce platform like FlipKart using the CSS Box Model is replicated successfully.

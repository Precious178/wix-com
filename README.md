# Wix-Com Project

A responsive website project showcasing various features and responsive design principles.

## Features
- Responsive design for all devices
- Dynamic image scaling
- Flexible layouts
- Mobile-friendly navigation
- Background image optimization

## Technologies Used
- HTML5
- CSS3
- Media Queries
- Flexbox

## Recent Changes - Responsive Implementation

### 1. Basic Responsiveness
We made the website adapt to different screen sizes using `media queries`:
- 1024px (tablets/small laptops)
- 768px (tablets portrait)
- 480px (mobile phones)

Example:

css
@media screen and (max-width: 768px) {
/ Styles for tablet and smaller devices /
}

### 2. Fixed White Space Issue
Added basic CSS rules to prevent unwanted white space:
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    width: 100%;
    max-width: 100vw;
    overflow-x: hidden;
}
```

### 3. Responsive Images
Made images scale properly:
```css
img {
    max-width: 100%;
    height: auto;
    object-fit: contain; /* Keeps original proportions */
}
```

### 4. Layout Adjustments
On smaller screens:
- Menu items stack vertically
- Flex containers change direction
- Text size adjusts for readability
- Centered buttons

Example:
```css
@media screen and (max-width: 768px) {
    .flex {
        flex-direction: column;
        align-items: center;
    }
}
```

### 5. Background Images
Added fallback colors for background images:
```css
.about {
    background-image: url("your-image.jpg");
    background-color: #333; /* Fallback color */
    background-size: cover;
    background-position: center;
}
```

## Results
The website is now:
- ✅ Usable on all devices
- ✅ Readable at all screen sizes
- ✅ Visually consistent
- ✅ No horizontal scrollbars
- ✅ Correct image proportions

## Important Implementation Notes
Always include the viewport meta tag in your HTML:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## Testing
Test your responsive design using:
1. Browser developer tools
2. Real devices
3. Different screen orientations
4. Various browsers

## Installation
1. Clone the repository
2. Open index.html in your browser
3. No additional dependencies required

## Contributing
Feel free to submit issues and enhancement requests.

## License
[Add your license here]

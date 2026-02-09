# PRODIGY_WD_01 - Interactive E-Commerce Navigation Menu

An elegant and fully responsive e-commerce website navigation menu featuring dynamic scroll effects, smooth hover animations, and interactive elements. Built with pure HTML, CSS, and JavaScript.

![Project Banner](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Key Functionalities](#key-functionalities)
- [Responsive Design](#responsive-design)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🎯 Overview

This project showcases a modern e-commerce website navigation system that enhances user experience through interactive design patterns. The navigation menu adapts to user scrolling behavior and provides visual feedback on hover interactions, creating an engaging shopping experience.

**Project Type:** Web Development Internship Task  
**Task ID:** PRODIGY_WD_01  
**Objective:** Create an interactive navigation menu that changes color or style when scrolled or hovering over menu items

## ✨ Features

### Navigation Components
- **Three-Tier Navigation Structure**
  - Top promotional bar with contact information and quick links
  - Main navigation with logo, search bar, and user icons
  - Category menu with product sections

### Interactive Elements
- **Scroll-Based Effects**
  - Navigation background color transitions on scroll
  - Top bar auto-hides when scrolling down
  - Compact navigation layout after scroll threshold
  - Enhanced shadow effects for depth

- **Hover Animations**
  - Category menu items lift on hover with underline animation
  - Icon scaling and rotation effects
  - Product cards elevate with shadow enhancement
  - Button color transitions and scaling

- **Shopping Features**
  - Live shopping cart counter
  - Wishlist functionality with badge
  - Product grid with pricing and ratings
  - Add to cart with visual confirmation
  - Search functionality with smooth interactions

### User Experience
- Smooth scroll-to-section navigation
- Active category highlighting
- Dynamic cart counter updates
- Visual feedback on all interactions
- Fixed position for constant accessibility

### Quick Preview
- Navigate through different sections
- Scroll to see the navigation transform
- Hover over menu items and icons
- Click "Add to Cart" to see the counter update
- Test the search functionality

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | Structure and semantic markup |
| CSS3 | Styling, animations, and responsive design |
| JavaScript | Interactivity and dynamic functionality |
| Git | Version control |
| GitHub | Code hosting and collaboration |

### CSS Features
- Flexbox for layout
- CSS Grid for product display
- CSS Transitions and Transforms
- Custom animations
- Media queries for responsiveness
- Linear gradients

### JavaScript Features
- DOM manipulation
- Event listeners (scroll, click, hover)
- Dynamic class toggling
- Smooth scrolling
- Real-time counter updates

## 📥 Installation

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- Text editor or IDE (VS Code recommended)
- Git (optional, for cloning)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/shindeshridhar07-walle/PRODIGY_WD_01.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd PRODIGY_WD_01
   ```

3. **Open the file**
   - Simply open `ecommerce-nav.html` in your web browser
   - Or use Live Server extension in VS Code

### Alternative: Download ZIP
- Click the green "Code" button on GitHub
- Select "Download ZIP"
- Extract and open `ecommerce-nav.html`

## 💻 Usage

### Basic Usage
1. Open `ecommerce-nav.html` in any modern web browser
2. Scroll down to see the navigation menu transform
3. Hover over menu items to see interactive effects
4. Click on category links to navigate
5. Try the search bar and shopping cart features

### Customization

#### Changing Colors
Edit the CSS variables in the `<style>` section:
```css
/* Example: Change primary color */
.navbar {
    background-color: #YOUR-COLOR;
}

.category-nav {
    background-color: #YOUR-COLOR;
}
```

#### Modifying Categories
Update the category menu in HTML:
```html
<li class="category-item">
    <a href="#your-category" class="category-link">Your Category</a>
</li>
```

#### Adding Products
Duplicate the product card structure:
```html
<div class="product-card">
    <div class="product-image">ICON</div>
    <div class="product-info">
        <div class="product-name">Product Name</div>
        <div class="product-rating">⭐⭐⭐⭐⭐</div>
        <div class="product-price">$XX.XX</div>
        <button class="add-to-cart-btn">Add to Cart</button>
    </div>
</div>
```

## 📁 Project Structure

```
PRODIGY_WD_01/
│
├── ecommerce-nav.html    # Main HTML file with embedded CSS and JS
├── README.md             # Project documentation
└── screenshots/          # Screenshots folder (optional)
    ├── desktop-view.png
    ├── mobile-view.png
    └── scroll-effect.png
```

## 🔑 Key Functionalities

### 1. Scroll Detection
```javascript
window.addEventListener('scroll', function() {
    if (window.scrollY > 50) {
        navbar.classList.add('scrolled');
    } else {
        navbar.classList.remove('scrolled');
    }
});
```

### 2. Active Category Tracking
```javascript
categoryLinks.forEach(link => {
    link.addEventListener('click', function(e) {
        categoryLinks.forEach(l => l.classList.remove('active'));
        this.classList.add('active');
    });
});
```

### 3. Cart Counter Update
```javascript
addToCartButtons.forEach(button => {
    button.addEventListener('click', function() {
        cartCount++;
        cartBadge.textContent = cartCount;
    });
});
```

### 4. Smooth Scrolling
```javascript
document.querySelector(href).scrollIntoView({
    behavior: 'smooth',
    block: 'start'
});
```

## 📱 Responsive Design

The navigation menu is fully responsive and adapts to different screen sizes:

| Screen Size | Behavior |
|-------------|----------|
| Desktop (>968px) | Full navigation with all features |
| Tablet (768px-968px) | Hidden search bar, wrapped categories |
| Mobile (<768px) | Compact layout, smaller fonts, stacked elements |

### Breakpoints
- **968px**: Search bar hidden, categories wrap
- **768px**: Condensed top bar, smaller navigation elements

## 🚧 Future Enhancements

- [ ] Add dropdown mega menus for categories
- [ ] Implement actual shopping cart functionality
- [ ] Add user authentication system
- [ ] Create product detail pages
- [ ] Integrate payment gateway
- [ ] Add product filtering and sorting
- [ ] Implement wishlist persistence using localStorage
- [ ] Add dark mode toggle
- [ ] Create admin dashboard
- [ ] Multi-language support

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👤 Contact

**Your Name**
- GitHub: [@YOUR-USERNAME](https://github.com/shindeshridhar07-walle)
- LinkedIn: [Your LinkedIn](https://www.linkedin.com/in/shridhar-shinde)
- Email: shindeshridhar07@gmail.com

**Project Link:** (https://github.com/shindeshridhar07-walle/PRODIGY_WD_01.git)

---

## 🙏 Acknowledgments

- Prodigy InfoTech for the internship opportunity
- Icons and emojis from Unicode standard
- Inspiration from modern e-commerce platforms
- Community feedback and suggestions

---

### 📌 Note
This project was created as part of the Prodigy InfoTech Web Development Internship Program.

**Task:** Create an interactive navigation menu  
**Completion Date:** February 2026  
**Status:** ✅ Completed

---

<div align="center">
  <p>Made with ❤️ by [Your Name]</p>
  <p>⭐ Star this repository if you found it helpful!</p>
</div>

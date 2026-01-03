# Guitar Tuner Headquarters

A comprehensive, modern directory website for guitar tuners featuring free online tools, mobile apps, physical tuners for purchase, and educational resources.

![Guitar Tuner HQ](https://img.shields.io/badge/version-1.0.0-orange) ![License](https://img.shields.io/badge/license-MIT-blue)

## 🎸 Features

- **Modern Dark Theme Design** - Sleek interface with gold accent colors
- **Responsive Layout** - Works perfectly on desktop, tablet, and mobile devices
- **Four Main Sections:**
  - 📱 Free Online Guitar Tuners
  - 📲 Mobile Tuner Apps (iOS & Android)
  - 🛒 Physical Tuners for Sale
  - 📚 Learning Resources & Tutorials
- **Blog-Style Commentary** - Educational content about tuning and ear training
- **Smooth Animations** - Scroll-triggered animations for engaging user experience
- **SEO Optimized** - Proper meta tags and semantic HTML

## 🚀 Quick Start

### View the Site Locally

1. Clone this repository:
```bash
git clone https://github.com/yourusername/guitar-tuner-hq.git
cd guitar-tuner-hq
```

2. Open `index.html` in your web browser:
   - Double-click the file, or
   - Right-click and select "Open with" your preferred browser

That's it! No build process or dependencies required.

### Deploy to GitHub Pages

1. Go to your repository settings on GitHub
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select the main branch
4. Click "Save"
5. Your site will be live at `https://yourusername.github.io/guitar-tuner-hq/`

## 📁 Project Structure

```
guitar-tuner-hq/
├── index.html          # Main HTML file with embedded CSS and JavaScript
├── README.md           # This file
├── LICENSE             # MIT License
└── .gitignore         # Git ignore file
```

## 🎨 Customization

### Change Colors

Edit the CSS variables in the `<style>` section of `index.html`:

```css
:root {
    --bg-primary: #0a0a0a;        /* Main background color */
    --bg-secondary: #161616;       /* Card background color */
    --accent-primary: #f59e0b;     /* Primary accent (gold) */
    --accent-secondary: #d97706;   /* Secondary accent */
    --text-primary: #f5f5f5;       /* Main text color */
    --text-secondary: #a3a3a3;     /* Secondary text color */
}
```

### Add Your Own Content

- **Online Tuners**: Modify the cards in the `#online-tuners` section
- **Apps**: Update the `#tuner-apps` section with different apps
- **Products**: Edit the `#tuners-for-sale` section to feature different products
- **Learning Resources**: Customize the `#learning-resources` section

### Add Images

To add product images, insert an `<img>` tag in each card:

```html
<div class="card">
    <span class="card-badge">Best Seller</span>
    <img src="path/to/image.jpg" alt="Product name" class="card-image">
    <h3>Product Name</h3>
    <!-- rest of card content -->
</div>
```

Then add this CSS for image styling:

```css
.card-image {
    width: 100%;
    height: 200px;
    object-fit: contain;
    border-radius: 8px;
    margin-bottom: 1.5rem;
}
```

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS Grid and Flexbox
- **Vanilla JavaScript** - Smooth scrolling and scroll-reveal animations
- **Google Fonts** - Bebas Neue and Outfit font families

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Font families from [Google Fonts](https://fonts.google.com/)
- Product information sourced from manufacturer websites
- Educational resources linked from reputable guitar learning platforms

## 📧 Contact

For questions or suggestions, please open an issue on GitHub.

---

**Note:** This is an educational project. All product information and prices are for demonstration purposes. Visit manufacturer websites for current pricing and availability.

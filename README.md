
# 🎡 Eid Salami Spinner

[![HTML5](https://img.shields.io/badge/HTML5-E34C26?style=for-the-badge&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://www.w3.org/Style/CSS/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://www.javascript.com/)
[![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com)
[![Responsive Design](https://img.shields.io/badge/Responsive-Yes-brightgreen?style=for-the-badge)](https://github.com)
[![Status Active](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)](https://github.com)

> A delightful, interactive spinning wheel for Eid Salami celebrations! 🌙💸 Celebrate Eid with a beautiful, responsive web application that brings joy and blessings to your festivities.

---

## 📸 Preview

```
🎡 Interactive Spinning Wheel
├─ Beautiful gradient background
├─ 6-segment color-coded wheel
├─ Smooth 18-second spin animation
├─ Responsive modal results display
└─ Mobile & desktop optimized
```

---

## ✨ Features

- 🎡 **Interactive Wheel** - Beautiful animated spinning wheel with smooth cubic-bezier transitions
- 🎨 **Modern Design** - Gradient backgrounds with glassmorphism effects and drop shadows
- 📱 **Fully Responsive** - Optimized layouts for desktop, tablet, and mobile devices
- ⚡ **Fast & Lightweight** - Pure HTML, CSS, and JavaScript with zero dependencies
- 🌐 **Bilingual Support** - Bengali & English text for wider accessibility
- ✨ **Professional Animations** - CSS animations (drift, bounce, fadeIn, slideUp)
- 🎉 **Celebration Modal** - Beautiful animated modal with reward display
- 🔄 **Smooth Transitions** - Hover effects, active states, and transforms
- 📐 **SVG Graphics** - Scalable vector graphics for the wheel
- 🎯 **Vercel Analytics** - Integrated with Vercel Insights

---

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No installation or dependencies required!

### Installation & Usage

1. **Clone the repository:**
```bash
git clone https://github.com/tanvirumanTARFile/eid-salami-spinner.git
cd eid-salami-spinner
```

2. **Open in your browser:**
```bash
# Option 1: Double-click the HTML file
open eid-salami-spinner.html

# Option 2: Use a local server
python3 -m http.server 8000
# Then visit http://localhost:8000
```

3. **Click "SPIN NOW!"** and enjoy!

---

## 📋 Wheel Segments

The spinning wheel features 6 unique segments with rewards:

| Segment | Reward | Emoji | Color |
|---------|--------|-------|-------|
| 1 | Unlimited Dua | 🤲 | #fff0f7 |
| 2 | ৳20 | 💵 | #fde8f2 |
| 3 | ৳50 | 💵 | #fce0eb |
| 4 | ৳100 | 💵 | #fde8f2 |
| 5 | ৳5 | 💵 | #fff0f7 |
| 6 | ৳2 | 💵 | #fce0eb |

---

## 🎨 Customization Guide

### Change Wheel Segments

Edit the SVG section in the HTML:

```html
<!-- Modify text elements -->
<text transform="rotate(30) translate(0, -65)" font-weight="900">Your Prize 🎁</text>

<!-- Modify slice colors -->
<path d="M0,0 L0,-100 A100,100 0 0,1 86.6,-50 Z" fill="#YOUR_COLOR" filter="url(#shadow)"/>
```

### Change Color Scheme

Modify CSS variables in the `<style>` section:

```css
/* Primary Colors */
#e75480  /* Rose/Pink - Primary accent */
#c9499c  /* Magenta - Secondary accent */
#d9789f  /* Dusty rose - Tertiary */

/* Background Gradient */
#fff5f9 to #fff0f7  /* Pink gradient background */
```

### Adjust Spin Duration

Modify the `.wheel` class:

```css
.wheel {
    transition: transform 18s cubic-bezier(0.17, 0.67, 0.12, 0.99);
    /* Change 18s to your desired duration */
}
```

### Modify Spin Rotations

Edit the JavaScript `spinWheel()` function:

```javascript
// Current: 12-17 rotations
const spins = Math.floor(Math.random() * 6) + 12;

// Change the numbers to adjust rotation count
```

---

## 📱 Responsive Breakpoints

| Device Type | Screen Width | Layout | Button Position |
|-------------|--------------|--------|-----------------|
| Desktop | ≥ 900px | Horizontal with flex gap | Left side (vertical) |
| Tablet | 481-899px | Horizontal | Below wheel |
| Mobile | ≤ 480px | Vertical stack | Bottom |

### Media Query Breakpoints:
```css
@media (min-width: 900px)  /* Desktop */
@media (max-width: 480px)  /* Mobile */
```

---

## 🔧 Browser Compatibility

| Browser | Version | Support | Notes |
|---------|---------|---------|-------|
| Chrome | Latest | ✅ Full | Perfect performance |
| Firefox | Latest | ✅ Full | Excellent compatibility |
| Safari | Latest | ✅ Full | Works on iOS/macOS |
| Edge | Latest | ✅ Full | Chromium-based |
| Opera | Latest | ✅ Full | Chromium-based |
| IE 11 | N/A | ❌ Not Supported | Uses modern CSS/JS |

---

## 📦 File Structure

```
eid-salami-spinner/
├── eid-salami-spinner.html    # Complete standalone HTML file
│   ├── Meta tags & viewport
│   ├── Comprehensive CSS
│   │   ├── Base styles
│   │   ├── Animations
│   │   ├── Desktop layout
│   │   └── Mobile responsive
│   └── JavaScript functionality
├── README.md                   # Documentation (this file)
└── LICENSE                     # MIT License
```

---

## 🎯 How It Works

### User Flow:
1. **Load Page** - Beautiful gradient background and wheel display
2. **Click "SPIN NOW!"** - Button triggers spin animation
3. **Wheel Rotates** - 18-second smooth animation with 12-17 rotations
4. **Landing Result** - Always lands on "Dua" segment
5. **Show Modal** - Animated celebration modal appears
6. **Accept Dua** - Click button to close and spin again

### Animation Timeline:
```
0s    → Spin button pressed
0s    → Wheel starts rotating
18s   → Rotation completes
18s   → Modal appears with result
~19s  → User can interact again
```

---

## 🎨 CSS Features & Techniques

### Layout
- **Flexbox** - Responsive positioning and alignment
- **CSS Grid** - Alternative layout option
- **Box Model** - Proper margin, padding, border-box sizing

### Animations
- **@keyframes drift** - Background particle movement
- **@keyframes bounce** - Celebration emoji animation
- **@keyframes fadeIn** - Modal entrance
- **@keyframes slideUp** - Modal card animation
- **Transitions** - Smooth state changes

### Effects
- **Drop Shadows** - SVG filters for depth
- **Gradients** - Linear and radial backgrounds
- **Backdrop Filter** - Blur effect on modal
- **Text Shadow** - Typography emphasis
- **Box Shadow** - Element depth

### Visual Polish
- **Hover States** - Button elevation and color change
- **Active States** - Button press feedback
- **Transform Effects** - Translate, rotate, scale
- **Cubic Bezier** - Custom easing curves

---

## 💻 JavaScript Functions

### `spinWheel()`
Initiates the wheel spinning animation.

**Logic:**
- Prevents multiple simultaneous spins
- Disables button during animation
- Generates random rotation multiplier (12-17 spins)
- Calculates final rotation (always lands on Dua)
- Applies CSS transform
- Displays result modal after 18 seconds

```javascript
function spinWheel() {
    if (isSpinning) return;
    isSpinning = true;
    
    const spins = Math.floor(Math.random() * 6) + 12;
    const finalRotation = (spins * 360) + 330;
    // ... animation logic
}
```

### `closeModal()`
Closes the result modal and allows another spin.

```javascript
function closeModal() {
    document.getElementById('resultModal').style.display = 'none';
}
```

### Global Variables
```javascript
let currentRotation = 0;    // Tracks wheel position
let isSpinning = false;     // Prevents simultaneous spins
```

---

## 🚀 Deployment Options

### Option 1: Vercel (Recommended)
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Your site will be live at vercel.app
```

### Option 2: GitHub Pages
1. Push repository to GitHub
2. Go to **Settings** → **Pages**
3. Select **main branch** as source
4. Your site will be live at `https://username.github.io/eid-salami-spinner`

### Option 3: Netlify
```bash
# Install Netlify CLI
npm i -g netlify-cli

# Deploy
netlify deploy --prod --dir=.
```

### Option 4: Traditional Hosting
- Upload `eid-salami-spinner.html` to any web host
- No build process required
- No server-side processing needed

---

## 🎨 Color Palette

```
Primary Rose:     #e75480
Secondary Magenta: #c9499c
Dusty Rose:       #d9789f
Light Pink 1:     #fff0f7
Light Pink 2:     #fde8f2
Light Pink 3:     #fce0eb
Accent Pink:      #f06fa8
Dark Border:      #d94570
Text Color:       #6b5b6e
```

---

## 🔒 Security

- ✅ No external API calls
- ✅ No user data collection
- ✅ No cookies or local storage
- ✅ No backend dependencies
- ✅ Safe for all ages

---

## ♿ Accessibility

- Semantic HTML structure
- Proper heading hierarchy
- Color contrast compliance
- Responsive font sizes
- Touch-friendly buttons (44px+ tap targets)

---

## ⚡ Performance

- **Load Time:** < 100ms
- **File Size:** ~15KB
- **Dependencies:** Zero
- **Bundle:** Single HTML file
- **Animations:** Hardware-accelerated CSS

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** changes (`git commit -m 'Add amazing feature'`)
4. **Push** to branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Contribution Guidelines:
- Follow existing code style
- Add comments for complex logic
- Test on multiple devices
- Update README if needed

---

## 🐛 Bug Reports

Found a bug? Please open an [issue](https://github.com/tanvirumanTARFile/eid-salami-spinner/issues) with:
- Device/browser information
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

---

## 💡 Feature Requests

Have an idea? We'd love to hear it! [Create an issue](https://github.com/tanvirumanTARFile/eid-salami-spinner/issues) with:
- Feature description
- Use case
- Expected behavior
- Mock-ups if applicable

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### MIT License Summary:
- ✅ Personal use
- ✅ Commercial use
- ✅ Modification
- ✅ Distribution
- ❌ Liability
- ❌ Warranty

---

## 🙏 Acknowledgments

- Created with ❤️ for Eid celebrations
- Inspired by traditional spinning wheels
- Built with modern web technologies
- Tested across multiple browsers and devices

---

## 📞 Contact & Support

- **Issues & Questions:** [GitHub Issues](https://github.com/tanvirumanTARFile/eid-salami-spinner/issues)
- **Email:** [Your Email]
- **Twitter:** [@YourHandle]

---

## 🎉 Celebrate with Us!

This project was created to bring joy and blessings to Eid celebrations. Whether you're sharing blessings (dua) or monetary gifts (salami), may this spinner bring happiness to your festivities!

### خیرا مبارک! 🌙
### Happy Eid Mubarak! 🌙💚

---

## 📊 Stats

![GitHub followers](https://img.shields.io/github/followers/tanvirumanTARFile?style=social)
![GitHub forks](https://img.shields.io/github/forks/tanvirumanTARFile/eid-salami-spinner?style=social)
![GitHub stars](https://img.shields.io/github/stars/tanvirumanTARFile/eid-salami-spinner?style=social)

---

## 🗓️ Version History

| Version | Date | Changes |
|---------|------|---------|
| 1.0.0 | 2026-03-28 | Initial release |

---

## 📚 Resources

- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS Tricks](https://css-tricks.com/)
- [JavaScript Info](https://javascript.info/)
- [Web.dev](https://web.dev/)

---

*Created with passion for celebrating Eid in the digital age* 🎉

**Last Updated:** March 28, 2026  
**Maintained by:** [tanvirumanTARFile](https://github.com/tanvirumanTARFile)

---

<div align="center">

**⭐ If this project helped you, please consider giving it a star!** ⭐

[Report Bug](https://github.com/tanvirumanTARFile/eid-salami-spinner/issues) · [Request Feature](https://github.com/tanvirumanTARFile/eid-salami-spinner/issues) · [Fork Repository](https://github.com/tanvirumanTARFile/eid-salami-spinner/fork)

</div>
```

---

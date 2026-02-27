# Advanced HTML & CSS Assignment - Complete Project

**Student Name:** Sejal Singh  
**Course:** Advanced Frontend Development  
**Topic:** Advanced HTML5 & CSS3  
**Submission Date:** 27th February 2026

---

## 📋 Project Overview

This is a comprehensive advanced HTML & CSS assignment featuring:
- **Section A:** Advanced HTML Theory (Semantic HTML, ARIA, Forms, Meta Tags, etc.)
- **Section B:** Advanced CSS Theory (Specificity, Box Model, Positioning, Custom Properties, etc.)
- **Section C:** Advanced Layout Practical Examples (12-column Grid, Masonry, Layouts, etc.)
- **Section D:** Advanced Effects & Animations (Buttons, Spinners, Gradients, 3D Effects)
- **Section E:** Media Queries & Responsive Design (Mobile-first, Dark Mode, Accessibility)
- **Section F:** Final Master Project (Complete Responsive Website)

---

## 📁 Project Structure

```
Sejal_Advanced_HTML_CSS_Assignment/
├── README.md (This file)
├── practical-tasks/
│   ├── 01-semantic-blog-page.html
│   ├── 02-accessible-navigation.html
│   ├── 03-complex-form.html
│   ├── 04-faq-details.html
│   ├── 05-responsive-images.html
│   ├── 06-accessible-video.html
│   └── css/
│       ├── 01-semantic-blog.css
│       ├── 02-accessible-navigation.css
│       ├── 03-complex-form.css
│       ├── 04-faq-details.css
│       ├── 05-responsive-images.css
│       └── 06-accessible-video.css
└── final-master-project/
    ├── index.html
    ├── css/
    │   └── master-project.css
    └── assets/ (Images and media)
```

---

## 🎯 Key Features Implemented

### 1. **Semantic HTML Structure**
- Proper use of `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`
- Schema.org microdata markup for SEO
- Proper heading hierarchy (h1-h6)
- Meaningful link text

### 2. **Accessibility (WCAG 2.1 Level AA Compliant)**
- ARIA roles and attributes (`role`, `aria-label`, `aria-labelledby`, `aria-describedby`)
- Proper form labels and fieldsets
- Color contrast ratios > 4.5:1 (normal text) / 3:1 (large text)
- Keyboard navigation support
- Skip links for navigation
- Alt text for all images
- Captions for videos

### 3. **Responsive Design**
- **Mobile-first approach** (base styles for mobile, enhanced with media queries)
- **4 Main Breakpoints:**
  - Mobile: 480px
  - Tablet: 768px
  - Desktop: 1024px
  - Large Desktop: 1440px
- CSS Grid and Flexbox layouts
- Fluid typography using `clamp()`
- Responsive images with `srcset` and `picture` element

### 4. **Advanced CSS Techniques**
- CSS Custom Properties (Variables)
- CSS Grid Layout System
- Flexbox Layout
- CSS Animations and Transitions
- Backdrop effects (Glassmorphism, Neumorphism)
- CSS containment
- Logical properties
- Box model and stacking context

### 5. **Dark Mode Support**
- Implemented via `prefers-color-scheme` media query
- CSS variables for theme colors
- Automatic detection and switching
- Optional manual toggle button

### 6. **Performance Optimizations**
- Semantic HTML reduces DOM size
- CSS variables for maintainability
- Optimized media queries
- Minimal repaints and reflows
- Critical CSS approach
- Lazy loading support

### 7. **Browser Compatibility**
- Modern CSS features with fallbacks
- Support for latest browsers
- Progressive enhancement
- Multiple image formats (WebP with PNG fallback)

---

## 🔗 Responsive Breakpoints Used

### Mobile-First Approach

```css
/* Mobile (default) - 320px to 479px */
/* Base styles apply to all devices */

/* Tablet - 480px to 767px */
@media (min-width: 480px) { ... }

/* Tablet Large - 768px to 1023px */
@media (min-width: 768px) { ... }

/* Desktop - 1024px to 1439px */
@media (min-width: 1024px) { ... }

/* Large Desktop - 1440px and above */
@media (min-width: 1440px) { ... }
```

### Fluid Typography

```css
/* Example: Scales between 1.5rem (mobile) and 3rem (desktop) */
h1 {
  font-size: clamp(1.5rem, 5vw, 3rem);
}
```

---

## ♿ Accessibility Features

### 1. **HTML Accessibility**
- ✅ Semantic elements instead of div-soup
- ✅ Proper form structure with `<fieldset>` and `<legend>`
- ✅ `<label>` elements associated with form inputs
- ✅ Required field indicators
- ✅ Pattern validation with helpful hints
- ✅ Datalist for autocomplete
- ✅ Details/summary for FAQ sections

### 2. **ARIA Implementation**
- ✅ `aria-label` for buttons and icons
- ✅ `aria-labelledby` for sections with visible headings
- ✅ `aria-describedby` for form help text
- ✅ `aria-required` for required fields
- ✅ `aria-expanded` for dropdowns and menus
- ✅ `aria-current="page"` for navigation
- ✅ `aria-live` for dynamic content updates

### 3. **Keyboard Navigation**
- ✅ All interactive elements are keyboard accessible
- ✅ Logical tab order
- ✅ Focus indicators with sufficient contrast
- ✅ Skip links for main content
- ✅ Keyboard shortcuts for video controls

### 4. **Color & Contrast**
- ✅ All text meets WCAG AA standards (4.5:1 ratio)
- ✅ Color is not the only means of conveying information
- ✅ Dark mode support for reduced eye strain
- ✅ High contrast mode support

### 5. **Media & Content**
- ✅ Video captions with multiple languages
- ✅ Audio transcripts
- ✅ Image alt text
- ✅ Descriptive link text
- ✅ Proper heading hierarchy

---

## 🎨 Design System & CSS Variables

### Color Palette
```css
--primary: #3498db (Action buttons, links)
--secondary: #2c3e50 (Headings, dark backgrounds)
--accent: #e74c3c (Highlights, warnings)
--success: #27ae60 (Success states)
--warning: #f39c12 (Warning states)
```

### Typography Scale
```css
h1: clamp(1.8rem, 5vw, 3rem)
h2: clamp(1.4rem, 4vw, 2.5rem)
h3: clamp(1.1rem, 3vw, 1.5rem)
body: 16px base with 1.6 line-height
```

### Spacing System (8px base unit)
```css
--spacing-xs: 0.5rem (4px)
--spacing-sm: 1rem (8px)
--spacing-md: 1.5rem (12px)
--spacing-lg: 2rem (16px)
--spacing-xl: 3rem (24px)
--spacing-xxl: 4rem (32px)
```

### Shadows & Effects
```css
--shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.1)
--shadow: 0 2px 8px rgba(0, 0, 0, 0.1)
--shadow-lg: 0 4px 16px rgba(0, 0, 0, 0.15)
--shadow-xl: 0 10px 40px rgba(0, 0, 0, 0.2)
```

---

## 📱 Device Testing

### Tested On:
- ✅ iPhone 12/13/14 (375px - 390px)
- ✅ iPad (768px)
- ✅ iPad Pro (1024px)
- ✅ Desktop (1920px, 2560px)
- ✅ Chrome DevTools responsive mode

### Browser Compatibility:
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

---

## 🚀 Performance Metrics

### Core Web Vitals Optimization:
- ✅ **LCP (Largest Contentful Paint):** < 2.5s
- ✅ **FID (First Input Delay):** < 100ms
- ✅ **CLS (Cumulative Layout Shift):** < 0.1

### Optimization Techniques:
1. **CSS Optimization:**
   - Minimal CSS bundle size
   - Efficient selectors
   - CSS variables reduce duplication
   - Media queries avoid loading unnecessary CSS

2. **Image Optimization:**
   - Responsive images with srcset
   - Multiple formats (WebP, PNG, JPG)
   - Proper sizing and aspect ratios

3. **HTML Optimization:**
   - Semantic markup reduces parsing overhead
   - Minimal DOM nodes
   - Proper viewport meta tag
   - Preconnect to external resources

---

## 🎓 Learning Outcomes

This assignment covers and demonstrates:

### Advanced HTML5
1. ✅ Semantic HTML structure
2. ✅ Accessible forms with validation
3. ✅ Structured data (Schema.org)
4. ✅ Responsive images (picture, srcset)
5. ✅ Video/audio embedding
6. ✅ ARIA attributes

### Advanced CSS3
1. ✅ CSS Grid layout system
2. ✅ Flexbox layout
3. ✅ CSS custom properties
4. ✅ CSS animations & transitions
5. ✅ Media queries & responsive design
6. ✅ CSS containment
7. ✅ Stacking context
8. ✅ CSS specificity
9. ✅ Box model mastery
10. ✅ Logical properties

### Best Practices
1. ✅ Mobile-first approach
2. ✅ Component-based design
3. ✅ DRY (Don't Repeat Yourself) principles
4. ✅ WCAG 2.1 accessibility compliance
5. ✅ Performance optimization
6. ✅ Code maintainability
7. ✅ Semantic versioning

---

## 📝 Practical Tasks Descriptions

### 1. **Semantic Blog Page**
- Demonstrates proper use of HTML5 semantic elements
- Includes article schema markup
- Proper navigation and footer structure
- Blog article layout

### 2. **Accessible Navigation**
- ARIA roles for menu items
- Submenu with proper attributes
- Search form integration
- Breadcrumb navigation
- Mobile-friendly hamburger menu

### 3. **Complex Form**
- Multiple fieldsets with legends
- Input types and validation
- Datalist for autocomplete
- Pattern validation with hints
- Accessibility labels
- Error messaging with aria-live

### 4. **FAQ Section**
- HTML5 `<details>` and `<summary>` elements
- CSS styling and animations
- Expand/collapse all functionality
- Keyboard navigation support

### 5. **Responsive Images**
- Srcset with width descriptors
- Picture element with media queries
- Art direction examples
- Format selection (WebP fallback)
- Background image responsive approach

### 6. **Accessible Video**
- HTML5 video element
- Multiple track types (captions, subtitles, descriptions)
- Embedded video with accessibility
- Audio player with transcript
- Keyboard controls documentation

---

## 🏆 Final Master Project Features

The "TechFlow" landing page demonstrates:

### Structure
- ✅ Complete responsive website layout
- ✅ Sticky header with mobile menu
- ✅ Multiple content sections
- ✅ Footer with sitemap

### Layouts
- ✅ Hero section with gradient
- ✅ Services grid (responsive)
- ✅ Portfolio masonry layout
- ✅ Testimonials carousel (CSS-only)
- ✅ Pricing table with featured card
- ✅ Contact form with validation

### Features
- ✅ Dark mode toggle
- ✅ Smooth scrolling
- ✅ Hover animations
- ✅ Form validation
- ✅ Responsive navigation

### Design System
- ✅ CSS variables for theming
- ✅ Consistent spacing
- ✅ Color palette
- ✅ Typography scale
- ✅ Component library approach

---

## 🔧 How to Use

1. **Open in Browser:**
   ```bash
   # Open any HTML file directly in your browser
   # Or use a local server:
   python -m http.server 8000
   # Then visit http://localhost:8000
   ```

2. **Test Responsive Design:**
   - Use Chrome DevTools (F12)
   - Toggle device toolbar (Ctrl + Shift + M)
   - Test different viewport sizes

3. **Test Accessibility:**
   - Use WAVE browser extension
   - Test with screen reader (NVDA for Windows, VoiceOver for Mac)
   - Check keyboard navigation (Tab, Enter, Arrow keys)

4. **Dark Mode Testing:**
   - On macOS: System Preferences > General > Appearance
   - On Windows: Settings > Personalization > Colors
   - Or use browser's emulation in DevTools

---

## 📊 CSS Specifications Used

### Layout Systems
- ✅ CSS Grid (2D layouts)
- ✅ Flexbox (1D layouts)
- ✅ Logical properties (writing modes)

### Responsive Techniques
- ✅ Media queries (mobile-first)
- ✅ Fluid typography (clamp())
- ✅ Responsive images (srcset, picture)
- ✅ Container queries (future-proof)

### Modern CSS
- ✅ Custom properties (variables)
- ✅ CSS containment
- ✅ Backdrop filters
- ✅ Gradients (linear & radial)
- ✅ Transitions & animations
- ✅ Transform effects

### Accessibility CSS
- ✅ High contrast mode support
- ✅ Reduced motion respect
- ✅ Focus indicators
- ✅ Color contrast optimization
- ✅ Readable font sizes

---

## 🎯 Design Decisions

### Mobile-First Approach
- Ensures optimal mobile experience
- Progressive enhancement
- Reduces CSS bloat
- Better performance

### CSS Variables
- Theme switching without JavaScript
- Maintainability
- Consistency across components
- Easy dark mode implementation

### Semantic HTML
- Better accessibility
- Improved SEO
- Cleaner markup
- Easier maintenance

### No JavaScript for Core Functionality
- Follows assignment requirements
- Ensures functionality for all users
- Better performance
- Progressive enhancement

---

## 📚 References & Resources

### Accessibility
- [W3C WCAG 2.1](https://www.w3.org/WAI/WCAG21/quickref/)
- [MDN: ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA)
- [WebAIM](https://webaim.org/)

### CSS
- [MDN: CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS-Tricks](https://css-tricks.com/)
- [Web.dev CSS Guide](https://web.dev/learn/css/)

### HTML
- [MDN: HTML Reference](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [Schema.org](https://schema.org/)

### Responsive Design
- [Mobile-First Approach](https://www.nngroup.com/articles/mobile-first-web-design/)
- [Fluid Responsive Design](https://www.smashingmagazine.com/2022/01/modern-fluid-typography-using-css-clamp/)

---

## ✅ Submission Checklist

- ✅ All HTML files are valid and semantic
- ✅ All CSS is mobile-first and responsive
- ✅ WCAG 2.1 Level AA accessibility compliance
- ✅ Tested on multiple devices and browsers
- ✅ No JavaScript used (except theme toggle)
- ✅ Code is properly commented
- ✅ Performance optimized
- ✅ Dark mode support implemented
- ✅ Responsive images implemented
- ✅ All forms are accessible
- ✅ Final master project complete

---

## Author

**Sejal Singh**    


---


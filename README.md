# SRS Wealth - Premium Landing Page

A modern, professional landing page for SRS Wealth Management with a premium, trust-led design.

## 🎯 Features

### Design & User Experience
- **Premium Design**: Clean, sophisticated layout with gold accents and navy color scheme
- **Trust-Led Messaging**: Emphasizes credibility, data-driven approach, and long-term thinking
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Smooth Animations**: Fade-in effects, parallax scrolling, and interactive hover states
- **Professional Typography**: Playfair Display for headlines, Inter for body text

### Sections Included
1. **Hero Section**: Powerful headline with trust indicators (AUM, clients served, years of experience)
2. **Philosophy Section**: Core values and approach with visual cards
3. **Services Section**: Three main service offerings (Wealth Creation, Preservation, Legacy Planning)
4. **Approach Section**: 4-step process explanation
5. **Contact Form**: Lead capture with consultation scheduling
6. **Footer**: Complete navigation and legal links

### Interactive Elements
- Sticky navigation with scroll effects
- Mobile-responsive hamburger menu
- Animated number counters for trust indicators
- Smooth scroll to sections
- Form validation and submission handling
- Parallax background effects
- Hover animations on cards and buttons

## 📁 File Structure

```
srs-wealth-landing/
├── index.html          # Main HTML structure
├── styles.css          # Complete styling with responsive design
├── script.js           # Interactive JavaScript functionality
└── README.md          # This file
```

## 🚀 How to Use

### Option 1: Open Directly
Simply open `index.html` in any modern web browser.

### Option 2: Local Server (Recommended)
For best results, serve the files through a local server:

```bash
# Using Python 3
cd srs-wealth-landing
python3 -m http.server 8000

# Using Node.js (with http-server)
npx http-server srs-wealth-landing -p 8000

# Using PHP
php -S localhost:8000
```

Then visit: `http://localhost:8000`

## 🎨 Customization Guide

### Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-dark: #0a1628;      /* Main dark navy */
    --accent-gold: #d4af37;       /* Gold accent */
    --text-primary: #0a1628;      /* Body text */
    /* ... more colors */
}
```

### Content
All content can be edited directly in `index.html`:
- Headlines and subheadings
- Service descriptions
- Trust indicators (numbers)
- Contact form fields
- Footer information

### Fonts
Current fonts (loaded from Google Fonts):
- **Display**: Playfair Display (headlines)
- **Body**: Inter (paragraphs, UI)

To change fonts, update the Google Fonts link in `index.html` and CSS variables.

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px

## 🔧 Form Integration

The contact form currently uses a simulated submission. To integrate with your backend:

1. Open `script.js`
2. Find the form submission section (line ~100)
3. Replace the `setTimeout` simulation with your API call:

```javascript
const response = await fetch('/api/contact', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify({
        name: formData.get('name'),
        email: formData.get('email'),
        // ... other fields
    })
});
```

## 🎯 Performance Optimizations

- Minimal external dependencies (only Google Fonts)
- Optimized CSS with efficient selectors
- Lazy loading support for images (when added)
- Smooth animations using CSS transforms
- Intersection Observer for scroll animations

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📊 Key Metrics to Track

Once deployed, track these metrics:
- Form submission rate
- Time on page
- Scroll depth
- Click-through rate on CTA buttons
- Mobile vs. desktop traffic

## 🔒 Security Considerations

Before deploying to production:
1. Add HTTPS/SSL certificate
2. Implement CSRF protection on form
3. Add rate limiting to prevent spam
4. Sanitize all form inputs on backend
5. Add reCAPTCHA or similar bot protection

## 📝 SEO Recommendations

To improve search engine visibility:
1. Add meta description tag
2. Include Open Graph tags for social sharing
3. Add structured data (JSON-LD) for organization
4. Optimize images with alt text (when added)
5. Create sitemap.xml
6. Add robots.txt

## 🎨 Design Philosophy

This landing page follows these principles:
- **Trust First**: Professional, credible design that builds confidence
- **Clarity**: Clear messaging without jargon
- **Sophistication**: Premium feel appropriate for wealth management
- **Conversion-Focused**: Strategic CTAs and form placement
- **Mobile-First**: Responsive design that works everywhere

## 📞 Support

For questions or customization requests, contact the development team.

---

**Built with ❤️ for SRS Wealth Management**
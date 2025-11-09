# DDS Product Section - Shopify 2.0 Modern (2025)

A fully modern, accessible, and performance-optimized product section for Shopify themes, specifically designed for sustainable streetwear and organic apparel brands.

## Version

**5.0.0** - Built for 2025 with Shopify 2.0 best practices

## Compatibility

- **Shopify Plan**: Basic and above
- **Theme**: Atelier 2.1.1 and modern Shopify 2.0 themes
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)

## Features

### 🚀 Performance Optimizations

- **Mobile-first CSS** with optimized media queries
- **Native lazy loading** for images
- **Minimal JavaScript** - vanilla JS, no framework dependencies
- **CSS-in-Liquid** with scoped variables
- **Optimized image srcsets** for responsive loading
- **Reduced motion support** for better accessibility
- **Fast page speed scores** - optimized for Core Web Vitals

### ♿ Accessibility (WCAG 2.1 AA Compliant)

- **Full keyboard navigation** support
- **Screen reader optimized** with proper ARIA attributes
- **Focus-visible indicators** for all interactive elements
- **Semantic HTML5** structure
- **Skip to content** links
- **Proper heading hierarchy**
- **ARIA labels and live regions**
- **High contrast support**
- **Reduced motion preferences** respected

### 🎨 Design Features

- **FREE Shipping emphasis** for organic/recycled products
- **Certification badges** (GOTS, GRS, OCS, OEKO-TEX, PETA)
- **Sustainability information** prominently displayed
- **Product image gallery** with thumbnails
- **Size guide modal** with dynamic content
- **Variant selectors** (sizes, colors, custom options)
- **Mobile sticky bar** for easy cart addition
- **Animated free shipping banner**
- **Accordion product details**
- **Trust signals** and features

### 📱 Mobile Responsive

- **Mobile-first approach**
- **Touch-friendly buttons** and controls
- **Sticky add-to-cart bar** on mobile
- **Optimized spacing** for small screens
- **Swipeable image gallery**

### 🛍️ E-commerce Features

- **Real-time variant switching**
- **Price updates** with compare-at-price
- **Sale badge** with percentage off
- **Quantity selector**
- **Add to cart** with loading states
- **Dynamic checkout buttons** (Apple Pay, Google Pay, etc.)
- **Out of stock** handling
- **URL parameter** variant selection

## Installation

1. Copy `sections/dds-product-section.liquid` to your theme's `sections/` directory

2. In the Shopify theme customizer:
   - Navigate to your product template
   - Add the "DDS Product Section" section
   - Configure colors and settings

3. For FREE shipping to work, tag your products with:
   - `organic` or `GOTS` for organic products
   - `recycled` or `GRS` for recycled products
   - `sustainable` for general sustainable products

## Configuration

### Theme Customizer Settings

- **Product** - Select product for preview
- **Show dynamic checkout buttons** - Enable/disable Apple Pay, etc.
- **Primary color** - Main brand color
- **Accent color** - Secondary brand color
- **Eco/sustainability color** - Free shipping and eco badges
- **Text color** - Main text color

### Product Tagging

Tag your products to enable specific features:

#### Certifications
- `GOTS` - Global Organic Textile Standard
- `GRS` - Global Recycled Standard
- `OCS` - Organic Content Standard
- `OEKO-TEX` - OEKO-TEX Standard 100
- `vegan` - PETA-Approved Vegan

#### Free Shipping
- `organic` - Organic materials
- `recycled` - Recycled materials
- `sustainable` - General sustainability

### Size Guide

Add size guide in two ways:

1. **Metafield** (recommended):
   - Add custom metafield: `custom.size_guide`
   - Add your size guide HTML/table

2. **Product description**:
   - Add "SIZE GUIDE" heading in description
   - Follow with HTML table
   - Section will extract and display in modal

## Browser Support

- Chrome/Edge (last 2 versions)
- Firefox (last 2 versions)
- Safari (last 2 versions)
- Mobile browsers (iOS Safari, Chrome Android)

## Performance

### Optimizations Applied

- **CSS**: Scoped variables, mobile-first, no unused styles
- **JavaScript**: Vanilla JS, event delegation, no external libraries
- **Images**: Responsive srcsets, lazy loading, aspect ratios
- **HTML**: Semantic, minimal DOM, progressive enhancement
- **Loading**: Critical CSS inline, deferred scripts

### Expected Scores

- **Lighthouse Performance**: 90+
- **Accessibility**: 100
- **Best Practices**: 95+
- **SEO**: 100

## Accessibility Features

### Keyboard Navigation

- **Tab**: Navigate through interactive elements
- **Enter/Space**: Activate buttons, open modals
- **Escape**: Close modals
- **Arrow keys**: Navigate through options

### Screen Readers

- All images have descriptive alt text
- ARIA labels on all controls
- Live regions for dynamic updates
- Skip to content links
- Proper heading structure
- Form labels and descriptions

### Visual Accessibility

- High contrast colors
- Focus indicators on all interactive elements
- Reduced motion support
- Scalable text (no fixed font sizes)
- Touch target sizes (44x44px minimum)

## Customization

### CSS Variables

All styles use CSS custom properties for easy customization:

```css
--dds-primary: Primary brand color
--dds-accent: Accent color
--dds-eco: Sustainability color
--dds-text: Text color
--dds-bg: Background color
--dds-surface: Surface color
--dds-border: Border color
--dds-radius: Border radius
--dds-shadow-sm/md/lg: Box shadows
--dds-transition: Transition timing
--dds-spacing: Responsive spacing
```

### JavaScript API

Access the section's JavaScript functionality:

```javascript
// Get section instance
const productSection = window.DDSProduct['section-id'];

// Update variant programmatically
productSection.updateVariant(variantObject);

// Listen for cart additions
document.addEventListener('cart:item-added', (e) => {
  console.log('Added to cart:', e.detail);
});
```

## Translations

The section is fully translatable. Add translations to your theme's locale files:

```json
{
  "products": {
    "product": {
      "free_shipping": "FREE SHIPPING",
      "add_to_cart": "Add to Cart",
      "sold_out": "Sold Out",
      "size_guide": "Size Guide",
      // ... more translations
    }
  }
}
```

## Troubleshooting

### Free shipping banner not showing

- Ensure product is tagged with: `organic`, `GOTS`, `recycled`, `GRS`, or `sustainable`

### Size guide not appearing

- Add size guide to product description with "SIZE GUIDE" heading
- OR add to `custom.size_guide` metafield

### Variant images not updating

- Ensure variants have featured images assigned in Shopify admin

### Dynamic checkout buttons not showing

- Enable in section settings
- Ensure payment providers are configured in Shopify settings

## Support

For issues or questions:
1. Check product tags are correct
2. Verify section settings in theme customizer
3. Check browser console for JavaScript errors
4. Test in different browsers

## License

Proprietary - Design Delight Studio

## Changelog

### v5.0.0 (2025)
- Complete rewrite for Shopify 2.0
- Full accessibility compliance (WCAG 2.1 AA)
- Performance optimizations
- Mobile-first responsive design
- Modern JavaScript (ES6+)
- Enhanced free shipping emphasis
- Better keyboard navigation
- Screen reader optimizations

---

Built with ❤️ for sustainable fashion brands

# VeChain Calculator Landing Page - Maintenance Guide

This guide will help you maintain and customize the VeChain Calculator landing page. Whether you're new to web development or need a quick reference, follow these instructions to make updates safely and effectively.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the main navigation and logo. To update:

1. Change the logo text:
```html
<!-- Located in the header section -->
<a href="#" class="text-xl font-bold text-blue-400">VeChain Calculator</a>
```

2. Modify navigation items:
```html
<a href="#features" class="text-gray-300 hover:text-white transition duration-300">Features</a>
```

### Hero Section
The main headline and call-to-action are in the hero section:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6 bg-gradient-to-r from-blue-400 to-blue-600 bg-clip-text text-transparent">VeChain Calculator</h1>
```

**Tailwind CSS Tips:**
- `text-4xl`: Base font size
- `md:text-5xl`: Tablet font size
- `lg:text-6xl`: Desktop font size
- `mb-6`: Bottom margin spacing
- `from-blue-400 to-blue-600`: Gradient colors

### Features Section
Each feature card follows this structure:
```html
<div class="bg-gray-800 rounded-xl p-8 shadow-lg hover:shadow-2xl transition duration-300 transform hover:scale-105">
    <!-- Icon -->
    <h3 class="text-xl font-semibold mb-4">Feature Title</h3>
    <p class="text-gray-400">Feature description</p>
</div>
```

**Styling Tips:**
- Keep hover effects by maintaining the `hover:` classes
- Maintain responsive padding (`p-8`)
- Preserve animation classes (`transition`, `transform`)

## Managing Links

### Navigation Links
Current internal links:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
```

To update:
1. For internal sections, use `#section-id`
2. For external links, use full URLs
3. Example:
```html
<a href="https://your-external-link.com" class="text-gray-300 hover:text-white transition duration-300">Link Text</a>
```

### Call-to-Action Buttons
Current CTA link:
```html
<a href="https://bitvavo.com/invite?a=9A12094098" class="bg-blue-500 hover:bg-blue-600 text-white px-6 py-2 rounded-lg transition duration-300 transform hover:scale-105">Start Now</a>
```

To update:
1. Replace the `href` attribute with your new URL
2. Maintain the class structure for consistent styling

## Adding Privacy and Terms Pages

### Footer Link Updates
Locate the legal section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the links:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Styles**
   - Verify Tailwind CSS CDN link is working
   - Check for typos in class names
   - Ensure responsive classes (`md:`, `lg:`) are properly ordered

2. **Navigation Links Not Working**
   - Confirm section IDs match href attributes
   - Check for proper scroll-smooth class on html element
   - Verify external URLs are complete and correct

3. **Responsive Design Issues**
   - Test on multiple screen sizes
   - Maintain mobile-first approach
   - Keep responsive classes (`md:`, `lg:`) intact

### Best Practices

1. Always test changes in multiple browsers
2. Maintain the existing class structure for consistency
3. Back up files before making significant changes
4. Keep the responsive design classes intact
5. Test all links after updates

Need further assistance? Contact: vet@jesso.nl

---

This guide covers the basics of maintaining your VeChain Calculator landing page. For more complex modifications, consider consulting with a web developer.
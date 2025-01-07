# Ultimate Website Builder - Landing Page Maintenance Guide

This guide will help you maintain and customize the Ultimate Website Builder landing page. Whether you're new to web development or just getting started, follow these instructions to make updates while preserving the design integrity.

## Table of Contents
- [Text and Styling Updates](#text-and-styling-updates)
- [Link Management](#link-management)
- [Privacy and Terms Pages](#privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Text and Styling Updates

### Header Section
The header contains the logo and navigation menu. To modify:

1. **Logo Text**
```html
<!-- Find this section in the header -->
<div class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent">
    UWB  <!-- Change this text to your brand name -->
</div>
```

2. **Navigation Menu Items**
```html
<div class="hidden md:flex space-x-8">
    <!-- Modify these link texts as needed -->
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6 leading-tight">
    Ultimate AI Agent Built Websites  <!-- Update main headline here -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Create stunning websites instantly  <!-- Update subheading here -->
</p>
```

### Styling Tips
- Font sizes use Tailwind's scale: `text-sm`, `text-base`, `text-lg`, `text-xl`, etc.
- Colors follow the pattern: `text-{color}-{shade}` (e.g., `text-purple-600`)
- Spacing uses `m-` for margin and `p-` for padding followed by a number (e.g., `m-4`, `p-6`)

## Link Management

### Navigation Links
1. Internal section links (current setup):
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

2. Call-to-action button link:
```html
<!-- Update this URL -->
<a href="https://uwb.com" class="inline-block px-8 py-4 bg-gradient-to-r from-purple-600 to-blue-500">
    Start Building Now
</a>
```

### Footer Links
Replace placeholder links in the footer:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Links</h4>
    <ul class="space-y-2">
        <!-- Update these href attributes -->
        <li><a href="/about">About</a></li>
        <li><a href="/features">Features</a></li>
        <li><a href="/pricing">Pricing</a></li>
    </ul>
</div>
```

## Privacy and Terms Pages

### Adding Policy Links
1. Locate the legal section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <!-- Update these href attributes -->
        <li><a href="/privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="/terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

2. Create matching policy pages:
- Create `privacy.html` and `terms.html` in the same directory as `index.html`
- Use the same styling classes for consistency
- Link back to the main page using relative paths: `<a href="index.html">Home</a>`

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
- Check that all `href` attributes start with `/` for root-relative paths
- Use `./` for same-directory files
- Verify file names match exactly (case-sensitive)

2. **Styling Problems**
- Make sure Tailwind CSS CDN is properly loaded
- Check for typos in class names
- Maintain responsive classes (e.g., `md:`, `lg:` prefixes)

3. **Layout Issues**
- Preserve container classes: `container mx-auto px-6`
- Keep responsive grid classes: `grid-cols-1 md:grid-cols-3`
- Maintain spacing classes for consistency

### Best Practices
- Always test changes on multiple screen sizes
- Keep the gradient styling consistent (`from-purple-600 to-blue-500`)
- Maintain accessibility by keeping sufficient color contrast
- Preserve hover effects and transitions for interactive elements

Need more help? Contact support at admin@uwb.com or refer to the Tailwind CSS documentation for detailed styling information.
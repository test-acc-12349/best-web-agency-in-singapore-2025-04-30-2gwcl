# Landing Page Maintenance Guide

This guide will help you maintain and customize the Web Agency landing page. Follow these detailed instructions to make common updates while preserving the design and functionality.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Logo Text -->
<div class="text-xl font-bold text-white">
    <a href="/" class="flex items-center space-x-2">
        <span class="text-blue-500">Web</span>
        <span>Agency</span>
    </a>
</div>
```
To change the logo text, modify the content between the `<span>` tags.

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight tracking-tight mb-8">
    Best Web Agency In Singapore
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">
    Grow your business with clicks - Professional web development solutions that drive results
</p>
```
Update the main headline and subheading by changing the text within these elements.

### Understanding Tailwind Classes

Key class patterns used in this landing page:

- Responsive classes: `text-4xl md:text-5xl lg:text-6xl`
  - `text-4xl`: Base size for mobile
  - `md:text-5xl`: Medium screens (768px+)
  - `lg:text-6xl`: Large screens (1024px+)

- Spacing classes:
  - `px-6`: Horizontal padding
  - `py-24`: Vertical padding
  - `mb-8`: Bottom margin
  - `space-x-4`: Horizontal spacing between elements

- Color classes:
  - `bg-gray-900`: Dark background
  - `text-gray-300`: Light gray text
  - `text-blue-500`: Blue accent color

## 2. Fixing Broken Links

### Navigation Menu Links
Current internal links in the navigation:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update these:
1. Identify the section ID you want to link to
2. Update the `href` attribute with the section ID prefixed with `#`
3. Example: To link to a new section called "Services":
   ```html
   <a href="#services" class="text-gray-300 hover:text-white transition-colors duration-300">Services</a>
   ```

### Call-to-Action Links
Current CTA links:
```html
<a href="https://fixrr.online" class="inline-block bg-blue-600 hover:bg-blue-700 text-white font-semibold px-8 py-4 rounded-lg">
    Get Started Today
</a>
```

To update:
1. Replace `https://fixrr.online` with your desired URL
2. Update button text between the `<a>` tags
3. Maintain the existing classes for consistent styling

## 3. Linking Privacy and Terms Pages

### Footer Legal Links
Current placeholder links:
```html
<div>
    <h3 class="text-white text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting Tips

1. **Broken Internal Links**
   - Ensure section IDs match exactly (case-sensitive)
   - Check for extra spaces in IDs
   - Verify the `#` prefix is present

2. **Responsive Design Issues**
   - Test at different screen sizes using browser dev tools
   - Maintain the responsive class pattern (base/md/lg)
   - Don't remove container classes that center content

3. **Style Consistency**
   - Copy existing classes when adding new elements
   - Keep color schemes consistent (blue-500, gray-900, etc.)
   - Maintain padding/margin patterns from similar elements

## Best Practices

1. Always backup the file before making changes
2. Test all links after updating
3. View changes across different devices and browsers
4. Maintain the existing class structure for consistency
5. Keep the responsive design intact by preserving media query classes

Need help? Contact your web developer or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs) for detailed class references.
# Bryan Engel Photography Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Bryan Engel Photography landing page. It's designed for beginners with no prior coding experience.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<!-- Original header text -->
<div class="text-2xl font-bold text-gray-800">Bryan Engel</div>
```
To update the business name, simply replace "Bryan Engel" with your desired text while keeping the surrounding div tags intact.

#### Hero Section
Look for this section and modify the text between the tags:
```html
<h1 class="text-4xl md:text-6xl font-bold text-white mb-6">Bryan Engel Photography</h1>
<p class="text-xl md:text-2xl text-gray-200 mb-8">Taking your photography to the next level</p>
```

#### Announcement Bar
To update the announcement message:
```html
<div class="bg-gray-900 text-white py-2 px-4 text-center text-sm">
    <!-- Replace this text -->
    <p>Fast Worldwide Shipping (5 days delivery) | 100% Satisfaction Guarantee</p>
</div>
```

### Tailwind CSS Classes Explained

#### Common Tailwind Classes Used:
- `container mx-auto`: Centers content with automatic margins
- `px-6`: Adds horizontal padding (left and right)
- `py-4`: Adds vertical padding (top and bottom)
- `text-[size]`: Sets text size (xl, 2xl, 3xl, etc.)
- `bg-[color]`: Sets background color
- `text-[color]`: Sets text color

#### Responsive Design Classes:
```html
<!-- Example of responsive classes -->
<h1 class="text-4xl md:text-6xl">
```
- `text-4xl`: Default size on mobile
- `md:text-6xl`: Larger size on medium screens and up

## Fixing Broken Links

### Navigation Menu Links
Current placeholder links in the header:
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Home</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Services</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Portfolio</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Contact</a>
</div>
```

To update these links:
1. Replace `#` with your actual page URLs
2. Example: `<a href="services.html">Services</a>`
3. For external links, use complete URLs: `<a href="https://example.com">Example</a>`

### Footer Links
Update the Quick Links section in the footer:
```html
<ul class="space-y-2">
    <li><a href="index.html" class="hover:text-white transition-colors duration-300">Home</a></li>
    <li><a href="services.html" class="hover:text-white transition-colors duration-300">Services</a></li>
    <!-- Continue for other links -->
</ul>
```

## Linking Privacy and Terms Pages

### Adding Policy Pages
Locate the Policies section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Policies</h4>
    <ul class="space-y-2">
        <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
        <!-- Other policy links -->
    </ul>
</div>
```

To implement:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the href attributes with correct file paths
3. Maintain consistent styling by copying the existing classes

## Troubleshooting

### Common Issues and Solutions

1. **Broken Images**
   - Check if image URLs are correct
   - Ensure images exist at specified paths
   - Example fix:
   ```html
   <!-- Replace with your image path -->
   <img src="images/your-image.jpg" alt="Description">
   ```

2. **Responsive Design Issues**
   - Verify Tailwind classes are properly nested
   - Check mobile-first design principles
   - Example of proper responsive class usage:
   ```html
   <div class="text-sm md:text-base lg:text-lg">
   ```

3. **Link Issues**
   - Verify file paths are relative to your HTML file
   - Check for typos in URLs
   - Ensure files exist in specified locations

### Need Help?
- Double-check all file paths
- Verify HTML syntax and closing tags
- Test on multiple devices and browsers
- Use browser developer tools (F12) to inspect elements

Remember to always backup your files before making changes, and test all modifications in a development environment first.
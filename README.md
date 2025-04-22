# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. Follow these instructions carefully to make updates while preserving the design and functionality.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. **Logo Text**
```html
<div class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
    Logo <!-- Replace "Logo" with your company name -->
</div>
```

2. **Navigation Links**
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <!-- Update text between <a> tags for each navigation item -->
</div>
```

### Hero Section
Located at the top of the page with the main heading:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent mb-8">
    Lorem ipsum dolor <!-- Replace with your main heading -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Lorem ipsum dolor sit amet <!-- Replace with your subheading -->
</p>
```

### Features Section
To update feature cards:

1. Find the feature card template:
```html
<div class="p-8 rounded-2xl bg-white shadow-lg hover:shadow-xl transition duration-300 border border-gray-100">
    <div class="w-12 h-12 bg-purple-100 rounded-lg mb-6 flex items-center justify-center">
        <!-- Icon SVG here -->
    </div>
    <h3 class="text-xl font-semibold mb-4">Feature 1</h3> <!-- Update feature title -->
    <p class="text-gray-600">Lorem ipsum dolor sit amet</p> <!-- Update feature description -->
</div>
```

2. To add more features, copy the entire `<div>` block and paste it within the grid container.

### Understanding Tailwind Classes
Common classes used in this template:

- `container mx-auto`: Centers content with automatic margins
- `px-6`: Adds horizontal padding (6 units)
- `py-4`: Adds vertical padding (4 units)
- `text-gray-600`: Sets text color
- `hover:text-gray-900`: Changes text color on hover
- `md:text-2xl`: Applies font size on medium screens and up

## Managing Links

### Navigation Menu Links
Update the `href` attributes in the header:

```html
<div class="hidden md:flex space-x-8">
    <a href="features.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <a href="benefits.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Benefits</a>
    <a href="contact.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Contact</a>
</div>
```

### Call-to-Action Buttons
Update the "Get Started" button links:

```html
<a href="signup.html" class="inline-block bg-gradient-to-r from-purple-600 to-pink-600 text-white text-lg px-8 py-4 rounded-full hover:shadow-xl transform hover:scale-105 transition duration-300">
    Get Started Now
</a>
```

### Footer Links
Update company, resources, and legal links:

```html
<ul class="space-y-2">
    <li><a href="about.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">About</a></li>
    <li><a href="careers.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Careers</a></li>
    <!-- Continue for each footer link -->
</ul>
```

## Adding Privacy and Terms Pages

### 1. Update Footer Legal Links
Locate the legal section in the footer:

```html
<div>
    <h4 class="font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="privacy.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Privacy</a></li>
        <li><a href="terms.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Terms</a></li>
    </ul>
</div>
```

### 2. Create Policy Pages
1. Create new files named `privacy.html` and `terms.html`
2. Copy the header and footer from `index.html`
3. Add your policy content between them

## Troubleshooting

### Common Issues

1. **Broken Links**
   - Check that all HTML files exist in your directory
   - Verify file names match exactly (case-sensitive)
   - Use relative paths (e.g., `./privacy.html` or just `privacy.html`)

2. **Styling Problems**
   - Ensure Tailwind CSS is properly loaded
   - Check for typos in class names
   - Maintain responsive classes (e.g., `md:`, `lg:` prefixes)

3. **Layout Issues**
   - Keep the container structure intact
   - Maintain grid column settings
   - Preserve responsive design classes

### Need Help?
- Double-check all closing tags
- Validate HTML at [W3C Validator](https://validator.w3.org/)
- Inspect element using browser developer tools
- Ensure all required files are in the correct directory

Remember to test all changes across different screen sizes using your browser's developer tools.
# Landing Page Maintenance Guide

This guide will help you maintain and customize the Airco Naaldwijk landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common maintenance tasks.

## 1. Updating Text and Tailwind CSS Classes

### Header Section
```html
<header class="fixed w-full bg-white/95 backdrop-blur-sm shadow-md z-50">
    <div class="text-2xl font-bold text-blue-600">Airco Naaldwijk</div>
</header>
```
To update the company name:
1. Locate the `<div>` with class `text-2xl`
2. Replace "Airco Naaldwijk" with your desired text
3. Adjust text size using Tailwind classes:
   - `text-xl` (smaller)
   - `text-2xl` (current size)
   - `text-3xl` (larger)

### Hero Section
```html
<section class="pt-32 pb-20 bg-gradient-to-br from-blue-50 to-gray-100">
    <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold">
        🌟 Laatste Kans! De Beste Airco's Voor Deze Zomer 
    </h1>
</section>
```
To modify the hero section:
1. Find the `<h1>` tag within the first `<section>`
2. Update the emoji and text as needed
3. Responsive text sizes are controlled by:
   - `text-4xl` (mobile)
   - `md:text-5xl` (tablet)
   - `lg:text-6xl` (desktop)

### Features Section
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
    <div class="bg-white rounded-xl shadow-lg p-8">
        <h3 class="text-xl font-bold mb-4">⚡ Snelste Levering</h3>
        <p class="text-gray-600">Morgen al genieten van verkoeling!</p>
    </div>
</div>
```
To update feature cards:
1. Locate the feature cards within the grid
2. Modify emoji, heading, and description text
3. Key styling classes:
   - `rounded-xl` (corner rounding)
   - `shadow-lg` (box shadow)
   - `p-8` (padding)

## 2. Fixing Broken Links

### Navigation Menu
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-blue-600">Producten</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600">Voordelen</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600">Contact</a>
</div>
```
To update navigation links:
1. Find the `<a>` tags within the navigation
2. Update `href` attributes:
   - Internal sections use `#section-name`
   - External pages use full URLs
3. Update link text between `<a>` tags

### Call-to-Action Buttons
```html
<a href="https://amzn.to/3S5kfNj" class="inline-block bg-blue-600 hover:bg-blue-700">
    Direct Bestellen - 15% Korting
</a>
```
To update CTA buttons:
1. Locate `<a>` tags with `inline-block` class
2. Replace the Amazon affiliate link
3. Update button text
4. Maintain hover effects with `hover:` classes

## 3. Linking Privacy and Terms Pages

### Footer Links
```html
<div>
    <h3 class="text-xl font-bold mb-4">Links</h3>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-blue-400">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-blue-400">Algemene Voorwaarden</a></li>
    </ul>
</div>
```
To add policy pages:
1. Create new files:
   - `privacy.html`
   - `terms.html`
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-blue-400">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-blue-400">Algemene Voorwaarden</a></li>
```

## Troubleshooting Tips

1. **Broken Internal Links**
   - Ensure section IDs match href attributes
   - Example: `href="#features"` links to `id="features"`

2. **Responsive Issues**
   - Check mobile view using browser dev tools
   - Verify breakpoint classes:
     - `md:` (768px and up)
     - `lg:` (1024px and up)

3. **Style Inconsistencies**
   - Keep color classes consistent:
     - Primary: `blue-600`
     - Text: `gray-600`
     - Background: `gray-50`
   - Maintain spacing patterns:
     - Sections: `py-24`
     - Components: `p-8`

## Additional Notes

- All emojis can be updated by replacing the emoji character
- Social media links in footer need real URLs
- Contact email should be updated to your actual email
- Copyright year in footer should be kept current

Remember to test all changes across different screen sizes and browsers before publishing updates.
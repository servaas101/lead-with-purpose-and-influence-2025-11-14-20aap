# Leadership Academy Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain and customize the Leadership Academy landing page. Whether you're updating text, fixing links, or adding new content, this document provides step-by-step instructions tailored to your specific HTML structure.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
4. [Fixing and Managing Links](#fixing-and-managing-links)
5. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
6. [Common Customization Tasks](#common-customization-tasks)
7. [Troubleshooting](#troubleshooting)

---

## Getting Started

### What You'll Need

- **Text Editor**: Any text editor will work (Notepad, VS Code, Sublime Text, etc.)
- **Web Browser**: To preview your changes (Chrome, Firefox, Safari, Edge)
- **Basic Understanding**: This guide assumes no prior coding experience

### File Structure

Your landing page consists of:
- `index.html` - The main landing page file you'll be editing
- `privacy.html` - Privacy policy page (you'll create this)
- `terms.html` - Terms of service page (you'll create this)
- `blog.html` - Blog page (referenced in footer)

### How to Edit the File

1. **Open** the `index.html` file with your text editor
2. **Locate** the section you want to change (use Find/Search: `Ctrl+F` on Windows or `Cmd+F` on Mac)
3. **Make your changes** carefully
4. **Save** the file (`Ctrl+S` or `Cmd+S`)
5. **Preview** by opening the file in your web browser

---

## Updating Text Content

### Understanding the Structure

The HTML file is organized into sections. Each section contains text that you can easily update. Here's what you need to know:

- **Text between `<h1>` tags**: Main headings (largest text)
- **Text between `<h2>` tags**: Section headings
- **Text between `<h3>` tags**: Subheadings
- **Text between `<p>` tags**: Paragraphs (regular text)
- **Text between `<span>` tags**: Inline text (small portions)

### Announcement Bar (Top of Page)

**Location**: Lines 91-93

**Current Text**:
```html
<div class="bg-blue-600 text-white py-3 px-4 text-center text-sm font-medium">
    <i class="fas fa-truck mr-2"></i>Fast Worldwide Shipping (5 days delivery) | 100% Satisfaction Guarantee
</div>
```

**How to Change It**:
1. Find the text "Fast Worldwide Shipping (5 days delivery) | 100% Satisfaction Guarantee"
2. Replace it with your announcement
3. **Example**: Change to "Join 50,000+ Leaders Worldwide | Transform Your Leadership Today"

**Result**:
```html
<div class="bg-blue-600 text-white py-3 px-4 text-center text-sm font-medium">
    <i class="fas fa-truck mr-2"></i>Join 50,000+ Leaders Worldwide | Transform Your Leadership Today
</div>
```

### Logo and Company Name

**Location**: Lines 100-106

**Current Code**:
```html
<a href="#home" class="flex items-center gap-2">
    <div class="w-10 h-10 bg-gradient-to-br from-blue-600 to-blue-800 rounded-lg flex items-center justify-center">
        <i class="fas fa-crown text-white text-lg"></i>
    </div>
    <span class="text-xl font-bold text-gray-900">Leadership</span>
</a>
```

**To Change the Company Name**:
1. Find the text `Leadership` (inside the `<span>` tag)
2. Replace it with your company name
3. **Example**: Change to "Elite Leaders Academy"

**Result**:
```html
<span class="text-xl font-bold text-gray-900">Elite Leaders Academy</span>
```

**To Change the Logo Icon**:
1. The icon is defined by `<i class="fas fa-crown text-white text-lg"></i>`
2. Replace `fa-crown` with another Font Awesome icon
3. **Common alternatives**:
   - `fa-star` (star icon)
   - `fa-rocket` (rocket icon)
   - `fa-lightbulb` (lightbulb icon)
   - `fa-graduation-cap` (graduation cap icon)
   - Find more at [fontawesome.com](https://fontawesome.com/icons)

**Example with rocket icon**:
```html
<i class="fas fa-rocket text-white text-lg"></i>
```

### Hero Section Headline

**Location**: Lines 152-155

**Current Text**:
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold text-white leading-tight mb-6 tracking-tight">
    Lead With Purpose and Influence
</h1>
```

**How to Change It**:
1. Find "Lead With Purpose and Influence"
2. Replace with your headline
3. **Example**: "Transform Your Leadership. Inspire Your Team."

**Result**:
```html
<h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold text-white leading-tight mb-6 tracking-tight">
    Transform Your Leadership. Inspire Your Team.
</h1>
```

### Hero Section Subheadline

**Location**: Lines 156-158

**Current Text**:
```html
<p class="text-lg sm:text-xl md:text-2xl text-gray-100 mb-8 leading-relaxed font-light">
    Transform Your Skills. Lead With Confidence.
</p>
```

**How to Change It**:
1. Find "Transform Your Skills. Lead With Confidence."
2. Replace with your subheadline
3. **Example**: "Master the skills that drive organizational success"

**Result**:
```html
<p class="text-lg sm:text-xl md:text-2xl text-gray-100 mb-8 leading-relaxed font-light">
    Master the skills that drive organizational success
</p>
```

### Features Section

**Location**: Lines 187-250

The Features section contains three feature cards. Here's how to update each:

**Feature 1 - Values-based Leadership**:

Find this section (around line 195):
```html
<h3 class="text-2xl font-bold text-gray-900 mb-3">Values-based Leadership</h3>
<p class="text-gray-600 leading-relaxed mb-4">
    Learn to lead with authentic values and principles...
</p>
```

**To update the feature title**:
- Change `Values-based Leadership` to your title
- Example: `Strategic Decision Making`

**To update the feature description**:
- Change the paragraph text to your description
- Keep the same structure and formatting

**To update the feature checklist items**:
- Find each `<li>` tag within the feature card
- Update the text after the checkmark icon
- Example: Change "Authentic leadership principles" to "Data-driven strategies"

**Feature 2 - Interactive Workshops** (around line 212):
- Follow the same process as Feature 1
- Update title, description, and checklist items

**Feature 3 - Comprehensive Courses** (around line 229):
- Follow the same process as Feature 1
- Update title, description, and checklist items

### Benefits Section

**Location**: Lines 253-360

This section has three benefit blocks. Here's how to update them:

**Benefit 1 - Accessible Growth**:

**To update the title** (around line 273):
```html
<h3 class="text-3xl font-bold text-gray-900 mb-4 gradient-text">Accessible Growth</h3>
```
Change `Accessible Growth` to your benefit title.

**To update the description** (around line 274):
```html
<p class="text-gray-600 leading-relaxed mb-6">
    We believe leadership development should be accessible...
</p>
```
Replace the paragraph text with your content.

**To update the benefit checklist** (around line 278-286):
```html
<div class="flex items-start gap-3">
    <i class="fas fa-check-circle text-blue-600 mt-1 flex-shrink-0"></i>
    <span class="text-gray-700"><strong>Flexible scheduling</strong> that fits your lifestyle</span>
</div>
```
- Change the text in the `<span>` tag to your benefit point
- Keep the checkmark icon and styling

**Benefit 2 - Unlock Your Full Potential** (around line 298):
- Follow the same process as Benefit 1

**Benefit 3 - Guidance to Soar** (around line 328):
- Follow the same process as Benefit 1

### Testimonials Section

**Location**: Lines 410-490

Each testimonial card has the same structure. Here's how to update one:

**Testimonial 1 - Sarah Mitchell**:

```html
<p class="text-gray-700 leading-relaxed mb-6">
    "The values-based leadership program completely transformed..."
</p>
```

**To update the testimonial text**:
1. Find the quoted text
2. Replace with your testimonial
3. Keep the quotation marks and structure

**To update the author name**:
```html
<p class="font-bold text-gray-900">Sarah Mitchell</p>
```
Change `Sarah Mitchell` to the person's name.

**To update the author title**:
```html
<p class="text-sm text-gray-600">CEO, TechVision Inc.</p>
```
Change `CEO, TechVision Inc.` to their actual title and company.

**To update the author initials** (the circle with letters):
```html
<div class="w-12 h-12 bg-blue-600 rounded-full flex items-center justify-center text-white font-bold">
    SM
</div>
```
Change `SM` to the person's initials.

**Repeat this process** for the other three testimonials (James Kumar, Amara Johnson, Robert Chen).

### FAQ Section

**Location**: Lines 493-570

Each FAQ item has a question and answer. Here's how to update them:

**FAQ 1 - What makes your programs different**:

**To update the question** (around line 503):
```html
<span class="text-lg font-semibold text-gray-900 text-left">What makes your leadership programs different from other academies?</span>
```
Replace the question text with your own question.

**To update the answer** (around line 507):
```html
<p>Our academy stands out through our unique focus on values-based leadership...</p>
```
Replace the paragraph text with your answer.

**Repeat this process** for FAQ items 2, 3, and 4.

**To add a new FAQ item**:
1. Find the last FAQ item (around line 550)
2. Copy the entire `<div class="accordion-item...">` block
3. Paste it after the last FAQ item
4. Update the question and answer text
5. The styling and functionality will work automatically

### About Us Section

**Location**: Lines 573-610

**To update the "Our Story" heading and text** (around line 591):
```html
<h3 class="text-2xl font-bold text-gray-900 mb-4">Our Story</h3>
<p class="text-gray-600 leading-relaxed">
    Founded in 2015, Leadership Academy emerged...
</p>
```
Replace the text with your company's story.

**To update the "Our Mission & Vision" section** (around line 600):
```html
<h3 class="text-2xl font-bold text-gray-900 mb-4">Our Mission & Vision</h3>
<p class="text-gray-600 leading-relaxed">
    Our mission is to empower leaders...
</p>
```
Replace the text with your mission and vision.

### Contact Section

**Location**: Lines 612-680

**To update contact information**:

**Email Address** (around line 629):
```html
<a href="mailto:leaddershipacademy@leaddership.co.za" class="text-gray-600 hover:text-blue-600 transition">
    leaddershipacademy@leaddership.co.za
</a>
```
Change the email address in both places:
1. In the `href="mailto:..."` part
2. In the visible text

**Example**:
```html
<a href="mailto:hello@yourcompany.com" class="text-gray-600 hover:text-blue-600 transition">
    hello@yourcompany.com
</a>
```

**Location** (around line 640):
```html
<p class="text-gray-600">
    Cape Town, South Africa
</p>
```
Change to your location.

### Footer Section

**Location**: Lines 683-780

**To update the footer company description** (around line 697):
```html
<p class="text-sm leading-relaxed mb-4">
    Empowering leaders worldwide to lead with purpose, integrity, and influence...
</p>
```
Replace with your company description.

**To update the year in copyright** (around line 765):
```html
&copy; <span id="year"></span> Leadership Academy. All rights reserved.
```
The year automatically updates via JavaScript, so you only need to change "Leadership Academy" to your company name.

---

## Modifying Tailwind CSS Classes

### Understanding Tailwind CSS

Tailwind CSS is a utility-first framework that uses pre-defined classes to style elements. Instead of writing custom CSS, you combine classes to create designs.

**Key Concept**: Each class does one specific thing (like `text-blue-600` makes text blue, `p-8` adds padding, etc.)

### Common Tailwind Classes Used in This Page

#### Text Styling

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-white` | Makes text white | `<p class="text-white">` |
| `text-gray-900` | Makes text dark gray | `<p class="text-gray-900">` |
| `text-blue-600` | Makes text blue | `<p class="text-blue-600">` |
| `text-lg` | Makes text larger | `<p class="text-lg">` |
| `text-xl` | Makes text even larger | `<p class="text-xl">` |
| `font-bold` | Makes text bold | `<p class="font-bold">` |
| `font-semibold` | Makes text semi-bold | `<p class="font-semibold">` |

#### Background Colors

| Class | What It Does |
|-------|-------------|
| `bg-white` | White background |
| `bg-blue-600` | Blue background |
| `bg-gray-50` | Light gray background |
| `bg-gray-900` | Dark gray/black background |

#### Spacing

| Class | What It Does | Size |
|-------|-------------|------|
| `p-4` | Padding (space inside) | Small |
| `p-8` | Padding | Medium |
| `px-4` | Horizontal padding only | Small |
| `py-4` | Vertical padding only | Small |
| `mb-4` | Margin bottom (space below) | Small |
| `mb-8` | Margin bottom | Medium |
| `gap-4` | Space between items | Small |

#### Display & Layout

| Class | What It Does |
|-------|-------------|
| `flex` | Makes items display in a row |
| `grid` | Makes items display in columns |
| `hidden` | Hides the element |
| `block` | Shows the element as a block |
| `rounded-lg` | Rounded corners |
| `rounded-xl` | More rounded corners |

#### Responsive Design

Tailwind uses prefixes to make designs responsive:

| Prefix | Screen Size | Use Case |
|--------|------------|----------|
| (no prefix) | Mobile (small screens) | Default styling |
| `sm:` | Small screens (640px+) | Tablets |
| `md:` | Medium screens (768px+) | Larger tablets |
| `lg:` | Large screens (1024px+) | Desktops |

**Example**:
```html
<h1 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl">
```
This means:
- On mobile: text size 2xl
- On tablets (sm): text size 3xl
- On larger tablets (md): text size 4xl
- On desktops (lg): text size 5xl

### How to Change Colors

**Current Color Scheme**:
- Primary Blue: `blue-600` and `blue-800`
- Text: `gray-900` (dark), `gray-600` (medium), `gray-100` (light)
- Backgrounds: `white`, `gray-50`, `gray-900`

**To change the primary blue to another color**:

1. **Find all instances** of `blue-600` and `blue-800` (use Find: `Ctrl+F`)
2. **Replace with your color** using Tailwind color names:
   - `red-600`, `green-600`, `purple-600`, `indigo-600`, `teal-600`, etc.

**Example - Change from blue to purple**:

Original:
```html
<a href="https://leaddership.co.za/courses" class="btn-primary bg-blue-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-blue-700">
    Enroll Now
</a>
```

Changed:
```html
<a href="https://leaddership.co.za/courses" class="btn-primary bg-purple-600 text-white px-6 py-2 rounded-lg font-semibold hover:bg-purple-700">
    Enroll Now
</a>
```

**Find and Replace Steps**:
1. Open Find & Replace (`Ctrl+H` on Windows, `Cmd+Shift+H` on Mac)
2. Find: `blue-600`
3. Replace All with: `purple-600`
4. Find: `blue-800`
5. Replace All with: `purple-800`
6. Find: `blue-700`
7. Replace All with: `purple-700`
8. Find: `blue-100`
9. Replace All with: `purple-100`

### How to Change Button Styling

**Current Button** (Hero section, around line 161):
```html
<a href="https://leaddership.co.za/courses" class="btn-primary bg-blue-600 text-white px-8 py-4 rounded-lg font-bold text-lg hover:bg-blue-700 inline-block">
    Start Your Journey
    <i class="fas fa-arrow-right ml-2"></i>
</a>
```

**To make the button larger**:
- Change `px-8 py-4` to `px-10 py-6`
- Change `text-lg` to `text-xl`

**To make the button smaller**:
- Change `px-8 py-4` to `px-6 py-2`
- Change `text-lg` to `text-sm`

**To make the button more rounded**:
- Change `rounded-lg` to `rounded-full`

**To change button text color**:
- Change `text-white` to `text-blue-600` (or any other color)

### How to Change Spacing

**Current Feature Cards** (around line 190):
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
```

The `gap-8` creates space between cards.

**To increase space between cards**:
- Change `gap-8` to `gap-12`

**To decrease space between cards**:
- Change `gap-8` to `gap-4`

**To change padding inside cards** (around line 194):
```html
<div class="feature-card card-hover bg-white border border-gray-200 rounded-xl p-8 hover:border-blue-300">
```

The `p-8` is the internal padding.

**To increase internal padding**:
- Change `p-8` to `p-12`

**To decrease internal padding**:
- Change `p-8` to `p-4`

### How to Change Responsive Breakpoints

**Example - Make features display as 2 columns on larger screens instead of 3**:

Current (around line 190):
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
```

Changed:
```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
```

This removes the `lg:grid-cols-3`, so it will always be 2 columns on medium screens and up.

### How to Change Box Shadows

**Current Testimonial Cards** (around line 420):
```html
<div class="testimonial-card bg-white p-8 rounded-xl border border-gray-200">
```

To add a shadow effect:
```html
<div class="testimonial-card bg-white p-8 rounded-xl border border-gray-200 shadow-lg">
```

Shadow options:
- `shadow-sm` (subtle)
- `shadow` (default)
- `shadow-md` (medium)
- `shadow-lg` (large)
- `shadow-xl` (extra large)

### How to Change Border Styles

**Current Feature Cards** (around line 194):
```html
<div class="feature-card card-hover bg-white border border-gray-200 rounded-xl p-8 hover:border-blue-300">
```

The `border border-gray-200` creates a light gray border.

**To remove the border**:
- Delete `border border-gray-200`

**To make the border thicker**:
- Change `border` to `border-2`

**To change border color**:
- Change `border-gray-200` to `border-blue-300` (or any other color)

### Troubleshooting CSS Changes

**Problem**: Changes don't appear in browser
- **Solution**: Hard refresh your browser (`Ctrl+Shift+R` on Windows, `Cmd+Shift+R` on Mac)

**Problem**: Layout breaks on mobile
- **Solution**: Check that you haven't removed responsive prefixes (sm:, md:, lg:)

**Problem**: Colors don't match expectations
- **Solution**: Tailwind color names follow a pattern. Use `color-number` (e.g., `blue-600`, `gray-900`)

---

## Fixing and Managing Links

### Understanding Links in Your Page

Links are created using the `<a>` tag with an `href` attribute that specifies where the link goes.

**Basic Structure**:
```html
<a href="destination-url">Link Text</a>
```

- `href` = where the link points to
- `Link Text` = what users see and click

### Navigation Menu Links

**Location**: Lines 109-116 (Desktop Navigation)

**Current Code**:
```html
<nav class="hidden md:flex items-center gap-8">
    <a href="#home" class="nav-link text-gray-700 font-medium">Home</a>
    <a href="#features" class="nav-link text-gray-700 font-medium">Features</a>
    <a href="#benefits" class="nav-link text-gray-700 font-medium">Benefits</a>
    <a href="#about" class="nav-link text-gray-700 font-medium">About</a>
    <a href="#testimonials" class="nav-link text-gray-700 font-medium">Testimonials</a>
    <a href="#faq" class="nav-link text-gray-700 font-medium">FAQ</a>
    <a href="#contact" class="nav-link text-gray-700 font-medium">Contact</a>
</nav>
```

**Understanding the `#` symbol**:
- The `#` means "jump to this section on the same page"
- `#home` jumps to the element with `id="home"`
- This is called an "anchor link"

**Status**: ✅ These links are correct and working!

### Mobile Navigation Menu Links

**Location**: Lines 135-142

**Current Code**:
```html
<div class="mobile-menu hidden md:hidden pb-4 border-t border-gray-200">
    <a href="#home" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded transition">Home</a>
    <a href="#features" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded transition">Features</a>
    <!-- ... more links ... -->
</div>
```

**Status**: ✅ These links are correct and working!

### Call-to-Action (CTA) Button Links

**Location**: Multiple locations (Hero section, Features section, etc.)

**Current Code** (Hero section, around line 161):
```html
<a href="https://leaddership.co.za/courses" class="btn-primary bg-blue-600 text-white px-8 py-4 rounded-lg font-bold text-lg hover:bg-blue-700 inline-block">
    Start Your Journey
    <i class="fas fa-arrow-right ml-2"></i>
</a>
```

**To update the destination URL**:
1. Find the `href="https://leaddership.co.za/courses"`
2. Replace with your actual courses page URL
3. **Example**: If your courses are at `https://yourcompany.com/programs`:

```html
<a href="https://yourcompany.com/programs" class="btn-primary bg-blue-600 text-white px-8 py-4 rounded-lg font-bold text-lg hover:bg-blue-700 inline-block">
    Start Your Journey
    <i class="fas fa-arrow-right ml-2"></i>
</a>
```

**All CTA buttons that need updating**:

| Location | Current URL | Line |
|----------|------------|------|
| Hero Section | `https://leaddership.co.za/courses` | 161 |
| Hero Section (Learn More) | `#benefits` | 165 |
| Features Section (End) | `https://leaddership.co.za/courses` | 252 |
| Benefits Section (End) | `https://leaddership.co.za/courses` | 362 |
| About Section (End) | `https://leaddership.co.za/courses` | 409 |
| Footer (Mobile Enroll) | `https://leaddership.co.za/courses` | 139 |
| Footer (Desktop Enroll) | `https://leaddership.co.za/courses` | 127 |
| CTA Section 2 | `https://leaddership.co.za/courses` | 565 |

**How to Find and Update All CTA Links**:

1. **Open Find & Replace** (`Ctrl+H` or `Cmd+Shift+H`)
2. **Find**: `https://leaddership.co.za/courses`
3. **Replace All with**: Your actual courses page URL
4. **Click Replace All**

**Example**: If your courses are at `https://academy.com/enrollment`:
- Find: `https://leaddership.co.za/courses`
- Replace All with: `https://academy.com/enrollment`

### Footer Links

**Location**: Lines 697-750

#### Quick Links Section

**Current Code** (around line 717):
```html
<h4 class="text-lg font-bold text-white mb-6">Quick Links</h4>
<ul class="space-y-3">
    <li><a href="#home" class="hover:text-blue-400 transition duration-300">Home</a></li>
    <li><a href="#features" class="hover:text-blue-400 transition duration-300">Features</a></li>
    <li><a href="#benefits" class="hover:text-blue-400 transition duration-300">Benefits</a></li>
    <li><a href="#about" class="hover:text-blue-400 transition duration-300">About Us</a></li>
    <li><a href="#testimonials" class="hover:text-blue-400 transition duration-300">Testimonials</a></li>
    <li><a href="#faq" class="hover:text-blue-400 transition duration-300">FAQ</a></li>
</ul>
```

**Status**: ✅ These links are correct!

#### Resources Section

**Current Code** (around line 730):
```html
<h4 class="text-lg font-bold text-white mb-6">Resources</h4>
<ul class="space-y-3">
    <li><a href="https://leaddership.co.za/courses" class="hover:text-blue-400 transition duration-300">All Courses</a></li>
    <li><a href="blog.html" class="hover:text-blue-400 transition duration-300">Blog</a></li>
    <li><a href="#" class="hover:text-blue-400 transition duration-300">Webinars</a></li>
    <li><a href="#" class="hover:text-blue-400 transition duration-300">Community</a></li>
    <li><a href="#" class="hover:text-blue-400 transition duration-300">Events</a></li>
    <li><a href="#" class="hover:text-blue-400 transition duration-300">Support</a></li>
</ul>
```

**Issues to Fix**:
1. ❌ `href="https://leaddership.co.za/courses"` - needs to be updated
2. ❌ `href="blog.html"` - file needs to exist or be created
3. ❌ `href="#"` - these are placeholder links

**How to Fix**:

**For "All Courses" link**:
```html
<li><a href="https://yourcompany.com/programs" class="hover:text-blue-400 transition duration-300">All Courses</a></li>
```

**For "Blog" link** (if you have a blog page):
```html
<li><a href="blog.html" class="hover:text-blue-400 transition duration-300">Blog</a></li>
```

**For placeholder links** (if you don't have these pages yet):
- Option 1: Remove the link entirely
- Option 2: Link to a coming soon page
- Option 3: Link to a relevant external resource

**Example - Remove a placeholder link**:

Instead of:
```html
<li><a href="#" class="hover:text-blue-400 transition duration-300">Webinars</a></li>
```

Either remove it completely or comment it out:
```html
<!-- <li><a href="#" class="hover:text-blue-400 transition duration-300">Webinars</a></li> -->
```

#### Legal Section

**Current Code** (around line 743):
```html
<h4 class="text-lg font-bold text-white mb-6">Legal</h4>
<ul class="space-y-3">
    <li><a href="privacy.html" class="hover:text-blue-400 transition duration-300">Privacy Policy</a></li>
    <li><a href="terms.html" class="hover:text-blue-400 transition duration-300">Terms of Service</a></li>
    <li><a href="#" class="hover:text-blue-400 transition duration-300">Cookie Policy</a></li>
    <li><a href="#" class="hover:text-blue-400 transition duration-300">Accessibility</a></li>
    <li><a href="#" class="hover:text-blue-400 transition duration-300">Contact Us</a></li>
</ul>
```

**Status**: ⚠️ These links reference files that don't exist yet
- `privacy.html` - needs to be created
- `terms.html` - needs to be created
- Other links are placeholders

**We'll fix these in the next section!**

### Contact Email Link

**Location**: Line 629

**Current Code**:
```html
<a href="mailto:leaddershipacademy@leaddership.co.za" class="text-gray-600 hover:text-blue-600 transition">
    leaddershipacademy@leaddership.co.za
</a>
```

**To update the email address**:
1. Change the email in `href="mailto:..."`
2. Change the displayed email text
3. **Make sure both match!**

**Example**:
```html
<a href="mailto:hello@yourcompany.com" class="text-gray-600 hover:text-blue-600 transition">
    hello@yourcompany.com
</a>
```

### Complete Link Update Checklist

Use this checklist to ensure all links are correct:

- [ ] All navigation menu links (`#home`, `#features`, etc.) point to correct sections
- [ ] All CTA buttons link to your actual courses page
- [ ] Email link is your correct contact email
- [ ] Location information is accurate
- [ ] Blog link points to your blog page (or is removed)
- [ ] Privacy and Terms links point to your policy pages (we'll create these next)
- [ ] Placeholder links (`href="#"`) are either removed or replaced

---

## Adding Privacy and Terms Pages

### Why You Need These Pages

Privacy Policy and Terms of Service pages are:
- **Legally important** - they protect your business
- **User trust** - they show you're transparent
- **SEO benefit** - search engines favor sites with proper policies
- **Required by law** - many jurisdictions require them

### Step 1: Create the Privacy Policy Page

**To create `privacy.html`**:

1. **Open your text editor**
2. **Create a new file**
3. **Copy the following code** (this is a template):

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Leadership Academy">
    <meta name="keywords" content="privacy, policy, data protection">
    <title>Privacy Policy - Leadership Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');
        * {
            font-family: 'Inter', sans-serif;
        }
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header/Navigation (Copy from index.html) -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex-shrink-0">
                    <a href="index.html" class="flex items-center gap-2">
                        <div class="w-10 h-10 bg-gradient-to-br from-blue-600 to-blue-800 rounded-lg flex items-center justify-center">
                            <i class="fas fa-crown text-white text-lg"></i>
                        </div>
                        <span class="text-xl font-bold text-gray-900">Leadership</span>
                    </a>
                </div>
                <nav class="hidden md:flex items-center gap-8">
                    <a href="index.html#home" class="text-gray-700 font-medium hover:text-blue-600 transition">Home</a>
                    <a href="index.html#features" class="text-gray-700 font-medium hover:text-blue-600 transition">Features</a>
                    <a href="index.html#about" class="text-gray-700 font-medium hover:text-blue-600 transition">About</a>
                    <a href="index.html#contact" class="text-gray-700 font-medium hover:text-blue-600 transition">Contact</a>
                </nav>
                <button class="mobile-menu-button md:hidden text-gray-700 focus:outline-none">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <h1 class="text-5xl font-bold text-gray-900 mb-4">Privacy Policy</h1>
        <p class="text-gray-600 mb-8">Last updated: <span id="date"></span></p>

        <div class="prose prose-lg max-w-none space-y-8">
            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">1. Introduction</h2>
                <p class="text-gray-600 leading-relaxed">
                    Leadership Academy ("we", "us", "our", or "Company") operates the website. This page informs you of our policies regarding the collection, use, and disclosure of personal data when you use our Service and the choices you have associated with that data.
                </p>
                <p class="text-gray-600 leading-relaxed">
                    We use your data to provide and improve the Service. By using the Service, you agree to the collection and use of information in accordance with this policy.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">2. Information Collection and Use</h2>
                <p class="text-gray-600 leading-relaxed mb-4">
                    We collect several different types of information for various purposes to provide and improve our Service to you.
                </p>
                <h3 class="text-2xl font-semibold text-gray-900 mb-3">Types of Data Collected:</h3>
                <ul class="list-disc list-inside space-y-2 text-gray-600">
                    <li><strong>Personal Data:</strong> Name, email address, phone number, physical address</li>
                    <li><strong>Usage Data:</strong> Browser type, IP address, pages visited, time and date of visit</li>
                    <li><strong>Course Data:</strong> Progress, completion status, assessment scores</li>
                    <li><strong>Payment Data:</strong> Transaction history (processed securely)</li>
                </ul>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">3. Use of Data</h2>
                <p class="text-gray-600 leading-relaxed mb-4">
                    Leadership Academy uses the collected data for various purposes:
                </p>
                <ul class="list-disc list-inside space-y-2 text-gray-600">
                    <li>To provide and maintain our Service</li>
                    <li>To notify you about changes to our Service</li>
                    <li>To allow you to participate in interactive features of our Service</li>
                    <li>To provide customer support</li>
                    <li>To gather analysis or valuable information so we can improve our Service</li>
                    <li>To monitor the usage of our Service</li>
                    <li>To detect, prevent and address technical issues</li>
                </ul>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">4. Security of Data</h2>
                <p class="text-gray-600 leading-relaxed">
                    The security of your data is important to us but remember that no method of transmission over the Internet or method of electronic storage is 100% secure. While we strive to use commercially acceptable means to protect your Personal Data, we cannot guarantee its absolute security.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">5. Changes to This Privacy Policy</h2>
                <p class="text-gray-600 leading-relaxed">
                    We may update our Privacy Policy from time to time. We will notify you of any changes by posting the new Privacy Policy on this page and updating the "Last updated" date at the top of this Privacy Policy.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">6. Contact Us</h2>
                <p class="text-gray-600 leading-relaxed">
                    If you have any questions about this Privacy Policy, please contact us at:
                </p>
                <p class="text-gray-600 leading-relaxed mt-4">
                    <strong>Email:</strong> <a href="mailto:privacy@leaddership.co.za" class="text-blue-600 hover:text-blue-700">privacy@leaddership.co.za</a><br>
                    <strong>Address:</strong> Cape Town, South Africa
                </p>
            </section>
        </div>
    </main>

    <!-- Footer (Copy from index.html) -->
    <footer class="bg-gray-900 text-gray-300 py-16 mt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="border-t border-gray-800 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center gap-4">
                    <p class="text-sm text-gray-400">
                        &copy; <span id="year"></span> Leadership Academy. All rights reserved.
                    </p>
                    <div class="flex gap-6 text-sm">
                        <a href="privacy.html" class="text-gray-400 hover:text-blue-400 transition duration-300">Privacy</a>
                        <a href="terms.html" class="text-gray-400 hover:text-blue-400 transition duration-300">Terms</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Set current date
        const options = { year: 'numeric', month: 'long', day: 'numeric' };
        document.getElementById('date').textContent = new Date().toLocaleDateString('en-US', options);
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
```

4. **Save the file** as `privacy.html` in the same folder as `index.html`

### Step 2: Create the Terms of Service Page

**To create `terms.html`**:

1. **Open your text editor**
2. **Create a new file**
3. **Copy the following code**:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Leadership Academy">
    <meta name="keywords" content="terms, service, agreement, conditions">
    <title>Terms of Service - Leadership Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');
        * {
            font-family: 'Inter', sans-serif;
        }
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header/Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <div class="flex-shrink-0">
                    <a href="index.html" class="flex items-center gap-2">
                        <div class="w-10 h-10 bg-gradient-to-br from-blue-600 to-blue-800 rounded-lg flex items-center justify-center">
                            <i class="fas fa-crown text-white text-lg"></i>
                        </div>
                        <span class="text-xl font-bold text-gray-900">Leadership</span>
                    </a>
                </div>
                <nav class="hidden md:flex items-center gap-8">
                    <a href="index.html#home" class="text-gray-700 font-medium hover:text-blue-600 transition">Home</a>
                    <a href="index.html#features" class="text-gray-700 font-medium hover:text-blue-600 transition">Features</a>
                    <a href="index.html#about" class="text-gray-700 font-medium hover:text-blue-600 transition">About</a>
                    <a href="index.html#contact" class="text-gray-700 font-medium hover:text-blue-600 transition">Contact</a>
                </nav>
                <button class="mobile-menu-button md:hidden text-gray-700 focus:outline-none">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <h1 class="text-5xl font-bold text-gray-900 mb-4">Terms of Service</h1>
        <p class="text-gray-600 mb-8">Last updated: <span id="date"></span></p>

        <div class="prose prose-lg max-w-none space-y-8">
            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">1. Agreement to Terms</h2>
                <p class="text-gray-600 leading-relaxed">
                    By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">2. Use License</h2>
                <p class="text-gray-600 leading-relaxed mb-4">
                    Permission is granted to temporarily download one copy of the materials (information or software) on Leadership Academy's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                </p>
                <ul class="list-disc list-inside space-y-2 text-gray-600">
                    <li>Modifying or copying the materials</li>
                    <li>Using the materials for any commercial purpose or for any public display</li>
                    <li>Attempting to decompile or reverse engineer any software contained on the website</li>
                    <li>Removing any copyright or other proprietary notations from the materials</li>
                    <li>Transferring the materials to another person or "mirroring" the materials on any other server</li>
                </ul>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">3. Disclaimer</h2>
                <p class="text-gray-600 leading-relaxed">
                    The materials on Leadership Academy's website are provided "as is". Leadership Academy makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">4. Limitations</h2>
                <p class="text-gray-600 leading-relaxed">
                    In no event shall Leadership Academy or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on the website, even if Leadership Academy or an authorized representative has been notified orally or in writing of the possibility of such damage.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">5. Accuracy of Materials</h2>
                <p class="text-gray-600 leading-relaxed">
                    The materials appearing on Leadership Academy's website could include technical, typographical, or photographic errors. Leadership Academy does not warrant that any of the materials on the website are accurate, complete, or current. Leadership Academy may make changes to the materials contained on the website at any time without notice.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">6. Links</h2>
                <p class="text-gray-600 leading-relaxed">
                    Leadership Academy has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Leadership Academy of the site. Use of any such linked website is at the user's own risk.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">7. Modifications</h2>
                <p class="text-gray-600 leading-relaxed">
                    Leadership Academy may revise these terms of service for the website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">8. Governing Law</h2>
                <p class="text-gray-600 leading-relaxed">
                    These terms and conditions are governed by and construed in accordance with the laws of South Africa, and you irrevocably submit to the exclusive jurisdiction of the courts located in Cape Town, South Africa.
                </p>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-gray-900 mb-4">9. Contact Information</h2>
                <p class="text-gray-600 leading-relaxed">
                    If you have any questions about these Terms of Service, please contact us at:
                </p>
                <p class="text-gray-600 leading-relaxed mt-4">
                    <strong>Email:</strong> <a href="mailto:legal@leaddership.co.za" class="text-blue-600 hover:text-blue-700">legal@leaddership.co.za</a><br>
                    <strong>Address:</strong> Cape Town, South Africa
                </p>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-16 mt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="border-t border-gray-800 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center gap-4">
                    <p class="text-sm text-gray-400">
                        &copy; <span id="year"></span> Leadership Academy. All rights reserved.
                    </p>
                    <div class="flex gap-6 text-sm">
                        <a href="privacy.html" class="text-gray-400 hover:text-blue-400 transition duration-300">Privacy</a>
                        <a href="terms.html" class="text-gray-400 hover:text-blue-400 transition duration-300">Terms</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Set current date
        const options = { year: 'numeric', month: 'long', day: 'numeric' };
        document.getElementById('date').textContent = new Date().toLocaleDateString('en-US', options);
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
```

4. **Save the file** as `terms.html` in the same folder as `index.html`

### Step 3: Verify the Links Work

**To test the links**:

1. **Open `index.html`** in your web browser
2. **Scroll to the footer**
3. **Click on "Privacy Policy"** - should open `privacy.html`
4. **Click on "Terms of Service"** - should open `terms.html`
5. **On the policy pages, click the logo** - should return to `index.html`

### Step 4: Customize Your Policy Pages

Now that you have the basic templates, customize them with your actual information:

**In `privacy.html`, update**:
- Email address: Change `privacy@leaddership.co.za` to your email
- Location: Change "Cape Town, South Africa" to your location
- Content: Replace the generic text with your specific privacy practices
- Company name: Replace "Leadership Academy" with your company name

**In `terms.html`, update**:
- Email address: Change `legal@leaddership.co.za` to your email
- Location: Change "Cape Town, South Africa" to your location
- Governing Law: Change "South Africa" to your jurisdiction
- Content: Replace the generic text with your specific terms
- Company name: Replace "Leadership Academy" with your company name

### Important Privacy Considerations

**⚠️ These are template pages. You should**:

1. **Consult a lawyer** - Privacy policies and terms should be reviewed by legal professionals
2. **Use a policy generator** - Services like Termly, iubenda, or Privacypolicies.com can generate customized policies
3. **Keep them updated** - Review annually or when your practices change
4. **Be transparent** - Accurately describe how you collect and use data

---

## Common Customization Tasks

### Task 1: Change the Color Scheme

**Goal**: Change from blue to a different color

**Steps**:

1. **Open Find & Replace** (`Ctrl+H` or `Cmd+Shift+H`)
2. **Replace all instances of `blue-600`** with your chosen color
3. **Replace all instances of `blue-800`** with a darker shade
4. **Replace all instances of `blue-700`** with a medium shade
5. **Replace all instances of `blue-100`** with a light shade

**Example - Change to Green**:
- Find: `blue-600` → Replace: `green-600`
- Find: `blue-800` → Replace: `green-800`
- Find: `blue-700` → Replace: `green-700`
- Find: `blue-100` → Replace: `green-100`

**Tailwind Color Options**:
- `red`, `orange`, `yellow`, `green`, `teal`, `cyan`, `blue`, `indigo`, `purple`, `pink`, `rose`

### Task 2: Add a New Feature Card

**Goal**: Add a fourth feature to the Features section

**Steps**:

1. **Find the Features section** (around line 190)
2. **Locate the last feature card** (Comprehensive Courses)
3. **Copy the entire `<div class="feature-card...">` block** (lines 229-246)
4. **Paste it after the last feature card**
5. **Update the content**:
   - Change the icon (replace `fa-book`)
   - Change the title
   - Change the description
   - Update the checklist items

**Example**:

```html
<!-- Feature 4: Community Support (NEW) -->
<div class="feature-card card-hover bg-white border border-gray-200 rounded-xl p-8 hover:border-blue-300">
    <div class="mb-6">
        <div class="feature-icon w-14 h-14 bg-blue-100 rounded-lg flex items-center justify-center mb-4">
            <i class="fas fa-network-wired text-2xl text-blue-600"></i>
        </div>
    </div>
    <h3 class="text-2xl font-bold text-gray-900 mb-3">Community Support</h3>
    <p class="text-gray-600 leading-relaxed mb-4">
        Join a vibrant community of leaders committed to growth and mutual support.
    </p>
    <ul class="space-y-2 text-gray-600 text-sm">
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-green-500"></i>
            <span>Peer networking opportunities</span>
        </li>
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-green-500"></i>
            <span>Group discussions and forums</span>
        </li>
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-green-500"></i>
            <span>Collaborative projects</span>
        </li>
    </ul>
</div>
```

**Important**: Also update the grid to show 4 columns on large screens:
- Find: `lg:grid-cols-3`
- Change to: `lg:grid-cols-4`

Or keep it as 3 columns and let the 4th wrap to a new row.

### Task 3: Update Hero Background Image

**Goal**: Change the hero section background image

**Location**: Line 150

**Current Code**:
```html
<img src="https://images.unsplash.com/photo-1504093376055-b3094b674dcb?w=1600&h=900&fit=crop&q=80" alt="Leadership hero background" class="w-full h-full object-cover">
```

**To change the image**:

1. **Find a new image** from:
   - Unsplash: `https://unsplash.com`
   - Pexels: `https://pexels.com`
   - Pixabay: `https://pixabay.com`

2. **Copy the image URL**

3. **Replace the `src` value**:

```html
<img src="YOUR_NEW_IMAGE_URL" alt="Leadership hero background" class="w-full h-full object-cover">
```

**Example**:
```html
<img src="https://images.unsplash.com/photo-1552664730-d307ca884978?w=1600&h=900&fit=crop&q=80" alt="Leadership hero background" class="w-full h-full object-cover">
```

### Task 4: Change Section Background Colors

**Goal**: Change the background color of a section

**Location Examples**:
- Benefits section: Line 253 (`bg-gray-50`)
- CTA section: Line 362 (`bg-gradient-to-r from-blue-600 to-blue-800`)
- Footer: Line 683 (`bg-gray-900`)

**To change a simple background color**:

**Current**:
```html
<section id="benefits" class="py-20 sm:py-24 bg-gray-50">
```

**Changed to white**:
```html
<section id="benefits" class="py-20 sm:py-24 bg-white">
```

**Changed to light blue**:
```html
<section id="benefits" class="py-20 sm:py-24 bg-blue-50">
```

### Task 5: Add a Newsletter Signup Form

**Goal**: Add an email subscription form to the CTA section

**Location**: After line 568 (CTA Section 2)

**Add this code**:

```html
<!-- Newsletter Signup Section -->
<section class="py-20 sm:py-24 bg-blue-50">
    <div class="max-w-2xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h2 class="text-4xl font-bold text-gray-900 mb-6">
            Stay Updated on Leadership Tips
        </h2>
        <p class="text-lg text-gray-600 mb-8">
            Subscribe to our newsletter for exclusive insights and resources delivered to your inbox.
        </p>
        <form class="flex flex-col sm:flex-row gap-3 max-w-md mx-auto">
            <input type="email" placeholder="Enter your email" required class="flex-1 px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
            <button type="submit" class="bg-blue-600 text-white px-8 py-3 rounded-lg font-bold hover:bg-blue-700 transition duration-300">
                Subscribe
            </button>
        </form>
        <p class="text-sm text-gray-600 mt-4">
            We respect your privacy. Unsubscribe at any time.
        </p>
    </div>
</section>
```

### Task 6: Modify Button Styling

**Goal**: Make all buttons have a different style

**Current Button Style** (around line 161):
```html
<a href="https://leaddership.co.za/courses" class="btn-primary bg-blue-600 text-white px-8 py-4 rounded-lg font-bold text-lg hover:bg-blue-700 inline-block">
```

**To make buttons more rounded** (pill-shaped):
- Change `rounded-lg` to `rounded-full`

**To make buttons with outline style** (instead of filled):
- Change `bg-blue-600 text-white` to `bg-transparent text-blue-600 border-2 border-blue-600`
- Change `hover:bg-blue-700` to `hover:bg-blue-600 hover:text-white`

**Example - Outline button**:
```html
<a href="https://leaddership.co.za/courses" class="btn-primary bg-transparent text-blue-600 border-2 border-blue-600 px-8 py-4 rounded-lg font-bold text-lg hover:bg-blue-600 hover:text-white inline-block">
    Start Your Journey
    <i class="fas fa-arrow-right ml-2"></i>
</a>
```

### Task 7: Add Social Media Links

**Goal**: Update social media links in the footer

**Location**: Lines 708-716

**Current Code**:
```html
<div class="flex gap-4">
    <a href="#" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-blue-600 transition duration-300">
        <i class="fab fa-facebook-f text-white"></i>
    </a>
    <a href="#" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-blue-600 transition duration-300">
        <i class="fab fa-twitter text-white"></i>
    </a>
    <!-- ... more social links ... -->
</div>
```

**To add your social media URLs**:

Replace `href="#"` with your actual social media links:

```html
<div class="flex gap-4">
    <a href="https://facebook.com/yourpage" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-blue-600 transition duration-300">
        <i class="fab fa-facebook-f text-white"></i>
    </a>
    <a href="https://twitter.com/yourhandle" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-blue-600 transition duration-300">
        <i class="fab fa-twitter text-white"></i>
    </a>
    <a href="https://linkedin.com/company/yourcompany" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-blue-600 transition duration-300">
        <i class="fab fa-linkedin-in text-white"></i>
    </a>
    <a href="https://instagram.com/yourprofile" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-blue-600 transition duration-300">
        <i class="fab fa-instagram text-white"></i>
    </a>
</div>
```

### Task 8: Change Typography

**Goal**: Change the main font or heading sizes

**Current Font**: Inter (imported at line 46)

**To change the font**:

1. **Find the import statement** (line 46):
```html
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap');
```

2. **Replace with a different Google Font**:
```html
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap');
```

3. **Update the font-family** (line 49):

From:
```css
* {
    font-family: 'Inter', sans-serif;
}
```

To:
```css
* {
    font-family: 'Poppins', sans-serif;
}
```

**Popular Google Fonts**:
- Poppins
- Playfair Display
- Raleway
- Montserrat
- Open Sans
- Lato
- Roboto

Find more at [fonts.google.com](https://fonts.google.com)

---

## Troubleshooting

### General Issues

#### Problem: Changes don't appear in the browser

**Solution**:
1. **Save the file** - Make sure you saved your changes (`Ctrl+S`)
2. **Hard refresh** - Press `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)
3. **Clear cache** - Try opening in an incognito/private window
4. **Check file location** - Make sure the file is saved in the correct folder

#### Problem: Layout looks broken on mobile

**Solution**:
1. **Check responsive classes** - Ensure you haven't removed `sm:`, `md:`, or `lg:` prefixes
2. **Verify grid classes** - Make sure grid columns are properly defined
3. **Test in browser** - Open Developer Tools (`F12`) and toggle device toolbar
4. **Review changes** - Undo recent changes if layout was working before

#### Problem: Text is cut off or overlapping

**Solution**:
1. **Check padding** - Add `p-4` or `p-8` to elements if needed
2. **Check max-width** - Ensure containers have `max-w-` classes
3. **Check line-height** - Add `leading-relaxed` to paragraphs
4. **Test different screen sizes** - Some issues only appear on specific sizes

### Link Issues

#### Problem: Links don't work

**Solution**:
1. **Check the `href` value** - Make sure it's correctly formatted
2. **For internal links** - Use `#section-id` format
3. **For external links** - Use full URL with `https://`
4. **Test in browser** - Check the browser console for errors (`F12`)

**Example - Correct formats**:
```html
<!-- Internal link -->
<a href="#features">Features</a>

<!-- External link -->
<a href="https://example.com">Example</a>

<!-- Email link -->
<a href="mailto:hello@example.com">Email</a>

<!-- Phone link -->
<a href="tel:+1234567890">Call Us</a>
```

#### Problem: External links open in same tab (want new tab)

**Solution**: Add `target="_blank"` to the link:

```html
<a href="https://example.com" target="_blank">External Link</a>
```

#### Problem: Links don't match the site styling

**Solution**: Add the appropriate classes:

```html
<!-- Navigation link -->
<a href="#section" class="nav-link text-gray-700 font-medium">Link</a>

<!-- Button link -->
<a href="#section" class="btn-primary bg-blue-600 text-white px-6 py-2 rounded-lg font-semibold">Button</a>
```

### CSS/Styling Issues

#### Problem: Colors don't match what I expected

**Solution**:
1. **Use correct Tailwind names** - Format is `color-number` (e.g., `blue-600`)
2. **Check number range** - Usually 50, 100, 200...900
3. **Test in browser** - Some colors look different on screen vs. design
4. **Use color tools** - Check [tailwindcss.com/docs/colors](https://tailwindcss.com/docs/colors)

**Color number guide**:
- `50` = very light
- `100-300` = light
- `400-500` = medium
- `600-700` = dark
- `800-900` = very dark

#### Problem: Spacing looks wrong

**Solution**:
1. **Understand padding vs margin**:
   - `p-` = padding (space inside)
   - `m-` = margin (space outside)
2. **Check responsive sizes** - You might need different spacing on mobile
3. **Use gap for spacing between items** - Better than margin

**Spacing scale**:
- `2` = 8px
- `4` = 16px
- `6` = 24px
- `8` = 32px
- `12` = 48px

#### Problem: Text is too small or too large

**Solution**:
1. **Adjust text size classes**:
   - `text-sm` = small
   - `text-base` = normal
   - `text-lg` = large
   - `text-xl` = extra large
   - `text-2xl` = 2x large
   - `text-3xl` = 3x large

2. **Use responsive sizes**:
```html
<h1 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl">
```

### Form Issues

#### Problem: Form inputs don't look right

**Solution**: Add proper styling:

```html
<input type="text" class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500">
```

#### Problem: Form submission doesn't work

**Solution**: The form needs a backend service. Currently, it shows an alert. To make it functional:

1. **Use a form service** like Formspree, Netlify Forms, or EmailJS
2. **Follow their documentation** to add the necessary code
3. **Update the `action` attribute** if using traditional form submission

**Example - Using Formspree**:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
    <input type="email" name="email" required>
    <textarea name="message" required></textarea>
    <button type="submit">Send</button>
</form>
```

### Performance Issues

#### Problem: Page loads slowly

**Solution**:
1. **Optimize images** - Use smaller file sizes or compress images
2. **Lazy load images** - Add `loading="lazy"` to `<img>` tags
3. **Minimize code** - Remove unused CSS and JavaScript
4. **Use CDN** - Ensure external resources load from CDNs (already done)

#### Problem: Images don't load

**Solution**:
1. **Check image URLs** - Make sure they're accessible
2. **Check image format** - Use common formats (JPG, PNG, WebP)
3. **Check file size** - Large images take longer to load
4. **Use placeholder** - Add `alt` text as fallback

**Example**:
```html
<img src="https://example.com/image.jpg" alt="Description" loading="lazy">
```

### Browser Compatibility

#### Problem: Site looks different in different browsers

**Solution**:
1. **Test in multiple browsers** - Chrome, Firefox, Safari, Edge
2. **Use standard HTML/CSS** - Avoid browser-specific features
3. **Check Tailwind support** - Tailwind works in all modern browsers
4. **Use fallback colors** - Older browsers might not support all colors

#### Problem: Mobile view is broken

**Solution**:
1. **Check viewport meta tag** - Should be present (it is at line 44)
2. **Test on real devices** - Use browser DevTools mobile view
3. **Check touch targets** - Buttons should be at least 44x44px
4. **Test orientation** - Both portrait and landscape

---

## Best Practices for Maintenance

### Regular Maintenance Checklist

- [ ] **Monthly**: Review analytics and update testimonials
- [ ] **Quarterly**: Check all links are working
- [ ] **Quarterly**: Update course information and pricing
- [ ] **Semi-annually**: Review and update privacy/terms pages
- [ ] **Semi-annually**: Check for broken images
- [ ] **Annually**: Update copyright year (automatic in this template)
- [ ] **Annually**: Review SEO and meta descriptions

### Before Making Changes

1. **Backup your file** - Save a copy with today's date
2. **Make one change at a time** - This helps identify issues
3. **Test in browser** - Check each change works
4. **Test on mobile** - Ensure responsive design works

### When Making Updates

1. **Use Find & Replace carefully** - Review changes before applying
2. **Keep consistent styling** - Match existing styles
3. **Update related content** - If you change a feature, update benefits too
4. **Test all links** - Especially after URL updates

### File Organization

**Recommended folder structure**:
```
project/
├── index.html
├── privacy.html
├── terms.html
├── blog.html (optional)
├── css/
│   └── custom.css (if adding custom styles)
├── images/
│   └── your-images.jpg
└── js/
    └── custom.js (if adding custom scripts)
```

---

## Getting Help

### Resources

- **Tailwind CSS Docs**: [tailwindcss.com](https://tailwindcss.com)
- **Font Awesome Icons**: [fontawesome.com/icons](https://fontawesome.com/icons)
- **HTML Reference**: [mdn.org/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **CSS Reference**: [mdn.org/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- **Google Fonts**: [fonts.google.com](https://fonts.google.com)

### Common Questions

**Q: Can I use this template for my business?**
A: Yes! This template is designed to be customized for any leadership or educational business.

**Q: Do I need coding knowledge to use this?**
A: No! This guide provides step-by-step instructions for non-technical users. Basic text editing is all you need.

**Q: How do I host this website?**
A: You can use services like Netlify, Vercel, GitHub Pages, or traditional web hosting. Most offer free tiers.

**Q: Can I add more sections?**
A: Absolutely! Follow the same structure and styling of existing sections.

**Q: How do I add a blog?**
A: Create a `blog.html` file similar to the privacy/terms pages, or use a CMS like WordPress.

---

## Summary

You now have a comprehensive guide to maintaining and customizing your Leadership Academy landing page. Remember:

1. **Always save your changes** before testing
2. **Hard refresh** your browser to see updates
3. **Test on mobile** devices
4. **Keep backups** of working versions
5. **Update links** when your URLs change
6. **Customize content** to match your brand

For questions or issues not covered here, refer to the resource links above or consult with a web developer.

**Happy customizing!** 🚀